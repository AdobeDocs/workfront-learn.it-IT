---
title: Informazioni sulla modalità testo di base per i filtri
description: Scopri cosa sono la modalità testo, la notazione a cammello e alcune modalità testo “plug and play” di base che puoi utilizzare nei filtri dei rapporti in Workfront.
activity: use
feature: Text Mode Reporting
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-9086
exl-id: b3f16468-b720-468d-887a-b313fc32bd89
doc-type: video
source-git-commit: 409147f9a62302d28e14b834981992a0421d4e4b
workflow-type: ht
source-wordcount: '416'
ht-degree: 100%

---

# Informazioni sulla modalità testo di base per i filtri

>[!IMPORTANT]
>
>Prerequisiti:
>
>* Comprendere gli elementi del reporting
>* Comprendere i componenti di reporting
>* Creare un filtro di base

>[!TIP]
>
>* Per acquisire una comprensione più approfondita della modalità testo, ti consigliamo di guardare l’evento webinar registrato [Le domande agli esperti - Introduzione al reporting in modalità testo](https://experienceleague.adobe.com/docs/workfront-events/events/reporting-and-dashboards/introduction-to-text-mode-reporting.html?lang=it) della durata di un’ora.
>* Per saperne di più sulla modalità testo ti consigliamo di guardare i tutorial sul [Reporting avanzato](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/advanced-reporting/welcome-to-advanced-reporting.html?lang=it), che insieme hanno una durata di cinque ore e mezza.


In questo video scoprirai:

* Che cos’è la modalità testo
* Che cos’è la notazione a cammello
* Alcune modalità di testo “plug and play” di base che puoi utilizzare nei filtri dei rapporti

>[!VIDEO](https://video.tv.adobe.com/v/336820/?quality=12&learn=on)


## Attività: escludere le attività contrassegnate come “Ho terminato la mia parte”

La seguente modalità di testo escluderà le attività che un utente ha contrassegnato come “Ho terminato la mia parte”. È sufficiente creare un filtro delle attività, aggiungere le regole di filtro desiderate, quindi passare alla modalità testo e incollare il codice sottostante dopo qualsiasi modalità di testo visualizzata nel filtro.

```
EXISTS:1:$$OBJCODE=ASSGN  
EXISTS:1:taskID=FIELD:ID  
EXISTS:1:status=DN  
EXISTS:1:status_Mod=notin  
EXISTS:1:assignedToID=$$USER.ID 
```

## Attività: mostrare tutte le attività in attesa della mia approvazione

```
approvalProcessID_Mod=notblank
currentUserApproversMM:ID=$$USER.ID
currentUserApproversMM:ID_Mod=in
currentUserApproversMM_Join=allowingnull
```

## Attività: mostrare tutte le attività approvate

Crea un rapporto di attività con i filtri desiderati, quindi passa alla scheda Filtro e fai clic su Passa a modalità testo. Aggiungi questo codice a un elemento già presente:

```
approvalProcessID_Mod=notblank
approverStatuses:approvedByID=$$USER.ID
approverStatuses:approvedByID_Mod=in
```

## Attività: mostrare tutte le attività con almeno un predecessore per più progetti

```
predecessorsMM:ID_Mod=notblank
predecessorsMM:projectID=FIELD:projectID
predecessorsMM:projectID_Mod=ne
```

## Attività: mostrare tutte le attività assegnate ad altri

Crea un rapporto di attività con i filtri desiderati, quindi passa alla scheda Filtro e fai clic su Passa a modalità testo. Aggiungi questo codice a un elemento già presente:

```
EXISTS:1:$$OBJCODE=ASSGN
EXISTS:1:taskID=FIELD:ID
EXISTS:1:assignedByID=$$USER.ID
```

Verranno visualizzate tutte le attività a cui l’utente connesso ha assegnato almeno uno degli assegnatari correnti. Se gli assegnatari sono stati assegnati da più persone, nella pagina di destinazione dell’attività per “Richiesto da” verrà visualizzato solo il nome della prima persona che ha assegnato qualcuno.

## Attività: visualizzare tutte le attività completate (In attesa di approvazione)

```
status=CPL:A
status_Mod=in
```


## Problema: mostrare tutti i problemi completati (In attesa di approvazione)

```
status=CPL:A
status_Mod=in
```


## Progetto: mostrare tutti i progetti completati (In attesa di approvazione)

```
status=CPL:A
status_Mod=in
```


## Nota: mostrare tutti i commenti in cui sono taggato

```
tags:userID=$$USER.ID
tags:userID_Mod=in
```


## Rapporto su parametri o campi personalizzati: mostrare i campi personalizzati non allegati a un modulo personalizzato (molto utile nelle operazioni di pulizia)

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=CTGYPA
EXISTS:A:parameterID=FIELD:ID
```
