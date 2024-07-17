---
title: Best practice - Reporting in modalità testo
description: Esplora le best practice consigliate dagli esperti di Adobe Workfront in merito all’impostazione, alla gestione e all’utilizzo della modalità di reporting in formato testo Workfront.
feature: Reports and Dashboards
role: Admin, Leader, User
level: Beginner
jira: KT-10928
exl-id: c624545c-ba42-4cc3-aafe-8be15baadb75
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 100%

---

# Best practice - Reporting in modalità testo

## Che cos’è una “best practice” di Adobe Workfront?

Le best practice sono linee guida che rappresentano una linea d’azione efficace ed efficiente; sono facilmente adottabili da te e dagli utenti della tua azienda; e possono essere replicate con successo in tutta l’organizzazione.

Mentre esamini questi consigli, tieni presente che alcune best practice di Workfront sono universali mentre altre potrebbero essere più specifiche per un dato argomento. Utilizza queste best practice come una base comune per le impostazioni e l’utilizzo del sistema Workfront.

## Esplorazione di questa pagina

Mentre scorri questa pagina, troverai innanzitutto un elenco di alto livello di tutte le best practice per questo argomento. Questo ti consente di rivedere i consigli senza entrare nei dettagli del “perché”.

La sezione “Perché queste sono best practice?”, che si trova dopo l’elenco di alto livello, fornisce maggiori dettagli su alcune delle best practice e sul motivo per cui sono considerate un processo, uno strumento ecc. da implementare con la tua istanza di Workfront.

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
