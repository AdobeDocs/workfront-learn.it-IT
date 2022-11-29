---
title: Procedura dettagliata degli archivi dati
description: Scopri come utilizzare un archivio dati per sincronizzare i nomi aziendali tra un elenco di aziende e Workfront utilizzando [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 9055
exl-id: e96fd109-2463-4702-b1bf-b42a6dcd7fc4
source-git-commit: 96f963bf5a44eac234cbf9215f19f6dddbe23143
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---

# Procedura dettagliata degli archivi dati

## Panoramica

In questo esercizio utilizziamo un archivio dati per sincronizzare i nomi aziendali tra un elenco di aziende e Workfront.

Questa è una parte di una sincronizzazione unidirezionale delle aziende in Workfront e in altri sistemi. Per il momento, si sincronizza solo tra un file CSV e Workfront. Tuttavia manterrà anche una tabella in un archivio dati che terrà traccia dell’ID Workfront (WFID) e dell’ID società nel file CSV (CID) per ogni azienda. Questo ci permetterà di rendere questa sincronizzazione bidirezionale in un certo momento del futuro.

![Immagine di uno scenario di fusione](assets/data-structures-and-data-stores-2.png)

## Procedura dettagliata degli archivi dati

Workfront consiglia di guardare il video dettagliato sull&#39;esercizio prima di cercare di ricreare l&#39;esercizio nel proprio ambiente.

>[!VIDEO](https://video.tv.adobe.com/v/335296/?quality=12)

>[!TIP]
>
>Per istruzioni dettagliate su come completare la procedura dettagliata, consulta [Procedura dettagliata degli archivi dati](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/data-stores.html?lang=en) esercizio fisico.


## Nota finale

Ora che hai finito di imparare le strutture di dati e gli archivi di dati, potresti chiederti: &quot;Quando dovrei usarle?&quot;

Le strutture di dati sono comunemente utilizzate per serializzare o analizzare formati di dati come JSON, XML, CSV e altri. Le strutture dati consentono di controllare la struttura dei dati e persino di convalidarli. Il motivo più comune per cui utilizzi una struttura dati è la creazione di dati validi da inviare a un’API che richiede JSON o XML. In questi casi, utilizza l’app JSON o XML insieme alla struttura dei dati per verificare che i dati siano nel formato corretto.

Gli archivi dati devono essere utilizzati solo per memorizzare dati persistenti a cui è necessario accedere da più di un’esecuzione di scenario. Ad esempio, puoi memorizzare i metadati sull’ultimo record elaborato per casi d’uso avanzati che richiedono un controllo preciso dell’elaborazione.

Gli archivi dati non sono progettati per essere utilizzati come data warehouse o registrazione. Gli archivi dati non sono accessibili al di fuori di Workfront Fusion e la maggior parte delle interazioni con gli archivi di dati avviene attraverso uno scenario Workfront Fusion. Di conseguenza, non è possibile collegare un archivio dati a uno strumento di analisi o di reporting previsto per i casi di utilizzo di data warehouse e logging. Il ruolo di Workfront Fusion in casi d&#39;uso come questi sarebbe quello di compilare un sistema appropriato per l&#39;organizzazione e la memorizzazione dei dati (ad esempio SQL, MariaDB).

## Vuoi saperne di più? Si consiglia quanto segue:

[Documentazione di Workfront Fusion](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
