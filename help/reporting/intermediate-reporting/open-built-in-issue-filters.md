---
title: Esplora i filtri dei problemi incorporati
description: Scopri come rivedere i filtri incorporati per i problemi, per capire come vengono generati e creare un filtro personalizzato per i problemi in Workfront.
activity: use
feature: Reports and Dashboards
thumbnail: 336819.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
last-substantial-update: '2025-07-25T00:00:00.000Z'
jira: KT-9085
exl-id: c1bdea98-e70a-4e93-935c-b8f7754afa21
doc-type: video
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: c6dd2ac5-f5bd-4e59-9101-25b156918623
subfeature_v2:
  - id: c68e30a0-f1f0-47be-a6a9-f26cd55c41a1
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-06T02:09:28.024Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 279
ht-degree: 53%

---

# Esplora i filtri dei problemi incorporati

In questo video:

* Controlla i filtri dei problemi incorporati per vedere come vengono generati
* Scoprire alcuni elementi di reporting utili sui problemi
* Scoprire come creare un filtro di problema personalizzato

>[!VIDEO](https://video.tv.adobe.com/v/336819/?quality=12&learn=on&enablevpops=0)


## Attività &quot;Comprendere i filtri dei problemi incorporati&quot;


### Attività: creare un rapporto sui problemi

Desidere vedere tutti i problemi che devono ancora essere risolti su tutti i progetti attivi di tua proprietà, inclusi i problemi con un oggetto di risoluzione. Crea un report sui problemi e denominalo &quot;Problemi non risolti nei miei progetti&quot;.

### Risposta

Ecco come dovrebbe essere il filtro:

![Immagine della schermata per la creazione di un filtro di problema](assets/opening-built-in-issue-filters-1.png)

Nel filtro integrato &quot;I miei problemi aperti&quot;, una delle regole di filtro escludeva eventuali problemi in cui era presente un oggetto di risoluzione. Il motivo è che non c&#39;è bisogno di preoccuparsi di questi problemi. Qualcuno ha già creato un progetto, un&#39;attività o un problema che li risolverà, quindi cosa c&#39;è da preoccuparsi? Ma non sono ancora risolti, e nel nostro esempio li includiamo per renderli facili da identificare e controllare come stanno facendo.

A questo scopo, devi aggiungere una colonna nella scheda della vista per &quot;Problema >> Oggetto risolutivo&quot;. Questo mostra il nome dell’oggetto di risoluzione, se ce n’è uno, che si tratti di progetto, attività o problema. Facendo clic sul nome si accede all’oggetto di risoluzione.

È possibile raggruppare l’elenco in base al nome del progetto.

Ecco come si presenterà il rapporto:

![Immagine di un rapporto sui problemi](assets/opening-built-in-issue-filters-2.png)
