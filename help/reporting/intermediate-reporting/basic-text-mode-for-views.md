---
title: Comprendere la modalità testo di base per le visualizzazioni
description: Scopri la modalità testo, il cammello e alcune modalità testo "plug and play" di base che puoi utilizzare nelle visualizzazioni in Workfront.
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 11367
exl-id: 156e5510-4a51-449f-9c8c-e16fdd8ea23d
doc-type: video
source-git-commit: 650e4d346e1792863930dcebafacab4c88f2a8bc
workflow-type: tm+mt
source-wordcount: '650'
ht-degree: 0%

---

# Comprendere la modalità testo di base per le visualizzazioni


>[!IMPORTANT]
>
>Prerequisiti:
>
>* Comprendere gli elementi di reporting
>* Comprendere i componenti di reporting
>* Creare una visualizzazione di base


>[!TIP]
>
>* Per una comprensione più approfondita della modalità di testo, si consiglia di guardare l&#39;evento del webinar registrato [Chiedi all&#39;esperto - Introduzione al reporting in modalità testo](https://experienceleague.adobe.com/docs/workfront-events/events/reporting-and-dashboards/introduction-to-text-mode-reporting.html?lang=en), che dura un&#39;ora.
>* Per ulteriori informazioni sulla modalità testo, si consiglia di guardare la [Rapporti avanzati](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/advanced-reporting/welcome-to-advanced-reporting.html?lang=en) i tutorial, che insieme sono lunghi cinque ore e mezza.


In questo video imparerai:

* Modalità testo
* Che caso di cammello è
* Alcune modalità di testo &quot;plug and play&quot; di base possono essere utilizzate nelle visualizzazioni

