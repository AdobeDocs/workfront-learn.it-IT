---
title: Procedura dettagliata sugli archivi di dati
description: Scopri come utilizzare un archivio dati per sincronizzare i nomi delle società tra un elenco di aziende e Workfront utilizzando  [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9055
exl-id: e96fd109-2463-4702-b1bf-b42a6dcd7fc4
recommendations: noDisplay,noCatalog
doc-type: video
source-git-commit: a4e61514567ac8c2b4ad5c9ecacb87bd83947731
workflow-type: ht
source-wordcount: '393'
ht-degree: 100%

---

# Procedura dettagliata sugli archivi di dati

In questo esercizio verrà utilizzato un archivio dati per sincronizzare i nomi delle aziende tra un elenco di aziende e Workfront.

Questa è una parte di una sincronizzazione unidirezionale delle aziende in Workfront e in altri sistemi. Per ora, la sincronizzazione verrà eseguita soltanto tra un file CSV e Workfront. Ma manterrà anche una tabella in un archivio dati che terrà traccia dell’ID Workfront (WFID) e dell’ID azienda nel file CSV (CID) per ciascuna azienda. Ciò consentirà una sincronizzazione bidirezionale in futuro.

![Immagine di uno scenario Fusion](assets/data-structures-and-data-stores-2.png)

## Procedura dettagliata sugli archivi di dati

Workfront consiglia di guardare il video della procedura dettagliata relativa all’esercizio, prima di provare a ricrearlo nel proprio ambiente.

>[!VIDEO](https://video.tv.adobe.com/v/335296/?quality=12&learn=on)



## Nota finale

Ora che hai finito di imparare le strutture di dati e gli archivi di dati, potresti chiederti quando dovresti usarli.

Le strutture dati vengono comunemente utilizzate per serializzare o analizzare formati di dati come JSON, XML, CSV e altri. Le strutture dati ti permettono di controllare la struttura dei tuoi dati e persino di convalidarli. Il motivo più comune per cui utilizzi una struttura dati è quello di creare dati validi da inviare a un’API che prevede JSON o XML. In questi casi, puoi utilizzare l’app JSON o XML insieme alla struttura dati per verificare che i dati siano nel formato corretto.

Gli archivi dati devono essere utilizzati solo per archiviare dati persistenti a cui è necessario accedere tramite l’esecuzione di più scenari. Ad esempio, puoi memorizzare metadati sull’ultimo record elaborato per casi d’uso avanzati che richiedono un controllo preciso sull’elaborazione.

Gli archivi dati non sono progettati per essere utilizzati come data warehouse o registrazione. Gli archivi dati non sono accessibili al di fuori di Workfront Fusion e la maggior parte delle interazioni con gli archivi dati avviene tramite uno scenario Workfront Fusion. Di conseguenza, non è possibile connettere un archivio dati a uno strumento di analisi o di reporting come previsto per i casi d’uso di data warehouse e registrazione. In casi di utilizzo di questo tipo, Workfront Fusion ha il compito di popolare un sistema appropriato per l’organizzazione e l’archiviazione dei dati (ad esempio SQL, MariaDB).

## Desideri ulteriori informazioni? Consigliamo quanto segue:

[Documentazione di Workfront Fusion](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=it)
