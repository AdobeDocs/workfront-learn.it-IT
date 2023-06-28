---
title: 'Best practice: prestazioni e manutenzione del sistema'
description: Esplora le best practice consigliate dagli esperti Adobe Workfront sulle prestazioni e la manutenzione dei sistemi Workfront.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
jira: KT-10927
exl-id: c3f32975-96f4-4e62-8c3a-5b985b45bbbf
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '635'
ht-degree: 0%

---

# Best practice: prestazioni e manutenzione del sistema

## Cos’è una &quot;best practice&quot; di Adobe Workfront?

Le best practice sono linee guida che rappresentano una linea di condotta efficace ed efficiente, sono facilmente adottabili da te e dagli utenti della tua azienda e possono essere replicate correttamente all’interno dell’organizzazione.

Mentre esamini questi consigli, tieni presente che alcune best practice di Workfront sono universali, mentre altre potrebbero essere più specifiche per l’argomento. Utilizza queste best practice come framework per guidare le impostazioni e l’utilizzo del sistema Workfront.

## Navigazione in questa pagina

Scorrendo questa pagina, troverai innanzitutto un elenco di alto livello di tutte le best practice per l’argomento. Questo ti consente di rivedere i consigli senza immergerti nei dettagli di &quot;perché&quot;.

La sezione &quot;Perché sono queste best practice?&quot; , disponibile dopo l’elenco di alto livello, fornisce maggiori dettagli su alcune delle best practice e sul perché sono considerate un processo, uno strumento, ecc., è consigliabile implementarle con l’istanza di Workfront.

</br>
</br>

## Best practice per le prestazioni del sistema e la manutenzione

* Rivedi le note sulla versione del prodotto prima della data di rilascio.

* Creare diversi tipi di report delle eccezioni che evidenziano dati e impostazioni mancanti o non corretti.

* Creare un processo di disattivazione degli utenti che includa una revisione degli oggetti di loro proprietà o a loro assegnati in modo che gli utenti che non fanno più parte dell’azienda non rimangano attivi nel sistema e creino confusione per altri utenti.

* Mantieni le configurazioni del flusso di lavoro il più semplici possibile per assicurarti che siano scalabili e possano essere mantenute in assenza di.

* Utilizzare i filtri nei report e negli elenchi di oggetti per ridurre il numero di righe visualizzate contemporaneamente e concentrare il team su informazioni importanti.

* Cancella regolarmente la cache del browser e i cookie per migliorare le prestazioni in Workfront.

* Inizia a pulire il sistema nelle principali aree di Adobe Workfront che tendono a essere più disordinate, come moduli personalizzati, modelli, progetti e utenti.

* Scopri il cluster su cui si trova l’istanza di Workfront, in modo da poter controllare gli aggiornamenti, conoscere le finestre di manutenzione e così via.

* Mantieni i progetti brevi.

* Laddove possibile, mantieni i rapporti &quot;leggeri&quot; con pochissimi e semplici filtri per migliorare le prestazioni.

</br>
</br>

## Perché si tratta di procedure ottimali?

**Best practice**

Rivedi le note sulla versione del prodotto prima della data di rilascio.



**Ecco perché**

Le note sulla versione illustrano le nuove funzionalità e gli strumenti che verranno introdotti nel sistema Workfront. Esaminando queste note e giocando con la nuova funzionalità nell’ambiente Sandbox in anteprima, hai la possibilità di scoprire, esercitarti con e risolvere eventuali bug con nuovi miglioramenti prima che vengano rilasciati in produzione.

</br>
</br>

**Best practice**

Creare diversi tipi di report delle eccezioni che evidenziano dati e impostazioni mancanti o non corretti.



**Ecco perché**

Questi rapporti includono quelli che indicano quali utenti devono essere disattivati, quali progetti mostrano una percentuale di completamento del 100% ma non sono contrassegnati come completati, quali modelli non sono mai stati utilizzati e così via.



Inserisci questi rapporti come questi e altri su un dashboard e concedi ad altri amministratori di sistema e di gruppo l’accesso a questo dashboard per mantenere un sistema pulito in modo tempestivo. Ad esempio, Workfront Cleanup Dashboard e Workfront Usage Dashboard includono esempi di report che è possibile creare.



Per ricordarti di controllare questi rapporti, crea un progetto con attività trimestrali e assegnalo a te stesso e agli amministratori di sistema e di gruppo, almeno una volta al trimestre. Accertarsi che a queste attività siano associate ore pianificate in modo che gli assegnatari di questi elementi di lavoro possano allocare correttamente il tempo.

</br>
</br>

**Best practice**

Mantieni i progetti brevi.



**Ecco perché**

Ogni volta che si salva un progetto o un&#39;attività all&#39;interno del progetto, viene eseguito un calcolo della sequenza temporale per aggiornare tutte le dipendenze. A seconda del numero di attività nel progetto, l&#39;esecuzione del ricalcolo può richiedere molto tempo.
