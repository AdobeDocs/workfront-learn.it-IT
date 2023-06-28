---
title: Comprendere la modalità testo di base per i filtri
description: Scopri che cosa sono la modalità testo, la notazione a cammello e alcune modalità testo "plug and play" di base che puoi utilizzare nei filtri dei rapporti in Workfront.
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-9086
exl-id: b3f16468-b720-468d-887a-b313fc32bd89
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
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
>* Per comprendere meglio la modalità testo, consigliamo di guardare l’evento del webinar registrato [Ask the Expert - Introduzione al reporting in modalità testo](https://experienceleague.adobe.com/docs/workfront-events/events/reporting-and-dashboards/introduction-to-text-mode-reporting.html?lang=en), della durata di un&#39;ora.
>* Per ulteriori informazioni sulla modalità testo, si consiglia di guardare [Reporting avanzato](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/advanced-reporting/welcome-to-advanced-reporting.html?lang=en) esercitazioni, che insieme durano cinque ore e mezza.


Questo video illustra:

* Che cos’è la modalità testo
* Che cos’è Camel Case
* Alcune modalità di testo &quot;plug and play&quot; di base che puoi utilizzare nei filtri dei rapporti

>[!VIDEO](https://video.tv.adobe.com/v/336820/?quality=12&learn=on)


## Attività: consente di escludere le attività contrassegnate come &quot;Completate con la parte&quot;

La modalità di testo seguente esclude le attività in cui un utente ha contrassegnato &quot;Fine con la mia parte&quot;. È sufficiente creare un filtro delle attività, aggiungere le regole di filtro desiderate, quindi passare alla modalità testo e incollare il codice sottostante dopo qualsiasi modalità di testo visualizzata nel filtro.

```
EXISTS:1:$$OBJCODE=ASSGN  
EXISTS:1:taskID=FIELD:ID  
EXISTS:1:status=DN  
EXISTS:1:status_Mod=notin  
EXISTS:1:assignedToID=$$USER.ID 
```

## Attività: mostra tutte le attività in attesa della mia approvazione

```
approvalProcessID_Mod=notblank
currentUserApproversMM:ID=$$USER.ID
currentUserApproversMM:ID_Mod=in
currentUserApproversMM_Join=allowingnull
```

## Attività: mostra tutte le attività approvate

Crea un rapporto di attività con i filtri desiderati, quindi passa alla scheda Filtro e fai clic su Passa a modalità testo. Aggiungi questo codice a qualsiasi elemento già presente:

```
approvalProcessID_Mod=notblank
approverStatuses:approvedByID=$$USER.ID
approverStatuses:approvedByID_Mod=in
```

## Attività: mostra tutte le attività con almeno un predecessore per più progetti

```
predecessorsMM:ID_Mod=notblank
predecessorsMM:projectID=FIELD:projectID
predecessorsMM:projectID_Mod=ne
```

## Attività: mostra tutte le attività che ho assegnato ad altri

Crea un rapporto di attività con i filtri desiderati, quindi passa alla scheda Filtro e fai clic su Passa a modalità testo. Aggiungi questo codice a qualsiasi elemento già presente:

```
EXISTS:1:$$OBJCODE=ASSGN
EXISTS:1:taskID=FIELD:ID
EXISTS:1:assignedByID=$$USER.ID
```

Verranno visualizzate tutte le attività a cui l&#39;utente connesso ha assegnato almeno uno degli assegnatari correnti. Se gli assegnatari sono stati assegnati da più persone, nella pagina di destinazione dell’attività verrà visualizzato &quot;Richiesto da&quot; solo il nome della prima persona che ha assegnato qualcuno.

## Attività: visualizza tutte le attività completate - In attesa di approvazione

```
status=CPL:A
status_Mod=in
```


## Problema - Mostra tutti i problemi completati - In attesa di approvazione

```
status=CPL:A
status_Mod=in
```


## Progetto - Mostra tutti i progetti completati - In attesa di approvazione

```
status=CPL:A
status_Mod=in
```


## Nota: mostra tutti i commenti in cui sono taggato

```
tags:userID=$$USER.ID
tags:userID_Mod=in
```


## Rapporto su parametri/campi personalizzati: mostra i campi personalizzati non allegati a un modulo personalizzato (molto utile nelle operazioni di pulizia)

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=CTGYPA
EXISTS:A:parameterID=FIELD:ID
```
