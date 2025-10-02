---
title: Comprendere la modalità testo di base per i raggruppamenti
description: Scopri la modalità testo, la notazione Camel e alcune modalità testo di base che puoi utilizzare nei raggruppamenti di rapporti in Workfront.
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
last-substantial-update: 2025-08-12T00:00:00Z
jira: KT-11369
exl-id: 5f45c64f-a22b-4983-91fd-9a1939f99fb1
doc-type: video
source-git-commit: bbdf99c6bc1be714077fd94fc3f8325394de36b3
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 85%

---

# Comprendere la modalità testo di base per i raggruppamenti

>[!PREREQUISITES]
>
>* [Informazioni sugli elementi di reporting](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/reporting-elements.html?lang=it)
>* [Informazioni sui componenti di reporting](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/reporting-components.html?lang=it)
>* [Creare un raggruppamento di base](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/create-a-basic-grouping.html?lang=it)


>[!TIP]
>
>* Per comprendere meglio la modalità testo, ti consigliamo di guardare l’evento webinar registrato [Le domande agli esperti - Introduzione alla reportistica in modalità testo](https://experienceleague.adobe.com/en/docs/events/classics/reporting-and-dashboards/introduction-to-text-mode-reporting), della durata di un’ora.
>* Per ulteriori informazioni sulla modalità testo, ti consigliamo di guardare i tutorial sulla [Reportistica avanzata](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/advanced-reporting/welcome-to-advanced-reporting.html?lang=it) che hanno una durata totale di cinque ore e mezzo.
>* Fai clic qui per accedere a [[!UICONTROL API Explorer]](https://developer.adobe.com/workfront/api-explorer/)

In questo video scoprirai:

* Che cos’è la modalità testo
* Che cos’è la notazione a cammello
* Alcuni _blocchi di codice in modalità testo_ che puoi utilizzare nei raggruppamenti di rapporti

>[!VIDEO] (https://video.tv.adobe.com/v/3470787/?quality=12&learn=on&enablevpops=0&captions=ita

## Attività &quot;Comprendere la modalità testo di base per i raggruppamenti&quot;

### Attività: raggruppamento di 4 elementi principali

La seguente modalità di testo raggrupperà le attività in base a un massimo di quattro livelli di elementi principali e lascerà vuoti gli elementi principali che non esistono.

```
textmode=true
group.0.name=Parents
group.0.valueexpression=CONCAT({parent}.{parent}.{parent}.{parent}.{name},IF(ISBLANK({parent}.{parent}.{parent}.{parent}.{name}),"",", "),{parent}.{parent}.{parent}.{name},IF(ISBLANK({parent}.{parent}.{parent}.{name}),"",", "),{parent}.{parent}.{name},IF(ISBLANK({parent}.{parent}.{name}),"",", "),IF(ISBLANK({parent}.{name}),"No parent",{parent}.{name}))
group.0.linkedname=parent
group.0.namekeyargkey.0=parent
group.0.namekeyargkey.1=name
group.0.valueformat=string
```

![Immagine di una schermata che mostra le attività del progetto raggruppate per 4 elementi principali](assets/4-parents-grouping.png)


### Attività: raggruppamento per percentuale di completamento

La seguente modalità di testo raggrupperà le attività in base alla percentuale di completamento. Quando saranno raggruppate, le attività rientreranno in una delle seguenti categorie:

* 0%
* Dall’1% al 25%
* Dal 26% al 50%
* Dal 51% al 75%
* Dal 76% al 99%
* 100%

```
group.0.linkedname=direct
group.0.namekey=percentComplete
group.0.valueexpression=IF({percentComplete}<1,"0%",IF({percentComplete}<26,"1% to 25%",IF({percentComplete}<51,"26% to 50%",IF({percentComplete}<76,"51% to 75%",IF({percentComplete}<100,"76% to 99%",IF({percentComplete}=100,"100","***"))))))
group.0.valueformat=doubleAsString
textmode=true
```

![Immagine della schermata che mostra le attività del progetto raggruppate per percentuale di completamento](assets/percent-complete-grouping.png)

### Attività: statusEquatesWith, quindi per stato

La seguente modalità di testo raggrupperà le attività per statusEquatesWith, quindi per stato.

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

![Immagine dello schermo che mostra le attività del progetto raggruppate per statusEquatesWith](assets/status-equates-with.png)


### Approvazione bozze: raggruppa per nome del progetto

```
group.0.valueformat=HTML
group.0.valuefield=documentVersion:document:project:name
group.0.displayname=Project Name
```

![Immagine della schermata che mostra le approvazioni di bozze raggruppate per nome del progetto](assets/proof-approvals-grouped-by-project-name.png)


### Approvazione bozze: raggruppa per nome del documento

```
group.0.displayname=Document Name
group.0.valuefield=documentVersion:document:name
group.0.valueformat=HTML
```

![Immagine della schermata che mostra le approvazioni di bozze raggruppate per nome del progetto](assets/proof-approvals-grouped-by-doc-name.png)

