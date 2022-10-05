---
title: Procedure consigliate - Generazione rapporti in modalità testo
description: Scopri le best practice consigliate dagli esperti di Adobe Workfront sull’impostazione, la gestione e l’utilizzo dei rapporti in modalità testo di Workfront.
feature: Reports and Dashboards
role: Admin, Leader, User
level: Beginner
kt: 10928
exl-id: c624545c-ba42-4cc3-aafe-8be15baadb75
source-git-commit: 444f059d3cc26d8e3074a7145bc5419407c786cf
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 0%

---

# Procedure consigliate - Generazione rapporti in modalità testo

## Qual è una &quot;best practice&quot; di Adobe Workfront?

Le migliori pratiche sono linee guida che rappresentano un&#39;azione efficace ed efficiente; sono facilmente adottati da te e dagli utenti della tua azienda; e può essere replicato correttamente in tutta l’organizzazione.

Quando si esaminano queste raccomandazioni, tenere presente che alcune best practice di Workfront sono universali, mentre altre potrebbero essere più specifiche per l’argomento. Utilizza queste best practice come framework per guidare le impostazioni e l’utilizzo del sistema Workfront.

## Navigazione in questa pagina

Scorrendo questa pagina, troverai innanzitutto un elenco di alto livello contenente tutte le best practice per l’argomento. Questo ti consente di rivedere le raccomandazioni senza immergerti nei dettagli del &quot;perché&quot;.

Perché queste best practice? area, disponibile dopo l’elenco di alto livello, fornisce maggiori dettagli su alcune delle best practice e sui motivi per cui vengono considerate un processo, uno strumento, ecc., dovresti considerare l’implementazione con la tua istanza Workfront.

</br>
</br>

## Best practice per la generazione di rapporti in modalità testo

* Utilizza le espressioni di valore della modalità testo invece dei campi personalizzati calcolati quando possibile nelle colonne dei rapporti elenco.

* Inserire i calcoli utilizzati nel calcolo in modalità testo nella descrizione del rapporto.

</br>
</br>

## Perché queste best practice sono?

**Best practice**

Utilizza le espressioni di valore della modalità testo invece dei campi personalizzati calcolati quando possibile nelle colonne dei rapporti elenco.



**Ecco perché**

Le espressioni del valore della modalità testo vengono calcolate al momento dell’esecuzione del rapporto e vengono ricalcolate ogni volta che questo viene aggiornato. Ciò significa che avrai sempre a disposizione dati aggiornati e rapporti precisi.



I campi personalizzati calcolati (utilizzati nei moduli personalizzati) non vengono aggiornati automaticamente quando i dati vengono visualizzati in Workfront. Al contrario, visualizzano i risultati del calcolo più recente memorizzato in Workfront. Ciò significa che tali valori potrebbero essere &quot;obsoleti&quot; o obsoleti in un dato momento. I campi personalizzati calcolati devono essere aggiornati manualmente, ricalcolando l’espressione o modificando e salvando l’oggetto che contiene il campo calcolato. Questo può richiedere molto tempo, così come è facile dimenticare di farlo.


</br>
</br>

**Best practice**

Inserire i calcoli utilizzati nel calcolo in modalità testo nella descrizione del rapporto.



**Ecco perché**

L’inclusione di calcoli in modalità testo nella descrizione del rapporto aiuta altri a comprendere come è stato creato il calcolo e che tipo di informazioni deve visualizzare. Inoltre, ricorda agli amministratori di sistema come è stato creato il rapporto, nel caso in cui siano necessari aggiornamenti in futuro.
