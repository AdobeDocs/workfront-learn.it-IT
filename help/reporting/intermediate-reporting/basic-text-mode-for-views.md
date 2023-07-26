---
title: Comprendere la modalità testo di base per le visualizzazioni
description: Scopri che cosa sono la modalità testo, la notazione a cammello e alcune modalità testo "plug and play" di base che puoi utilizzare nelle visualizzazioni di Workfront.
activity: use
feature: Text Mode Reporting
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-11367
exl-id: 156e5510-4a51-449f-9c8c-e16fdd8ea23d
doc-type: video
source-git-commit: 078fa7b82919ada1dcf35791b43f996b875cbf8f
workflow-type: tm+mt
source-wordcount: '685'
ht-degree: 0%

---

# Comprendere la modalità testo di base per le visualizzazioni


>[!IMPORTANT]
>
>Prerequisiti:
>
>* [Comprendere gli elementi di reporting](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/reporting-elements.html?lang=en)
>* [Comprendere i componenti di reporting](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/reporting-components.html?lang=en)
>* [Creare una visualizzazione di base](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/create-a-basic-view.html?lang=en)

>[!TIP]
>
>* Per comprendere meglio la modalità testo, consigliamo di guardare l’evento del webinar registrato [Ask the Expert - Introduzione al reporting in modalità testo](https://experienceleague.adobe.com/docs/workfront-events/events/reporting-and-dashboards/introduction-to-text-mode-reporting.html?lang=en), della durata di un&#39;ora.
>* Per ulteriori informazioni sulla modalità testo, si consiglia di guardare [Reporting avanzato](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/advanced-reporting/welcome-to-advanced-reporting.html?lang=en) esercitazioni, che insieme durano cinque ore e mezza.

Questo video illustra:

* Che cos’è la modalità testo
* Che cos’è Camel Case
* Alcune modalità di testo &quot;plug and play&quot; di base che è possibile utilizzare nelle visualizzazioni

>[!VIDEO](https://video.tv.adobe.com/v/3410571/?quality=12&learn=on)

## Attività - Vista a 4 elementi principali

Creare innanzitutto una colonna per Nome attività e Nome padre, quindi utilizzare la modalità di testo seguente per creare le altre tre colonne.

### Attività: padre del nome padre

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

### Attività: elemento padre del nome padre

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

### Attività: elemento padre dell&#39;elemento padre del nome padre

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

![Un&#39;immagine della schermata che mostra la vista dei 4 elementi principali](assets/4-parents-view.png)

## Utente: iterazioni che mostrano elenchi nelle visualizzazioni utente

### Utente: tutti i ruoli

```
displayname=All job roles
listdelimiter=<p>
listmethod=nested(userRoles).lists
textmode=true
type=iterate
valuefield=role:name
valueformat=HTML
```

### Utente: tutti i ruoli principali visualizzati

```
displayname=All Job Roles showing primary
listdelimiter=<p> 
listmethod=nested(userRoles).lists 
textmode=true
type=iterate 
valueexpression=IF({user}.{roleID}={role}.{ID},CONCAT("** ",{role}.{name}," **"),{role}.{name})
valueformat=HTML
```

### Utente - Tutti i team

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
>È disponibile un campo Team accessibile tramite l’interfaccia utente di che mostra tutti i team, separati da virgole, ma utilizzando la modalità di testo precedente ogni team verrà visualizzato su una riga separata.


### Utente - Tutti i gruppi

```
displayname=All groups
listdelimiter=<p>
listmethod=nested(userGroups).lists
textmode=true
type=iterate
valuefield=group:name
valueformat=HTML
```

### Utente: tutti i gruppi che mostrano il gruppo predefinito

```
displayname=All groups showing home group
listdelimiter=<p>
listmethod=nested(userGroups).lists
textmode=true
type=iterate
valueexpression=IF({user}.{homeGroupID}={group}.{ID},CONCAT("** ",{group}.{name}," **"),{group}.{name})
valueformat=HTML
```


### Utente - Referenti diretti

```
displayname=Direct reports
listdelimiter=<p>
listmethod=nested(directReports).lists
textmode=true
type=iterate
valueexpression={name}
valueformat=HTML
```

### Utente - PTO futuro

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

![Un&#39;immagine della schermata che mostra la vista Elenco utenti](assets/user-lists-view-large.png)

## Attività: come visualizzare le assegnazioni delle attività e lavorare sullo stato

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


## Attività: come visualizzare ruolo e allocazione su più assegnazioni di attività

### Attività - Ruolo + Ore

```
displayname=Role+hours
listdelimiter=<li>
listmethod=nested(assignments).lists
textmode=true
type=iterate
valueexpression=CONCAT({role}.{name}," (",round({workRequired}/60,2),")")
valueformat=HTML
```

### Attività - Assegnazione + allocazione percentuale

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

## Attività: predecessori e successori tra progetti

### Filtro attività (facoltativo)

**Mostra tutte le attività con almeno un predecessore per più progetti o almeno un successore per più progetti nei progetti correnti**

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

### Attività: mostra i nomi dei predecessori e il predecessore del progetto in

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

### Attività: mostra nomi successore e successore progetto in

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

### Attività: mostra la data di completamento prevista dei predecessori

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

### Attività: mostra lo stato di avanzamento dei predecessori

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

### Attività: mostra la percentuale di completamento del progetto del predecessore di un altro progetto

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

![Immagine della schermata che mostra la vista predecessori e successori tra progetti](assets/cross-project-predecessors-and-successors.png)


## Attività: iterazione che mostra tutte le persone assegnate e chi le ha assegnate

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

## Attività/Progetto - Iterazione che mostra tutti i moduli personalizzati su un progetto o un’attività

```
displayname=All Forms Assigned
listdelimiter=<p>
listmethod=nested(objectCategories).lists
textmode=true
type=iterate
valuefield=category:name
valueformat=HTML
```

![Immagine schermata che mostra tutti i moduli personalizzati di un progetto](assets/all-custom-forms-on-a-project.png)


## Progetto: iterazione che mostra tutti i contatti principali per i risolvibili nella vista Progetto

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

## Progetto: iterazione che mostra tutti i membri del team di progetto

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

![Un&#39;immagine della schermata che mostra tutti i membri del team di progetto](assets/all-project-team-members.png)

## Progetto: iterazione che mostra la data di entrata di tutte le Issues risolvibili di un progetto

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

![Immagine schermata che mostra la data di entrata di tutti i problemi risolvibili per un progetto](assets/resolvables-entry-date.png)

## Progetto: mostra il gruppo predefinito del richiedente del progetto originale

```
displayname=Requestor home group
linkedname=direct
namekey=name
querysort=convertedOpTaskOriginator:homeGroup:name
textmode=true
valuefield=convertedOpTaskOriginator:homeGroup:name
valueformat=HTML
```

![Immagine della schermata che mostra il gruppo predefinito del richiedente del progetto](assets/requestor-home-group.png)

## Progetto: mostra se il progetto è una coda di richieste

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

![Immagine che mostra se il progetto è una coda di richieste](assets/project-is-a-request-queue.png)

## Problema: iterazione che mostra tutti i membri del team del progetto di risoluzione

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

![Un&#39;immagine della schermata che mostra tutti i membri del team di progetto di risoluzione](assets/all-resolve-project-team-members.png)

## Problema: iterazione che mostra tutti i team del contatto principale del problema

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

![Un&#39;immagine della schermata che mostra tutti i team di contatto principali](assets/all-primary-contact-teams.png)

## Documento - Iterazione che mostra la cartella in un rapporto di documento

```
displayname=Folder
listdelimiter=<br><br>
listmethod=nested(folders).lists
textmode=true
type=iterate
valuefield=name
valueformat=HTML
```

![Immagine schermata che mostra la cartella in un report documento](assets/folder-in-a-document-report.png)

## Documento: iterazione che mostra la cartella principale in un rapporto di documento

```
displayname=Parent Folder
listdelimiter=<br><br>
listmethod=nested(folders).lists
textmode=true
type=iterate
valuefield=parent:name
valueformat=HTML
```

![Immagine schermata che mostra la cartella principale in un report di documenti](assets/parent-folder-in-a-document-report.png)

## Documento - Date di approvazione documento

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

![Immagine che mostra la visualizzazione delle date di approvazione del documento](assets/document-approval-dates.png)

## Approvazioni bozze

### Approvazione bozza - Mostra nome progetto

```
displayname=Project Name
textmode=true 
valuefield=documentVersion:document:project:name 
valueformat=HTML
```

### Approvazione bozza - Mostra nome attività

```
displayname=Task Name
textmode=true 
valuefield=documentVersion:document:task:name 
valueformat=HTML
```

![Immagine schermata che mostra il progetto e l’attività dell’approvazione di una bozza](assets/proof-approval-project-and-task.png)
