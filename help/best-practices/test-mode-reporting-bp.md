---
title: Best practice - Reporting in modalità testo
description: Esplora le best practice consigliate dagli esperti di Adobe Workfront in merito all’impostazione, alla gestione e all’utilizzo della modalità di reporting in formato testo Workfront.
feature: Reports and Dashboards
role: Admin, Leader, User
level: Beginner
jira: KT-10928
exl-id: c624545c-ba42-4cc3-aafe-8be15baadb75
TQID: https://experienceleague.adobe.com/k8DYutzVcGrJc7p0x74B2iQ3nkiohWeQu1egOWZ34AI
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bdid: f8a45b24-4be7-4f1b-909b-60d06b483a20
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: 36674ed53c8645f556862bb2d99f3bfd6c993c1e
workflow-type: tm+mt
source-wordcount: 418
ht-degree: 90%

---

# Best practice - Reporting in modalità testo

## Che cos’è una “best practice” di Adobe Workfront?

Le best practice sono linee guida che rappresentano una linea d’azione efficace ed efficiente; sono facilmente adottabili da te e dagli utenti della tua azienda; e possono essere replicate con successo in tutta l’organizzazione.

Mentre esamini questi consigli, tieni presente che alcune best practice di Workfront sono universali mentre altre potrebbero essere più specifiche per un dato argomento. Utilizza queste best practice come una base comune per le impostazioni e l’utilizzo del sistema Workfront.

## Esplorazione di questa pagina

Mentre scorri questa pagina, troverai innanzitutto un elenco di alto livello di tutte le best practice per questo argomento. Questo ti consente di rivedere i consigli senza entrare nei dettagli del “perché”.

L’area &quot;Perché queste best practice?&quot;, che si trova dopo l’elenco di alto livello, fornisce maggiori dettagli su alcune delle best practice e sul perché vengono considerate un processo, uno strumento, ecc., è consigliabile implementarle con l’istanza di Workfront.

</br>
</br>

## Best practice per il reporting in modalità testo

* Se possibile, utilizza espressioni di valore in modalità testo anziché campi personalizzati calcolati nelle colonne dei rapporti elenco.

* Inserisci i calcoli utilizzati in un calcolo in modalità testo nella descrizione del report.

</br>
</br>

## Perché queste sono best practice?

**Best practice**

Se possibile, utilizza espressioni di valore in modalità testo anziché campi personalizzati calcolati nelle colonne dei rapporti elenco.



**Ecco perché**

Le espressioni dei valori in modalità testo vengono calcolate al momento dell’esecuzione del report e ricalcolate ogni volta che il report viene aggiornato. Ciò significa che avrai sempre dati aggiornati e rapporti accurati.



I campi personalizzati calcolati (utilizzati sui moduli personalizzati) non si aggiornano automaticamente quando i dati vengono visualizzati in Workfront. Vengono invece visualizzati i risultati del calcolo più recente memorizzato in Workfront. Ciò significa che tali valori potrebbero essere &quot;obsoleti&quot; o non aggiornati in un dato momento. I campi personalizzati calcolati devono essere aggiornati manualmente, ricalcolando l’espressione o modificando e salvando l’oggetto che contiene il campo calcolato. Questo può richiedere molto tempo e può essere facile dimenticarsi di farlo.


</br>
</br>

**Best practice**

Inserisci i calcoli utilizzati in un calcolo in modalità testo nella descrizione del report.



**Ecco perché**

L’inclusione di calcoli in modalità testo nella descrizione del rapporto aiuta gli altri a capire in che modo è stato creato il calcolo e che tipo di informazioni dovrebbe essere visualizzato. Inoltre, ricorda agli amministratori di sistema come è stato creato il rapporto, nel caso in cui siano necessari aggiornamenti in futuro.
