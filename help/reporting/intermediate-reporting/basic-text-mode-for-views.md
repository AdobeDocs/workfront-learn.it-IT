---
title: Comprendere la modalità testo di base per le visualizzazioni
description: Scopri la modalità testo, la notazione a cammello e alcune modalità testo di base che puoi utilizzare nelle visualizzazioni dei rapporti in Workfront.
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
last-substantial-update: 2025-08-12T00:00:00Z
jira: KT-11367
exl-id: 156e5510-4a51-449f-9c8c-e16fdd8ea23d
doc-type: video
source-git-commit: 062a7f3576c4d5af02b04340e9763a82a9b8c721
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 93%

---

# Comprendere la modalità testo di base per le visualizzazioni


>[!PREREQUISITES]
>
>* [Informazioni sugli elementi di reporting](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/reporting-elements.html?lang=it)
>* [Informazioni sui componenti di reporting](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/reporting-components.html?lang=it)
>* [Creare una vista di base](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/create-a-basic-view.html?lang=it)


>[!TIP]
>
>* Per comprendere meglio la modalità testo, ti consigliamo di guardare l’evento webinar registrato [Le domande agli esperti - Introduzione alla reportistica in modalità testo](https://experienceleague.adobe.com/it/docs/events/classics/reporting-and-dashboards/introduction-to-text-mode-reporting), della durata di un’ora.
>* Per ulteriori informazioni sulla modalità testo, ti consigliamo di guardare i tutorial sulla [Reportistica avanzata](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/advanced-reporting/welcome-to-advanced-reporting.html?lang=it) che hanno una durata totale di cinque ore e mezzo.
>* Fai clic qui per accedere a [[!UICONTROL API Explorer]](https://developer.adobe.com/workfront/api-explorer/)

In questo video scoprirai:

* Che cos’è la modalità testo
* Che cos’è la notazione a cammello
* Alcuni _blocchi di codice in modalità testo_ che puoi utilizzare nelle visualizzazioni dei report

>[!VIDEO](https://video.tv.adobe.com/v/3470796/?quality=12&learn=on&captions=ita)

## Attività &quot;Comprendere la modalità testo di base per le visualizzazioni&quot;

### Attività: vista a 4 elementi principali

Crea innanzitutto una colonna per il Nome attività e il Nome principale, quindi utilizza la modalità testo seguente per creare le altre tre colonne.

#### Attività: principale del nome principale

```
displayname=Parent of Parent Name
linkedname=parent
namekey=view.relatedcolumn
namekeyargkey.0=parent
namekeyargkey.1=name
querysort=parent:parent:name
textmode=true
valuefield=parent:parent:name
valueformat=HTML
```

#### Attività: principale del principale del nome principale

```
displayname=Parent of Parent of Parent Name
linkedname=parent
namekey=view.relatedcolumn
namekeyargkey.0=parent
namekeyargkey.1=name
querysort=parent:parent:parent:name
textmode=true
valuefield=parent:parent:parent:name
valueformat=HTML
```

#### Attività: principale del principale del principale del nome principale

```
displayname=Parent of Parent of Parent of Parent Name
linkedname=parent
namekey=view.relatedcolumn
namekeyargkey.0=parent
namekeyargkey.1=name
querysort=parent:parent:parent:parent:name
textmode=true
valuefield=parent:parent:parent:parent:name
valueformat=HTML
```

![Immagine dello schermo che mostra la vista a 4 elementi principali](assets/4-parents-view.png)

### Utente: iterazioni che mostrano gli elenchi nelle viste utente

#### Utente: tutte le mansioni

```
displayname=All job roles
listdelimiter=<p>
listmethod=nested(userRoles).lists
textmode=true
type=iterate
valuefield=role:name
valueformat=HTML
```

#### Utente: tutte le mansioni visualizzate come primarie

```
displayname=All Job Roles showing primary
listdelimiter=<p> 
listmethod=nested(userRoles).lists 
textmode=true
type=iterate 
valueexpression=IF({user}.{roleID}={role}.{ID},CONCAT("** ",{role}.{name}," **"),{role}.{name})
valueformat=HTML
```

#### Utente: tutti i team

```
displayname=All teams
listdelimiter=<p>
listmethod=nested(teams).lists
textmode=true
type=iterate
valueexpression={name}
valueformat=HTML
```

>[!NOTE]
>
>È disponibile un campo Team accessibile dall’interfaccia utente che mostra tutti i team, separati da virgole. Con la modalità testo precedente, ogni team verrà invece visualizzato su una riga separata.


#### Utente: tutti i gruppi

```
displayname=All groups
listdelimiter=<p>
listmethod=nested(userGroups).lists
textmode=true
type=iterate
valuefield=group:name
valueformat=HTML
```

#### Utente: tutti i gruppi che mostrano il gruppo home

```
displayname=All groups showing home group
listdelimiter=<p>
listmethod=nested(userGroups).lists
textmode=true
type=iterate
valueexpression=IF({user}.{homeGroupID}={group}.{ID},CONCAT("** ",{group}.{name}," **"),{group}.{name})
valueformat=HTML
```


#### Utente: referenti diretti

```
displayname=Direct reports
listdelimiter=<p>
listmethod=nested(directReports).lists
textmode=true
type=iterate
valueexpression={name}
valueformat=HTML
```

#### Utente: Future PTO (Ferie future)

```
displayname=Future PTO
listdelimiter=<br>
listmethod=nested(reservedTimes).lists
namekey=group.plural
textmode=true
type=iterate
valueexpression=IF({startDate}>$$TODAY,CONCAT({startDate}," - ",{endDate}),"")
valueformat=HTML
width=150
```

![Immagine della schermata che mostra la vista con l’elenco degli utenti](assets/user-lists-view-large.png)

### Attività: come visualizzare le assegnazioni delle attività e lavorare sullo stato

```
displayname=Assignments and Status
listdelimiter=<br>
listmethod=nested(assignments).lists
namekey=group.plural
textmode=true
type=iterate
valueexpression=CONCAT({assignedTo}.{name},IF(ISBLANK({assignedTo}.{name}),"",IF({status}="AA"," - Requested",IF({status}="AD"," - Working"," - Done"))))
valueformat=HTML
width=150
```

![Immagine che mostra la vista Assegnazioni e Stato](assets/assignments-and-status-view.png)


### Attività: come mostrare il ruolo e l’assegnazione su più assegnazioni di attività

#### Attività: ruolo + ore

```
displayname=Role+hours
listdelimiter=<li>
listmethod=nested(assignments).lists
textmode=true
type=iterate
valueexpression=CONCAT({role}.{name}," (",round({workRequired}/60,2),")")
valueformat=HTML
```

#### Attività: assegnazione + allocazione percentuale

```
displayname=Assignment+percent
valueexpression=CONCAT({assignedTo}.{name}," (",{assignmentPercent},")")
listdelimiter=<li>
listmethod=nested(assignments).lists
valueformat=HTML
textmode=true
type=iterate
```

![Immagine della schermata che mostra la vista Assegnazioni e ruoli](assets/assignments-roles-and-percent-view.png)

### Attività: predecessori e successori tra progetti

#### Filtro attività (facoltativo)

**Mostra tutte le attività nei progetti correnti con almeno un predecessore o un successore in altri progetti**

```
predecessorsMM:ID_Mod=notblank
predecessorsMM:projectID=FIELD:projectID
predecessorsMM:projectID_Mod=ne
project:statusEquatesWith=CUR
project:statusEquatesWith_Mod=in
OR:1:project:statusEquatesWith=CUR
OR:1:project:statusEquatesWith_Mod=in
OR:1:successorsMM:ID_Mod=notblank
OR:1:successorsMM:projectID=FIELD:projectID
OR:1:successorsMM:projectID_Mod=ne
```

#### Attività: mostra nomi dei predecessori e progetto del predecessore in

```
displayname=Predecessor names
listdelimiter=<br>
listmethod=nested(predecessors).lists
namekey=group.plural
textmode=true
type=iterate
valueexpression=CONCAT("TASK = ",{predecessor}.{name}," >> PROJECT = ",{predecessor}.{project}.{name})
valueformat=HTML
width=150
```

#### Attività: mostra nomi dei successori e progetto del successore in

```
displayname=Successor names
listdelimiter=<br>
listmethod=nested(successors).lists
namekey=group.plural
textmode=true
type=iterate
valueexpression=CONCAT("TASK = ",{successor}.{name}," >> PROJECT = ",{successor}.{project}.{name})
valueformat=HTML
width=150
```

#### Attività: mostra la data di completamento prevista dei predecessori

```
displayname=Predecessor projected completion dates
valueformat=atDate
listdelimiter=
textmode=true
width=90
stretch=0
valuefield=predecessor:projectedCompletionDate
type=iterate
listmethod=nested(predecessors).lists
shortview=false
```

#### Attività: mostra lo stato di avanzamento dei predecessori

```
displayname=Predecessor progress status
listdelimiter=<br>
listmethod=nested(predecessors).lists
shortview=false
stretch=0
textmode=true
type=iterate
valueexpression=IF({predecessor}.{progressStatus}="OT","On Time",IF({predecessor}.{progressStatus}="LT","Late",IF({predecessor}.{progressStatus}="BH","Behind","At Risk")))
valueformat=HTML
width=90
```

#### Attività: mostra la percentuale di completamento del progetto del predecessore in altri progetti

```
displayname=Predecessor project percent complete
listdelimiter=<br>
listmethod=nested(predecessors).lists
namekey=group.plural
textmode=true
type=iterate
valueexpression=IF({isCP}=true,CONCAT({predecessor}.{project}.{percentComplete},"%"),"")
valueformat=HTML
width=150
```

![Immagine della schermata che mostra la vista predecessori e successori in altri progetti](assets/cross-project-predecessors-and-successors.png)


### Attività: iterazione che mostra tutte le persone assegnate e chi le ha assegnate

```
displayname=All assignees and requesters
listdelimiter=<p>
listmethod=nested(assignments).lists
textmode=true
type=iterate
valueexpression=CONCAT("Assigned To: ",{assignedTo}.{name},"; Requested By: ",{assignedBy}.{name})
valueformat=HTML
```

![Immagine della schermata che mostra tutte le persone assegnate e chi le ha assegnate](assets/all-assignees-and-requesters.png)

### Attività/progetto: iterazione che mostra tutti i moduli personalizzati su un progetto o un’attività

```
displayname=All Forms Assigned
listdelimiter=<p>
listmethod=nested(objectCategories).lists
textmode=true
type=iterate
valuefield=category:name
valueformat=HTML
```

![Immagine della schermata che mostra tutti i moduli personalizzati di un progetto](assets/all-custom-forms-on-a-project.png)


### Progetto: iterazione che mostra tutti i contatti principali per i risolvibili nella vista Progetto

```
displayname=Requestor
listdelimiter=<br>
listmethod=nested(resolvables).lists
namekey=group.plural
textmode=true
type=iterate
valuefield=owner:name
valueformat=HTML
width=150
```

![Immagine della schermata che mostra i contatti principali per i risolvibili](assets/primary-contacts-for-resolvables.png)

### Progetto: iterazione che mostra tutti i membri del team di progetto

```
displayname=Project Team Members
listdelimiter=<br>
listmethod=nested(projectUsers).lists
namekey=group.plural
textmode=true
type=iterate
valuefield=user:name
valueformat=HTML
```

![Immagine della schermata che mostra tutti i membri del team di progetto](assets/all-project-team-members.png)

### Progetto: iterazione che mostra la data di immissione di tutti i problemi risolvibili per un progetto

```
displayname=Resolvables entry date
linkedname=direct
listdelimiter=<br>
listmethod=nested(project.resolvables).lists
listsort=string(description)
querysort=description
section=0
textmode=true
type=iterate
valuefield=entryDate
valueformat=HTML
```

![Immagine della schermata che mostra la data di immissione di tutti i problemi risolvibili per un progetto](assets/resolvables-entry-date.png)

### Progetto: mostra il gruppo home del richiedente del progetto originale

```
displayname=Requestor home group
linkedname=direct
namekey=name
querysort=convertedOpTaskOriginator:homeGroup:name
textmode=true
valuefield=convertedOpTaskOriginator:homeGroup:name
valueformat=HTML
```

![Immagine della schermata che mostra il gruppo home del richiedente del progetto](assets/requestor-home-group.png)

### Progetto: mostra se il progetto è una coda di richieste

```
querysort=queueDef:isPublic
valueformat=val
description=0 (None), 1 (Public), 2 (Private), 3 (Company), 4 (Group)
linkedname=direct
textmode=true
enumtype=PROJ
valuefield=queueDef:isPublic
namekey=status
type=enum
enumclass=com.attask.common.constants.ProjectStatusEnum
displayname=Public Selection
```

![Immagine della schermata che mostra se il progetto è una coda di richieste](assets/project-is-a-request-queue.png)

### Problema: iterazione che mostra tutti i membri del gruppo del progetto risolutivo

```
displayname=Resolve Project: Team Members
listdelimiter=<br>
listmethod=nested(resolveProject.projectUsers).lists
namekey=group.plural
textmode=true
type=iterate
valuefield=user:name
valueformat=HTML
width=150
```

![Immagine della schermata che mostra tutti i membri del gruppo del progetto risolutivo](assets/all-resolve-project-team-members.png)

### Problema: iterazione che mostra tutti i team del contatto principale del problema

```
displayname=Requestor Teams
listdelimiter=<br>
listmethod=nested(owner.teams).lists
namekey=group.plural
textmode=true
type=iterate
valuefield=name
valueformat=HTML
width=150
```

![Immagine della schermata che mostra tutti i team del contatto principale](assets/all-primary-contact-teams.png)

### Documento: iterazione che mostra la cartella in un rapporto del documento

```
displayname=Folder
listdelimiter=<br><br>
listmethod=nested(folders).lists
textmode=true
type=iterate
valuefield=name
valueformat=HTML
```

![Immagine della schermata che mostra la cartella in un rapporto del documento](assets/folder-in-a-document-report.png)

### Documento: iterazione che mostra la cartella principale in un rapporto del documento

```
displayname=Parent Folder
listdelimiter=<br><br>
listmethod=nested(folders).lists
textmode=true
type=iterate
valuefield=parent:name
valueformat=HTML
```

![Immagine della schermata che mostra la cartella principale in un rapporto del documento](assets/parent-folder-in-a-document-report.png)

### Documento: date di approvazione del documento

```
displayname=Document approval dates
valueformat=HTML
listdelimiter=<br>
linkedname=direct
textmode=true
listsort=string(description)
valuefield=approvalDate
type=iterate
listmethod=nested(approvals).lists
shortview=false
section=0
```

![Immagine della schermata che mostra la visualizzazione delle date di approvazione del documento](assets/document-approval-dates.png)

### Approvazioni bozze

#### Approvazione bozza: mostra il nome del progetto

```
displayname=Project Name
textmode=true 
valuefield=documentVersion:document:project:name 
valueformat=HTML
```

#### Approvazione bozza: mostra il nome dell’attività

```
displayname=Task Name
textmode=true 
valuefield=documentVersion:document:task:name 
valueformat=HTML
```

![Immagine della schermata che mostra il progetto e l’attività di approvazione bozza](assets/proof-approval-project-and-task.png)
