---
title: Comprendere la modalità testo di base per i filtri
description: Scopri la modalità testo, il cammello e alcune modalità testo "plug and play" di base utilizzabili nei filtri per report in Workfront.
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 9086
exl-id: b3f16468-b720-468d-887a-b313fc32bd89
doc-type: video
source-git-commit: 650e4d346e1792863930dcebafacab4c88f2a8bc
workflow-type: tm+mt
source-wordcount: '416'
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


>[!TIP]
>
>* Per una comprensione più approfondita della modalità di testo, si consiglia di guardare l&#39;evento del webinar registrato [Chiedi all&#39;esperto - Introduzione al reporting in modalità testo](https://experienceleague.adobe.com/docs/workfront-events/events/reporting-and-dashboards/introduction-to-text-mode-reporting.html?lang=en), che dura un&#39;ora.
>* Per ulteriori informazioni sulla modalità testo, si consiglia di guardare la [Rapporti avanzati](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/advanced-reporting/welcome-to-advanced-reporting.html?lang=en) i tutorial, che insieme sono lunghi cinque ore e mezza.



In questo video imparerai:

* Modalità testo
* Che caso di cammello è
* Modalità testo &quot;plug and play&quot; di base utilizzabile nei filtri dei rapporti

>[!VIDEO](https://video.tv.adobe.com/v/336820/?quality=12&learn=on)


## Attività - Filtrare le attività in cui ho contrassegnato &quot;Fine con la parte&quot;

La seguente modalità di testo esclude le attività in cui l’utente ha contrassegnato la dicitura &quot;Fine con la parte personale&quot;. Tutto quello che devi fare è creare un filtro attività, aggiungere le regole di filtro desiderate, quindi passare alla modalità testo e incollare il codice sottostante dopo qualsiasi modalità di testo che vedi nel filtro.

```
EXISTS:1:$$OBJCODE=ASSGN  
EXISTS:1:taskID=FIELD:ID  
EXISTS:1:status=DN  
EXISTS:1:status_Mod=notin  
EXISTS:1:assignedToID=$$USER.ID 
```

## Attività - Visualizza tutte le attività in attesa di approvazione

```
approvalProcessID_Mod=notblank
currentUserApproversMM:ID=$$USER.ID
currentUserApproversMM:ID_Mod=in
currentUserApproversMM_Join=allowingnull
```

## Attività - Visualizza tutte le attività approvate

Crea un rapporto di attività con i filtri desiderati, quindi vai alla scheda Filtro e fai clic su Passa alla modalità di testo. Aggiungi questo codice a qualsiasi elemento già presente:

```
approvalProcessID_Mod=notblank
approverStatuses:approvedByID=$$USER.ID
approverStatuses:approvedByID_Mod=in
```

## Attività: visualizza tutte le attività con almeno un predecessore di progetto incrociato

```
predecessorsMM:ID_Mod=notblank
predecessorsMM:projectID=FIELD:projectID
predecessorsMM:projectID_Mod=ne
```

## Attività - Visualizza tutti i task assegnati ad altri

Crea un rapporto di attività con i filtri desiderati, quindi vai alla scheda Filtro e fai clic su Passa alla modalità di testo. Aggiungi questo codice a qualsiasi elemento già presente:

```
EXISTS:1:$$OBJCODE=ASSGN
EXISTS:1:taskID=FIELD:ID
EXISTS:1:assignedByID=$$USER.ID
```

Verranno visualizzate tutte le attività a cui l&#39;utente connesso ha assegnato almeno uno degli assegnatari correnti. Se gli assegnatari sono stati assegnati da più persone, nella pagina di destinazione dell’attività verrà visualizzato solo il nome della prima persona che ha assegnato un utente come &quot;Richiesto da&quot;.

## Attività - Visualizza tutte le attività completate - In attesa di approvazione

```
status=CPL:A
status_Mod=in
```


## Problema: visualizza tutti i problemi completati - In attesa di approvazione

```
status=CPL:A
status_Mod=in
```


## Progetto - Visualizza tutti i progetti completati - In attesa di approvazione

```
status=CPL:A
status_Mod=in
```


## Nota: visualizza tutti i commenti con tag

```
tags:userID=$$USER.ID
tags:userID_Mod=in
```


## Rapporto campo personalizzato/parametro : visualizza campi personalizzati non associati a un modulo personalizzato (molto utile nelle operazioni di pulizia)

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=CTGYPA
EXISTS:A:parameterID=FIELD:ID
```
