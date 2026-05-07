---
title: Procedura dettagliata per l’aggregazione avanzata
description: Scopri come chiamare un servizio web per restituire dettagli su più paesi e identificare la popolazione, raggruppata per sottoregione, il tutto in [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9040
exl-id: c79250d0-7341-4a25-83dc-de99ce5c6dc4
recommendations: noDisplay,catalog
doc-type: video
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: c3a155b4-a54b-4a82-a3d2-c8f0f971673e
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-06T16:33:27.197Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 258
ht-degree: 91%

---

# Procedura dettagliata per l’aggregazione avanzata

Chiama un servizio web per restituire dettagli su più paesi e identificare la popolazione totale di tutti i paesi, raggruppati per sottoregione.

![Immagine dello scenario Fusion](assets/iteration-and-aggregation-3.png)

## Procedura dettagliata per l’aggregazione avanzata

Workfront consiglia di guardare il video della procedura dettagliata relativa all’esercizio, prima di provare a ricrearlo nel proprio ambiente.

>[!VIDEO](https://video.tv.adobe.com/v/335281/?quality=12&learn=on&enablevpops=1)

## URL di esercizio

* `https://restcountries.com/v2/lang/es`
* `https://restcountries.com/v2/name/{country name}`



## Rafforzamento del principio di aggregazione

Ogni volta che un modulo produce più bundle, ogni modulo successivo eseguirà ogni bundle.

Per evitare questo problema, aggiungi un aggregatore dopo un modulo che potrebbe produrre più bundle.

Un’ombra evidenzia eventuali segmenti nello scenario da un **beginning-initiator** a un **end-aggregator**. In questo modo è più facile individuare tali segmenti nello scenario di Workfront Fusion.

## Tocca a te

>[!NOTE]
>
>Gli esercizi pratici e le sfide sono facoltativi e non necessari per completare la formazione su Fusion.

Questa esercitazione si basa su quanto appreso nella procedura dettagliata, ma è priva di soluzione.

Crea un nuovo scenario per sommare tutte le ore registrate per le attività nei progetti nel portfolio marketing. Inviare quindi un&#39;e-mail con la seguente dicitura: &quot;Il team di progetto {Project Name} ha registrato {summed hours} delle {planned hours} ore pianificate totali, arrivando a {percentage} del piano.&quot;

**Sfida:** prova a ripetere questo esercizio, ma solo per le ore registrate quest’anno.

## Desideri ulteriori informazioni? Consigliamo quanto segue:

[Documentazione di Workfront Fusion](https://experienceleague.adobe.com/it/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)
