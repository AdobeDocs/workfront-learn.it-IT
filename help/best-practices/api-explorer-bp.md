---
title: Procedure consigliate - Esplora API
description: Scopri le best practice consigliate dagli esperti Adobe Workfront sull’impostazione, la gestione e l’utilizzo di Workfront API Explorer.
feature: Workfront API
role: Admin, Leader, User
level: Beginner
kt: 10902
exl-id: 0f3fc5ba-d01a-4337-829f-def0830ddf81
source-git-commit: 444f059d3cc26d8e3074a7145bc5419407c786cf
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# Procedure consigliate - Esplora API

## Qual è una &quot;best practice&quot; di Adobe Workfront?

Le migliori pratiche sono linee guida che rappresentano un&#39;azione efficace ed efficiente; sono facilmente adottati da te e dagli utenti della tua azienda; e può essere replicato correttamente in tutta l’organizzazione.

Quando si esaminano queste raccomandazioni, tenere presente che alcune best practice di Workfront sono universali, mentre altre potrebbero essere più specifiche per l’argomento. Utilizza queste best practice come framework per guidare le impostazioni e l’utilizzo del sistema Workfront.

## Navigazione in questa pagina

Scorrendo questa pagina, troverai innanzitutto un elenco di alto livello contenente tutte le best practice per l’argomento. Questo ti consente di rivedere le raccomandazioni senza immergerti nei dettagli del &quot;perché&quot;.

Perché queste best practice? area, disponibile dopo l’elenco di alto livello, fornisce maggiori dettagli su alcune delle best practice e sui motivi per cui vengono considerate un processo, uno strumento, ecc., dovresti considerare l’implementazione con la tua istanza Workfront.

</br>
</br>

## Best practice di API Explorer

* Stabilisci una convenzione di denominazione per i campi personalizzati utilizzati con integrazioni da sistemi di terze parti.

* Tieni traccia di tutti i campi personalizzati utilizzati nelle integrazioni utilizzando un progetto Workfront.

* Aggiungere il campo ID oggetto ai rapporti utilizzati dall&#39;amministratore di sistema.

</br>
</br>

## Perché queste best practice sono?

**Best practice**

Stabilisci una convenzione di denominazione per i campi personalizzati utilizzati con integrazioni da sistemi di terze parti.

**Ecco perché**

Verificare che tutti gli utenti che creano moduli personalizzati siano a conoscenza della convenzione di denominazione, in modo che non utilizzino accidentalmente un campo riservato a un’integrazione. A seconda delle integrazioni e dei flussi di lavoro, l’utilizzo dello stesso campo in più modi potrebbe causare la modifica o la sovrascrittura dei dati e generare la presenza di dati errati nei rapporti.

</br>
</br>


**Best practice**

Tieni traccia di tutti i campi personalizzati utilizzati nelle integrazioni utilizzando un progetto Workfront.

**Ecco perché**

Un progetto rappresenta la posizione ideale per registrare i nomi di campi personalizzati, l’integrazione con cui vengono utilizzati, ecc. Questo ti aiuterà a evitare la creazione di campi personalizzati ridondanti o l’utilizzo dello stesso campo personalizzato con più integrazioni.

</br>
</br>


**Best practice**

Aggiungere il campo ID oggetto ai rapporti utilizzati dall&#39;amministratore di sistema.

**Ecco perché**

Gli amministratori di sistema spesso devono fare riferimento agli oggetti in Workfront in base al loro numero ID quando utilizzano API o altre integrazioni. Includi il campo ID nelle visualizzazioni degli oggetti su cui lavori (progetti, attività, problemi, modelli, moduli personalizzati, ecc.) per semplificare l’accesso e la copia.
