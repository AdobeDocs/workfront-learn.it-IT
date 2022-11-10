---
title: Procedura dettagliata sull’aggregazione avanzata
description: Scopri come chiamare un servizio Web per restituire i dettagli su più paesi e identificare la popolazione, raggruppata per sottoregione, il tutto in [!DNL Adobe Workfront Fusion].
activity: use
doc-type: feature video
team: Technical Marketing
kt: Jira ticket
exl-id: c79250d0-7341-4a25-83dc-de99ce5c6dc4
source-git-commit: ca56810c9eab36175a6280e319b5fd2aba90b2f2
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---

# Procedura dettagliata sull’aggregazione avanzata

## Panoramica

Chiamare un servizio Web per restituire i dettagli relativi a più paesi e identificare la popolazione totale di tutti i paesi, raggruppati per sottoregione.

![Immagine dello scenario di fusione](assets/iteration-and-aggregation-3.png)

## Procedura dettagliata sull’aggregazione avanzata

Workfront consiglia di guardare il video dettagliato sull&#39;esercizio prima di cercare di ricreare l&#39;esercizio nel proprio ambiente.

>[!VIDEO](https://video.tv.adobe.com/v/335281/?quality=12)

## URL di esercizio

* `https://restcountries.com/v2/lang/es`
* `https://restcountries.com/v2/name/{country name}`

>[!TIP]
>
>Per istruzioni dettagliate su come completare la procedura dettagliata, consulta [Procedura dettagliata sull’aggregazione avanzata](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/advanced-aggregation.html?lang=en) esercizio fisico.

## Rafforzamento del principio di aggregazione

Ogni volta che un modulo genera più bundle, ogni modulo successivo eseguirà ogni bundle.

Per evitare questo problema, aggiungi un aggregatore dopo un modulo che potrebbe generare più bundle.

Vedrai un’ombra intorno a qualsiasi segmento nello scenario da un **iteratore iniziale** al **aggregatore finale**. Questo consente di individuare facilmente questi segmenti nello scenario Workfront Fusion.

## Il tuo turno

Questo esercizio si basa su ciò che hai appreso nella procedura dettagliata, ma la soluzione non viene fornita.

Crea un nuovo scenario per sommare tutte le ore di accesso alle attività nei progetti nel portfolio marketing. Inviare quindi un messaggio e-mail con la dicitura &quot;Il team del progetto {Nome progetto} ha registrato {ore sommate} del totale di {ore pianificate} ore pianificate, inserendo {percentuale} del piano.&quot;

**Sfida:** Vedi se puoi fare la stessa cosa, ma solo per ore registrate quest&#39;anno.

## Vuoi saperne di più? Si consiglia quanto segue:

[Documentazione di Workfront Fusion](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
