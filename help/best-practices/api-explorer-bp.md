---
title: Best practice - API Explorer
description: Esplora le best practice consigliate dagli esperti di Adobe Workfront in merito all’impostazione, alla gestione e all’utilizzo dell’API Explorer di Workfront.
feature: Workfront API
role: Admin, Leader, User
level: Beginner
jira: KT-10902
exl-id: 0f3fc5ba-d01a-4337-829f-def0830ddf81
TQID: https://experienceleague.adobe.com/RUQeNzEb0eg9DKSKepugb0HD4O2ODql-0mWBn-ptgxk
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2:
  - id: bb1dd007-4a34-496d-9d3b-2278fdaadac1
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: f8a45b24-4be7-4f1b-909b-60d06b483a20
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
source-git-commit: 36674ed53c8645f556862bb2d99f3bfd6c993c1e
workflow-type: tm+mt
source-wordcount: 410
ht-degree: 75%

---

# Best practice - API Explorer

## Che cos’è una “best practice” di Adobe Workfront?

Le best practice sono linee guida che rappresentano una linea d’azione efficace ed efficiente; sono facilmente adottabili da te e dagli utenti della tua azienda; e possono essere replicate con successo in tutta l’organizzazione.

Mentre esamini questi consigli, tieni presente che alcune best practice di Workfront sono universali mentre altre potrebbero essere più specifiche per un dato argomento. Utilizza queste best practice come una base comune per le impostazioni e l’utilizzo del sistema Workfront.

## Esplorazione di questa pagina

Mentre scorri questa pagina, troverai innanzitutto un elenco di alto livello di tutte le best practice per questo argomento. Questo ti consente di rivedere i consigli senza entrare nei dettagli del “perché”.

L’area &quot;Perché queste best practice?&quot;, che si trova dopo l’elenco di alto livello, fornisce maggiori dettagli su alcune delle best practice e sul perché vengono considerate un processo, uno strumento, ecc., è consigliabile implementarle con l’istanza di Workfront.

</br>
</br>

## Best practice per API Explorer

* Stabilisci una convenzione di denominazione per i campi personalizzati utilizzati con integrazioni da sistemi di terze parti.

* Monitora tutti i campi personalizzati utilizzati nelle integrazioni tramite un progetto Workfront.

* Aggiungi il campo ID oggetto ai report utilizzati dall’amministratore di sistema.

</br>
</br>

## Perché queste sono best practice?

**Best practice**

Stabilisci una convenzione di denominazione per i campi personalizzati utilizzati con integrazioni da sistemi di terze parti.

**Ecco perché**

Assicurati che tutti coloro che creano moduli personalizzati siano a conoscenza della convenzione di denominazione, in modo da non utilizzare accidentalmente un campo riservato a un’integrazione. A seconda delle integrazioni e dei flussi di lavoro, l’utilizzo dello stesso campo in più modi potrebbe comportare la modifica o la sovrascrittura dei dati e la generazione di dati errati nei rapporti.

</br>
</br>


**Best practice**

Monitora tutti i campi personalizzati utilizzati nelle integrazioni tramite un progetto Workfront.

**Ecco perché**

Un progetto rappresenta il punto ideale per registrare i nomi di campo personalizzati, l’integrazione con cui vengono utilizzati, ecc. Questo ti aiuterà a evitare la creazione di campi personalizzati ridondanti o l’utilizzo dello stesso campo personalizzato con più integrazioni.

</br>
</br>


**Best practice**

Aggiungi il campo ID oggetto ai report utilizzati dall’amministratore di sistema.

**Ecco perché**

Quando si utilizzano API o altre integrazioni, gli amministratori di sistema spesso devono fare riferimento agli oggetti in Workfront per il numero ID. Includi il campo ID nelle visualizzazioni per gli oggetti su cui lavori (progetti, attività, problemi, modelli, moduli personalizzati, ecc.) per semplificare l&#39;accesso e la copia.
