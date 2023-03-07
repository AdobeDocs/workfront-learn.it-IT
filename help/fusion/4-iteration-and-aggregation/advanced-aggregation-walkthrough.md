---
title: Procedura dettagliata di aggregazione avanzata
description: Scopri come chiamare un servizio web per restituire dettagli su più paesi e identificare la popolazione, raggruppata per sottoregione, il tutto in [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 9040
exl-id: c79250d0-7341-4a25-83dc-de99ce5c6dc4
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 0%

---

# Procedura dettagliata di aggregazione avanzata

## Panoramica

Chiama un servizio web per restituire dettagli su più paesi e identificare la popolazione totale di tutti i paesi, raggruppati per sottoregione.

![Immagine dello scenario Fusion](assets/iteration-and-aggregation-3.png)

## Procedura dettagliata di aggregazione avanzata

Workfront consiglia di guardare il video con procedura dettagliata dell’esercizio prima di tentare di ricrearlo nel tuo ambiente.

>[!VIDEO](https://video.tv.adobe.com/v/335281/?quality=12)

## URL di esercizio

* `https://restcountries.com/v2/lang/es`
* `https://restcountries.com/v2/name/{country name}`

>[!TIP]
>
>Per istruzioni dettagliate sul completamento della procedura dettagliata, vedere [Procedura dettagliata di aggregazione avanzata](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/advanced-aggregation.html?lang=en) esercizio fisico.

## Rafforzamento del principio di aggregazione

Ogni volta che un modulo produce più bundle, ogni modulo successivo eseguirà ogni bundle.

Per evitare questo problema, aggiungi un aggregatore dopo un modulo che potenzialmente produce più bundle.

Vedrai un&#39;ombra che circonda qualsiasi segmento nello scenario da un **initiator** al **end-aggregator**. In questo modo è facile individuare questi segmenti nello scenario di Workfront Fusion.

## Tocca a te

>[!NOTE]
>
>Gli esercizi pratici e le sfide sono facoltativi e non sono necessari per completare la formazione su Fusion.

Questo esercizio di esercitazione si basa su quanto appreso nella procedura dettagliata, ma la soluzione non viene fornita.

Crea un nuovo scenario per sommare tutte le ore collegate alle attività nei progetti nel portfolio marketing. Quindi invia un’e-mail con la scritta &quot;Il team di progetto {Project Name} ha registrato {sum hours} delle {planned hours} ore totali pianificate, portando il tuo numero a {percentage} del piano.&quot;

**Sfida:** Vedi se puoi fare la stessa cosa, ma solo per le ore registrate quest&#39;anno.

## Vuoi saperne di più? Consigliamo quanto segue:

[Documentazione di Workfront Fusion](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
