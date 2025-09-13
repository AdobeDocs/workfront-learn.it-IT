---
title: Comprendere la modalità testo di base per i filtri
description: Scopri la modalità testo, la notazione Camel e alcune modalità testo di base che puoi utilizzare nei filtri dei rapporti in Workfront.
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
last-substantial-update: 2025-07-30T00:00:00Z
jira: KT-9086
exl-id: b3f16468-b720-468d-887a-b313fc32bd89
doc-type: video
source-git-commit: 9f5a6ba3ad6e4aa0af2b3bc18522777c646ae6f3
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 88%

---

# Informazioni sulla modalità testo di base per i filtri

>[!PREREQUISITES]
>
>* [Informazioni sugli elementi di reporting](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/reporting-elements.html?lang=it)
>* [Informazioni sui componenti di reporting](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/reporting-components.html?lang=it)
>* [Creare un filtro di base](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/intermediate-reporting/basic-text-mode-for-filters.html?lang=it)


>[!TIP]
>
>* Per comprendere meglio la modalità testo, ti consigliamo di guardare l’evento webinar registrato [Le domande agli esperti - Introduzione alla reportistica in modalità testo](https://experienceleague.adobe.com/it/docs/events/classics/reporting-and-dashboards/introduction-to-text-mode-reporting), della durata di un’ora.
>* Per ulteriori informazioni sulla modalità testo, ti consigliamo di guardare i tutorial sulla [Reportistica avanzata](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/advanced-reporting/welcome-to-advanced-reporting.html?lang=it) che hanno una durata totale di cinque ore e mezzo.
>* Fai clic qui per accedere a [[!UICONTROL API Explorer]](https://developer.adobe.com/workfront/api-explorer/)


In questo video scoprirai:

* Modalità testo
* Borsa Camel
* Alcuni _blocchi di codice in modalità testo_ che puoi utilizzare nei filtri dei report

>[!VIDEO](https://video.tv.adobe.com/v/336820/?quality=12&learn=on)

## Attività &quot;Comprendere la modalità testo di base per i filtri&quot;


### Attività: escludere le attività contrassegnate come “Ho terminato la mia parte”

La seguente modalità di testo escluderà le attività che un utente ha contrassegnato come “Ho terminato la mia parte”. È sufficiente creare un filtro delle attività, aggiungere le regole di filtro desiderate, quindi passare alla modalità testo e incollare il codice sottostante dopo qualsiasi modalità di testo visualizzata nel filtro.


>[!WARNING]
>
> Questa opzione non è destinata all’utilizzo nei filtri del calendario.

```
EXISTS:1:$$OBJCODE=ASSGN  
EXISTS:1:taskID=FIELD:ID  
EXISTS:1:status=DN  
EXISTS:1:status_Mod=notin  
EXISTS:1:assignedToID=$$USER.ID 
```

### Attività: mostrare tutte le attività in attesa della mia approvazione

```
approvalProcessID_Mod=notblank
currentUserApproversMM:ID=$$USER.ID
currentUserApproversMM:ID_Mod=in
currentUserApproversMM_Join=allowingnull
```

### Attività: mostrare tutte le attività approvate

Crea un rapporto di attività con i filtri desiderati, quindi passa alla scheda Filtro e fai clic su Passa a modalità testo. Aggiungi questo codice a un elemento già presente:

```
approvalProcessID_Mod=notblank
approverStatuses:approvedByID=$$USER.ID
approverStatuses:approvedByID_Mod=in
```

### Attività: mostrare tutte le attività con almeno un predecessore per più progetti

```
predecessorsMM:ID_Mod=notblank
predecessorsMM:projectID=FIELD:projectID
predecessorsMM:projectID_Mod=ne
```

### Attività: mostrare tutte le attività assegnate ad altri

Crea un rapporto di attività con i filtri desiderati, quindi passa alla scheda Filtro e fai clic su Passa a modalità testo. Aggiungi questo codice a un elemento già presente:

>[!WARNING]
> 
> Questa opzione non è destinata all’utilizzo nei filtri del calendario.

```
EXISTS:1:$$OBJCODE=ASSGN
EXISTS:1:taskID=FIELD:ID
EXISTS:1:assignedByID=$$USER.ID
```

Verranno visualizzate tutte le attività a cui l’utente connesso ha assegnato almeno uno degli assegnatari correnti. Se gli assegnatari sono stati assegnati da più persone, nella pagina di destinazione dell’attività per “Richiesto da” verrà visualizzato solo il nome della prima persona che ha assegnato qualcuno.

### Attività: visualizzare tutte le attività completate (In attesa di approvazione)

```
status=CPL:A
status_Mod=in
```


### Problema: mostrare tutti i problemi completati (In attesa di approvazione)

```
status=CPL:A
status_Mod=in
```


### Progetto: mostrare tutti i progetti completati (In attesa di approvazione)

```
status=CPL:A
status_Mod=in
```


### Nota: mostrare tutti i commenti in cui sono taggato

```
tags:userID=$$USER.ID
tags:userID_Mod=in
```


### Rapporto su parametri o campi personalizzati: mostrare i campi personalizzati non allegati a un modulo personalizzato (molto utile nelle operazioni di pulizia)

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=CTGYPA
EXISTS:A:parameterID=FIELD:ID
```
