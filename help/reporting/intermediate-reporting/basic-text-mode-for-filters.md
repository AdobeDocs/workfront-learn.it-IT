---
title: Comprendere la modalità testo di base per i filtri
description: Scopri la modalità testo, il cammello e la modalità testo "plug and play" di base che puoi utilizzare nei filtri dei rapporti in [!DNL  Workfront].
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 9086
exl-id: b3f16468-b720-468d-887a-b313fc32bd89
source-git-commit: 59ac9907b116f8abadf5e15f8de351c02a7a2909
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---

# Comprendere la modalità testo di base per i filtri

>[!IMPORTANT]
>
>Prerequisiti:
>
>* Comprendere gli elementi di reporting
>* Comprendere i componenti di reporting
>* Creare un filtro di base


In questo video imparerai:

* Modalità testo
* Che caso di cammello è
* Modalità testo &quot;plug and play&quot; di base utilizzabile nei filtri dei rapporti

>[!VIDEO](https://video.tv.adobe.com/v/336820/?quality=12)

La seguente modalità di testo esclude le attività in cui l’utente ha contrassegnato la dicitura &quot;Fine con la parte personale&quot;. Tutto quello che devi fare è creare un filtro attività, aggiungere le regole di filtro desiderate, quindi passare alla modalità testo e incollare il codice sottostante dopo qualsiasi modalità di testo che vedi nel filtro.

```
EXISTS:1:$$OBJCODE=ASSGN  
EXISTS:1:taskID=FIELD:ID  
EXISTS:1:status=DN  
EXISTS:1:status_Mod=notin  
EXISTS:1:assignedToID=$$USER.ID 
```

## Filtri aggiuntivi per la modalità plug-in e play text

### Attività - Visualizza tutte le attività in attesa di approvazione

```
approvalProcessID_Mod=notblank
currentUserApproversMM:ID=$$USER.ID
currentUserApproversMM:ID_Mod=in
currentUserApproversMM_Join=allowingnull
```

### Attività - Visualizza tutte le attività approvate

Crea un rapporto di attività con i filtri desiderati, quindi vai alla scheda Filtro e fai clic su Passa alla modalità di testo. Aggiungi questo codice a qualsiasi elemento già presente:

```
approvalProcessID_Mod=notblank
approverStatuses:approvedByID=$$USER.ID
approverStatuses:approvedByID_Mod=in
```

### Attività: visualizza tutte le attività con almeno un predecessore di progetto incrociato

```
predecessorsMM:ID_Mod=notblank
predecessorsMM:projectID=FIELD:projectID
predecessorsMM:projectID_Mod=ne
```

### Attività - Visualizza tutti i task assegnati ad altri

Crea un rapporto di attività con i filtri desiderati, quindi vai alla scheda Filtro e fai clic su Passa alla modalità di testo. Aggiungi questo codice a qualsiasi elemento già presente:

```
EXISTS:1:$$OBJCODE=ASSGN
EXISTS:1:taskID=FIELD:ID
EXISTS:1:assignedByID=$$USER.ID
```

Verranno visualizzate tutte le attività a cui l&#39;utente connesso ha assegnato almeno uno degli assegnatari correnti. Se gli assegnatari sono stati assegnati da più persone, nella pagina di destinazione dell’attività verrà visualizzato solo il nome della prima persona che ha assegnato un utente come &quot;Richiesto da&quot;.

## Attività: Domande sulla modalità testo

1. Come si scrive il cammello per il campo &quot;Inserito per ID&quot;?
1. In un rapporto del problema, crea un filtro per mostrare i problemi che sono stati contrassegnati come chiusi ma che sono in attesa di approvazione.

### Risposte

1. Il cammello del campo &quot;Inserito da ID&quot; deve essere scritto in questo modo—enterByID
1. La modalità di testo dovrebbe essere simile alla seguente nel filtro per report dei problemi:

   ![Immagine della schermata per creare un nuovo filtro in modalità testo](assets/btm-answer.png)
