---
title: Comprendere i filtri dei problemi incorporati
description: Scopri come rivedere i filtri incorporati per i problemi, per capire come vengono generati e creare un filtro personalizzato per i problemi in Workfront.
activity: use
feature: Reports and Dashboards
thumbnail: 336819.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
last-substantial-update: 2025-07-25T00:00:00Z
jira: KT-9085
exl-id: c1bdea98-e70a-4e93-935c-b8f7754afa21
doc-type: video
source-git-commit: bbdf99c6bc1be714077fd94fc3f8325394de36b3
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 56%

---

# Comprendere i filtri dei problemi incorporati

In questo video:

* Controlla i filtri dei problemi incorporati per vedere come vengono generati
* Scoprire alcuni elementi di reporting utili sui problemi
* Scoprire come creare un filtro di problema personalizzato

>[!VIDEO] (https://video.tv.adobe.com/v/3412679/?quality=12&learn=on&enablevpops=0&captions=ita


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
