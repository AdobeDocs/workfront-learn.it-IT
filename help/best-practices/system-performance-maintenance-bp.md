---
title: Best practice - Prestazioni e manutenzione del sistema
description: Esplorare le raccomandazioni sulle best practice degli esperti Adobe Workfront relative alle prestazioni e alla manutenzione del sistema Workfront.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
kt: 10927
exl-id: c3f32975-96f4-4e62-8c3a-5b985b45bbbf
source-git-commit: 444f059d3cc26d8e3074a7145bc5419407c786cf
workflow-type: tm+mt
source-wordcount: '635'
ht-degree: 0%

---

# Best practice - Prestazioni e manutenzione del sistema

## Qual è una &quot;best practice&quot; di Adobe Workfront?

Le migliori pratiche sono linee guida che rappresentano un&#39;azione efficace ed efficiente; sono facilmente adottati da te e dagli utenti della tua azienda; e può essere replicato correttamente in tutta l’organizzazione.

Quando si esaminano queste raccomandazioni, tenere presente che alcune best practice di Workfront sono universali, mentre altre potrebbero essere più specifiche per l’argomento. Utilizza queste best practice come framework per guidare le impostazioni e l’utilizzo del sistema Workfront.

## Navigazione in questa pagina

Scorrendo questa pagina, troverai innanzitutto un elenco di alto livello contenente tutte le best practice per l’argomento. Questo ti consente di rivedere le raccomandazioni senza immergerti nei dettagli del &quot;perché&quot;.

Perché queste best practice? area, disponibile dopo l’elenco di alto livello, fornisce maggiori dettagli su alcune delle best practice e sui motivi per cui vengono considerate un processo, uno strumento, ecc., dovresti considerare l’implementazione con la tua istanza Workfront.

</br>
</br>

## Best practice relative alle prestazioni e alla manutenzione del sistema

* Rivedi le note sulla versione del prodotto prima della data di rilascio.

* Crea diversi tipi di rapporti di eccezioni che evidenziano dati e impostazioni mancanti o errati.

* Crea un processo di disattivazione utente che include una revisione degli oggetti di proprietà o assegnati loro in modo che gli utenti che non fanno più parte della società non rimangano attivi nel sistema e creino confusione per gli altri utenti.

* Mantieni le configurazioni del flusso di lavoro il più semplici possibile per assicurarti che siano scalabili e possano essere mantenute in assenza di modifiche.

* Utilizza i filtri nei rapporti e negli elenchi di oggetti per ridurre il numero di righe visualizzate contemporaneamente e concentrare il team su informazioni importanti.

* Cancella regolarmente la cache del browser e i cookie per migliorare le prestazioni in Workfront.

* Inizia a pulire il sistema nelle aree principali di Adobe Workfront che tendono ad essere più complesse, ad esempio moduli personalizzati, modelli, progetti e utenti.

* Scopri su quale cluster è attiva la tua istanza Workfront in modo da poter guardare gli aggiornamenti, essere consapevoli delle finestre di manutenzione, ecc.

* Mantieni i progetti brevi.

* Laddove possibile, mantieni i rapporti &quot;leggeri&quot; con pochissimi filtri e non complicati per migliorare le prestazioni.

</br>
</br>

## Perché queste best practice sono?

**Best practice**

Rivedi le note sulla versione del prodotto prima della data di rilascio.



**Ecco perché**

Le note sulla versione indicano quali nuove funzionalità e strumenti sono in arrivo sul sistema Workfront. Esaminando queste note e riproducendo con le nuove funzionalità nell’ambiente Sandbox di anteprima, puoi scoprire, sperimentare e risolvere eventuali bug con nuovi miglioramenti prima che vengano pubblicati in produzione.

</br>
</br>

**Best practice**

Crea diversi tipi di rapporti di eccezioni che evidenziano dati e impostazioni mancanti o errati.



**Ecco perché**

Questi rapporti includono quelli che indicano quali utenti devono essere disattivati, quali progetti mostrano una percentuale di completamento del 100% ma non sono contrassegnati come completi, quali modelli non sono mai stati utilizzati, ecc.



Inserite questi e altri report in un dashboard e date ad altri amministratori di sistema e di gruppo l&#39;accesso a questo dashboard per mantenere un sistema pulito in modo tempestivo. Ad esempio, il Dashboard di pulizia di Workfront e il Dashboard di utilizzo di Workfront includono esempi di rapporti che puoi creare.



Per aiutarti a ricordarti di controllare questi rapporti, almeno trimestralmente, crea un progetto con attività trimestrali e assegnali a te stesso e agli amministratori di sistema e di gruppo. Assicurati che a queste attività siano associate ore pianificate in modo che gli assegnatari di questi elementi di lavoro possano allocare correttamente il loro tempo.

</br>
</br>

**Best practice**

Mantieni i progetti brevi.



**Ecco perché**

Ogni volta che salvi un progetto o un’attività all’interno del progetto, è in esecuzione un calcolo della timeline per aggiornare tutte le dipendenze. A seconda del numero di attività nel progetto, l’esecuzione del ricalcolo può richiedere molto tempo.
