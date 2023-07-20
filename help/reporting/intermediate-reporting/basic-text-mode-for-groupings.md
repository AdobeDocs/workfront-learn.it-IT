---
title: Comprendere la modalità testo di base per i raggruppamenti
description: Scopri che cosa sono la modalità testo, la notazione a cammello e alcune modalità testo "plug and play" di base che puoi utilizzare nei raggruppamenti in Workfront.
activity: use
feature: Text Mode Reporting
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-11369
exl-id: 5f45c64f-a22b-4983-91fd-9a1939f99fb1
doc-type: video
source-git-commit: 409147f9a62302d28e14b834981992a0421d4e4b
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# Comprendere la modalità testo di base per i raggruppamenti

>[!IMPORTANT]
>
>Prerequisiti:
>
>* Comprendere gli elementi di reporting
>* Comprendere i componenti di reporting
>* Creare un raggruppamento di base

>[!TIP]
>
>* Per comprendere meglio la modalità testo, consigliamo di guardare l’evento del webinar registrato [Ask the Expert - Introduzione al reporting in modalità testo](https://experienceleague.adobe.com/docs/workfront-events/events/reporting-and-dashboards/introduction-to-text-mode-reporting.html?lang=en), della durata di un&#39;ora.
>* Per ulteriori informazioni sulla modalità testo, si consiglia di guardare [Reporting avanzato](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/advanced-reporting/welcome-to-advanced-reporting.html?lang=en) esercitazioni, che insieme durano cinque ore e mezza.

Questo video illustra:

* Che cos’è la modalità testo
* Che cos’è Camel Case
* Alcune modalità di testo &quot;plug and play&quot; di base che è possibile utilizzare nei raggruppamenti

>[!VIDEO](https://video.tv.adobe.com/v/3410641/?quality=12&learn=on)

## Attività - Raggruppamento 4 padri

La modalità di testo seguente raggrupperà le attività in base a un massimo di quattro livelli di padri e lascerà vuoti i padri che non esistono.

```
textmode=true
group.0.name=Parents
group.0.valueexpression=CONCAT({parent}.{parent}.{parent}.{parent}.{name},IF(ISBLANK({parent}.{parent}.{parent}.{parent}.{name}),"",", "),{parent}.{parent}.{parent}.{name},IF(ISBLANK({parent}.{parent}.{parent}.{name}),"",", "),{parent}.{parent}.{name},IF(ISBLANK({parent}.{parent}.{name}),"",", "),IF(ISBLANK({parent}.{name}),"No parent",{parent}.{name}))
group.0.linkedname=parent
group.0.namekeyargkey.0=parent
group.0.namekeyargkey.1=name
group.0.valueformat=string
```

![Un&#39;immagine della schermata che mostra le attività del progetto raggruppate per 4 elementi principali](assets/4-parents-grouping.png)


## Attività - Raggruppamento percentuale di completamento

La modalità di testo seguente raggrupperà le attività in base alla loro percentuale di completamento. Le attività sono raggruppate in una delle seguenti categorie:

* 0%
* Da 1% a 25%
* Da 26% a 50%
* Da 51% a 75%
* Da 76% a 99%
* 100%

```
group.0.linkedname=direct
group.0.namekey=percentComplete
group.0.valueexpression=IF({percentComplete}<1,"0%",IF({percentComplete}<26,"1% to 25%",IF({percentComplete}<51,"26% to 50%",IF({percentComplete}<76,"51% to 75%",IF({percentComplete}<100,"76% to 99%",IF({percentComplete}=100,"100","***"))))))
group.0.valueformat=doubleAsString
textmode=true
```

![Immagine che mostra le attività di progetto raggruppate per percentuale di completamento](assets/percent-complete-grouping.png)

## Attività: statusEquatesWith, quindi status

La modalità di testo seguente raggrupperà le attività per statusEquatesWith, quindi per status.

```
group.0.enumclass=com.attask.common.constants.TaskStatusEnum
group.0.enumtype=TASK
group.0.linkedname=direct
group.0.name=State
group.0.type=enum
group.0.valuefield=statusEquatesWith
group.0.valueformat=val
group.1.enumclass=com.attask.common.constants.TaskStatusEnum
group.1.enumtype=TASK
group.1.linkedname=direct
group.1.namekey=status
group.1.type=enum
group.1.valuefield=status
group.1.valueformat=val
textmode=true
```

![Immagine schermata che mostra le attività del progetto raggruppate per statusEquatesWith](assets/status-equates-with.png)


## Approvazione bozza - Raggruppa per nome progetto

```
group.0.valueformat=HTML
group.0.valuefield=documentVersion:document:project:name
group.0.displayname=Project Name
```

![Immagine che mostra le approvazioni della bozza raggruppate per nome progetto](assets/proof-approvals-grouped-by-project-name.png)


## Approvazione bozza - Raggruppa per nome documento

```
group.0.displayname=Document Name
group.0.valuefield=documentVersion:document:name
group.0.valueformat=HTML
```

![Immagine che mostra le approvazioni della bozza raggruppate per nome progetto](assets/proof-approvals-grouped-by-doc-name.png)

