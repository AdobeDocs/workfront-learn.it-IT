---
title: Procedura dettagliata sugli archivi dati
description: Scopri come utilizzare un archivio dati per sincronizzare i nomi delle società tra un elenco di società e Workfront utilizzando [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 9055
exl-id: e96fd109-2463-4702-b1bf-b42a6dcd7fc4
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---

# Procedura dettagliata sugli archivi dati

## Panoramica

In questo esercizio utilizzeremo un archivio dati per sincronizzare i nomi delle società tra un elenco di società e Workfront.

Questa è una parte di una sincronizzazione unidirezionale delle aziende in Workfront e in altri sistemi. Per il momento, verrà sincronizzato solo tra un file CSV e Workfront. ma conserva anche una tabella in un archivio dati che tiene traccia del Workfront ID (WFID) e dell’ID azienda nel file CSV (CID) per ogni azienda. Questo ci permetterà di renderlo una sincronizzazione bidirezionale in futuro.

![Immagine di uno scenario Fusion](assets/data-structures-and-data-stores-2.png)

## Procedura dettagliata sugli archivi dati

Workfront consiglia di guardare il video con procedura dettagliata dell’esercizio prima di tentare di ricrearlo nel tuo ambiente.

>[!VIDEO](https://video.tv.adobe.com/v/335296/?quality=12)

>[!TIP]
>
>Per istruzioni dettagliate sul completamento della procedura dettagliata, vedere [Procedura dettagliata sugli archivi dati](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/data-stores.html?lang=en) esercizio fisico.


## Nota finale

Ora che hai finito di imparare le strutture di dati e gli archivi di dati, potresti chiederti: &quot;Quando dovrei usarli?&quot;

Le strutture di dati vengono utilizzate in genere per la serializzazione o l’analisi dei formati di dati come JSON, XML, CSV e altri. Le strutture di dati consentono di controllare la struttura dei dati e persino convalidarli. Il motivo più comune per utilizzare una struttura di dati è quello di creare dati validi da inviare a un’API che richiede JSON o XML. In questi casi, utilizza l’app JSON o XML insieme alla struttura dati per assicurarti che i dati siano nel formato corretto.

Gli archivi dati devono essere utilizzati solo per memorizzare dati persistenti a cui è necessario accedere da più di uno scenario. Ad esempio, puoi memorizzare metadati sull’ultimo record elaborato per casi d’uso avanzati che richiedono un controllo preciso sull’elaborazione.

Gli archivi dati non sono progettati per essere utilizzati come data warehouse o registrazione. Gli archivi dati non sono accessibili al di fuori di Workfront Fusion e la maggior parte delle interazioni con gli archivi dati avviene tramite uno scenario Workfront Fusion. Di conseguenza, non è possibile collegare un archivio dati a uno strumento di analisi o reporting che sarebbe previsto per i casi di utilizzo di data warehouse e registrazione. In casi di utilizzo di questo tipo, il ruolo di Workfront Fusion consiste nel popolare un sistema appropriato per l’organizzazione e l’archiviazione dei dati (ad esempio SQL, MariaDB).

## Vuoi saperne di più? Consigliamo quanto segue:

[Documentazione di Workfront Fusion](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
