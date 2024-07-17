---
title: Best practice - API Explorer
description: Esplora le best practice consigliate dagli esperti di Adobe Workfront in merito all’impostazione, alla gestione e all’utilizzo dell’API Explorer di Workfront.
feature: Workfront API
role: Admin, Leader, User
level: Beginner
jira: KT-10902
exl-id: 0f3fc5ba-d01a-4337-829f-def0830ddf81
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 100%

---

# Best practice - API Explorer

## Che cos’è una “best practice” di Adobe Workfront?

Le best practice sono linee guida che rappresentano una linea d’azione efficace ed efficiente; sono facilmente adottabili da te e dagli utenti della tua azienda; e possono essere replicate con successo in tutta l’organizzazione.

Mentre esamini questi consigli, tieni presente che alcune best practice di Workfront sono universali mentre altre potrebbero essere più specifiche per un dato argomento. Utilizza queste best practice come una base comune per le impostazioni e l’utilizzo del sistema Workfront.

## Esplorazione di questa pagina

Mentre scorri questa pagina, troverai innanzitutto un elenco di alto livello di tutte le best practice per questo argomento. Questo ti consente di rivedere i consigli senza entrare nei dettagli del “perché”.

La sezione “Perché queste sono best practice?”, che si trova dopo l’elenco di alto livello, fornisce maggiori dettagli su alcune delle best practice e sul motivo per cui sono considerate un processo, uno strumento ecc. da implementare con la tua istanza di Workfront.

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

Quando si utilizzano API o altre integrazioni, gli amministratori di sistema spesso devono fare riferimento agli oggetti in Workfront per il numero ID. Includi il campo ID nelle visualizzazioni per gli oggetti su cui lavori (progetti, attività, problemi, modelli, moduli personalizzati, ecc.) per semplificare l’accesso e la copia.