>[!VIDEO](https://video.tv.adobe.com/v/3410571/?quality=12&learn=on)

## Attività - Visualizzazione 4 elementi principali

Crea prima una colonna per Nome attività e Nome padre, quindi utilizza la seguente modalità di testo per creare le altre tre colonne.

### Attività - Elemento padre del nome padre

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

### Attività - Elemento padre del nome padre

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

### Attività - Elemento padre del nome padre

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

![Immagine dello schermo che mostra la visualizzazione dei 4 elementi principali](assets/4-parents-view.png)

## Utente - Iterazioni che mostrano gli elenchi nelle visualizzazioni utente

### Utente - Tutti i ruoli di lavoro

```
displayname=All job roles
listdelimiter=<p>
listmethod=nested(userRoles).lists
textmode=true
type=iterate
valuefield=role:name
valueformat=HTML
```

### Utente: tutti i ruoli di lavoro che mostrano il ruolo primario

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
>È disponibile un campo Team accessibile tramite l’interfaccia utente che mostra tutti i team, separati da virgole, ma utilizzando la modalità di testo di cui sopra ogni team verrà visualizzato su una riga separata.


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

### Utente: tutti i gruppi che mostrano il gruppo home

```
displayname=All groups showing home group
listdelimiter=<p>
listmethod=nested(userGroups).lists
textmode=true
type=iterate
valueexpression=IF({user}.{homeGroupID}={group}.{ID},CONCAT("** ",{group}.{name}," **"),{group}.{name})
valueformat=HTML
```


### Utente - Rapporti diretti

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

![Immagine di una schermata che mostra la visualizzazione degli elenchi utente](assets/user-lists-view-large.png)

## Attività: modalità di visualizzazione delle assegnazioni delle attività e utilizzo dello stato

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

![Immagine della schermata con le visualizzazioni Assegnazioni e Stato](assets/assignments-and-status-view.png)


## Attività: modalità di visualizzazione del ruolo e dell&#39;allocazione in più assegnazioni di attività

### Attività - Ruolo + ore

```
displayname=Role+hours
listdelimiter=<li>
listmethod=nested(assignments).lists
textmode=true
type=iterate
valueexpression=CONCAT({role}.{name}," (",round({workRequired}/60,2),")")
valueformat=HTML
```

### Attività - Assegnazione + percentuale di allocazione

```
displayname=Assignment+percent
valueexpression=CONCAT({assignedTo}.{name}," (",{assignmentPercent},")")
listdelimiter=<li>
listmethod=nested(assignments).lists
valueformat=HTML
textmode=true
type=iterate
```

![Immagine della schermata che mostra la vista Assegnazioni e Ruoli](assets/assignments-roles-and-percent-view.png)

## Attività: predecessori e successori di progetti diversi

### Filtro attività (facoltativo)

**Visualizza tutte le attività con almeno un predecessore di progetto incrociato**

```
predecessorsMM:ID_Mod=notblank
predecessorsMM:projectID=FIELD:projectID
predecessorsMM:projectID_Mod=ne
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

### Attività: mostra i nomi dei successori e il successore del progetto è in

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

### Task - Visualizza la data di completamento prevista dei predecessori

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

### Task - Visualizza lo stato di avanzamento dei predecessori

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

### Attività: mostra la percentuale di completamento del progetto del predecessore di più progetti

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

![Immagine della schermata che mostra la vista predecessori e successori di progetti incrociati](assets/cross-project-predecessors-and-successors.png)


## Attività : iterazione che mostra tutte le persone assegnate e che le hanno assegnate

```
displayname=All assignees and requesters
listdelimiter=<p>
listmethod=nested(assignments).lists
textmode=true
type=iterate
valueexpression=CONCAT("Assigned To: ",{assignedTo}.{name},"; Requested By: ",{assignedBy}.{name})
valueformat=HTML
```

![Immagine dello schermo che mostra tutte le persone assegnate e che le hanno assegnate](assets/all-assignees-and-requesters.png)

## Attività/Progetto : iterazione per visualizzare tutti i moduli personalizzati su un progetto o un&#39;attività

```
displayname=All Forms Assigned
listdelimiter=<p>
listmethod=nested(objectCategories).lists
textmode=true
type=iterate
valuefield=category:name
valueformat=HTML
```

![Un’immagine a schermo che mostra tutti i moduli personalizzati in un progetto](assets/all-custom-forms-on-a-project.png)


## Progetto - Iterazione che mostra tutti i contatti principali per i resolvables nella visualizzazione del progetto

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

![Un&#39;immagine a schermo che mostra i contatti primari per i resolubili](assets/primary-contacts-for-resolvables.png)

## Progetto: iterazione che mostra tutti i membri del team del progetto

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

![Un’immagine a schermo che mostra tutti i membri del team di progetto](assets/all-project-team-members.png)

## Progetto: iterazione che mostra l&#39;entryDate di tutti i problemi risolvibili per un progetto

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

![Immagine della schermata che mostra l&#39;entryDate di tutti i problemi risolvibili per un progetto](assets/resolvables-entry-date.png)

## Progetto: mostra il gruppo home del richiedente del progetto originale

```
displayname=Requestor home group
linkedname=direct
namekey=name
querysort=convertedOpTaskOriginator:homeGroup:name
textmode=true
valuefield=convertedOpTaskOriginator:homeGroup:name
valueformat=HTML
```

![Immagine della schermata che mostra il richiedente del progetto o il gruppo home](assets/requestor-home-group.png)

## Progetto: mostra se il progetto è una coda di richiesta

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

![Immagine della schermata che mostra se il progetto è una coda di richiesta](assets/project-is-a-request-queue.png)

## Problema: iterazione che mostra tutti i membri del team di progetto di risoluzione

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

![Immagine della schermata che mostra tutti i membri del team di progetto risolti](assets/all-resolve-project-team-members.png)

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

![Un’immagine a schermo che mostra tutti i team di contatto principali](assets/all-primary-contact-teams.png)

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

![Immagine di una schermata che mostra la cartella in un rapporto di documento](assets/folder-in-a-document-report.png)

## Documento - Iterazione che mostra la cartella padre in un report di documento

```
displayname=Parent Folder
listdelimiter=<br><br>
listmethod=nested(folders).lists
textmode=true
type=iterate
valuefield=parent:name
valueformat=HTML
```

![Immagine di una schermata che mostra la cartella principale in un report di documento](assets/parent-folder-in-a-document-report.png)

## Documento - Date di approvazione documento

```
displayname=Document Approval Dates
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

![Immagine della schermata che mostra la visualizzazione Date approvazione documento](assets/document-approval-dates.png)

## Approvazioni bozze

### Approvazione bozza - Visualizza nome progetto

```
displayname=Project Name
textmode=true 
valuefield=documentVersion:document:project:name 
valueformat=HTML
```

### Approvazione bozza - Visualizza nome attività

```
displayname=Task Name
textmode=true 
valuefield=documentVersion:document:task:name 
valueformat=HTML
```

![Immagine a schermo che mostra il progetto e l’attività di un’approvazione della bozza](assets/proof-approval-project-and-task.png)
