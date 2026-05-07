---
title: Best practice - Prestazioni e manutenzione del sistema
description: Esplora le best practice consigliate dagli esperti di Adobe Workfront sulle prestazioni e la manutenzione dei sistemi Workfront.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
jira: KT-10927
exl-id: c3f32975-96f4-4e62-8c3a-5b985b45bbbf
TQID: https://experienceleague.adobe.com/2tq7aNHE96fep1EFCPrjcCo13t5lQ24A6c-ORDUmlpY
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bdid: f8a45b24-4be7-4f1b-909b-60d06b483a20
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 36674ed53c8645f556862bb2d99f3bfd6c993c1e
workflow-type: tm+mt
source-wordcount: 638
ht-degree: 93%

---

# Best practice - Prestazioni e manutenzione del sistema

## Che cos’è una “best practice” di Adobe Workfront?

Le best practice sono linee guida che rappresentano una linea d’azione efficace ed efficiente; sono facilmente adottabili da te e dagli utenti della tua azienda; e possono essere replicate con successo in tutta l’organizzazione.

Mentre esamini questi consigli, tieni presente che alcune best practice di Workfront sono universali mentre altre potrebbero essere più specifiche per un dato argomento. Utilizza queste best practice come una base comune per le impostazioni e l’utilizzo del sistema Workfront.

## Esplorazione di questa pagina

Mentre scorri questa pagina, troverai innanzitutto un elenco di alto livello di tutte le best practice per questo argomento. Questo ti consente di rivedere i consigli senza entrare nei dettagli del “perché”.

L’area &quot;Perché queste best practice?&quot;, che si trova dopo l’elenco di alto livello, fornisce maggiori dettagli su alcune delle best practice e sul perché vengono considerate un processo, uno strumento, ecc., è consigliabile implementarle con l’istanza di Workfront.

</br>
</br>

## Best practice per le prestazioni del sistema e la manutenzione

* Consulta le note sulla versione del prodotto prima della data di rilascio.

* Crea diversi tipi di rapporto delle eccezioni per evidenziare dati e impostazioni mancanti o errati.

* Crea un processo di disattivazione degli utenti che includa la revisione degli oggetti di loro proprietà o a loro assegnati in modo che gli utenti che non fanno più parte dell’azienda non rimangano attivi nel sistema e creino confusione per altri utenti.

* Mantieni le configurazioni dei flussi di lavoro il più semplici possibile per assicurarti che siano scalabili e possano essere mantenute in tua assenza.

* Utilizza i filtri nei rapporti e negli elenchi di oggetti per ridurre il numero di righe visualizzate contemporaneamente e concentrare l’attenzione sulle informazioni più importanti.

* Cancella regolarmente la cache del browser e i cookie per migliorare le prestazioni in Workfront.

* Inizia a pulire il sistema nelle principali aree di Adobe Workfront che tendono a essere più disordinate, come moduli personalizzati, modelli, progetti e utenti.

* Scopri il cluster su cui si trova la tua istanza di Workfront, in modo da poter controllare quando vi sono aggiornamenti, conoscerne le finestre di manutenzione e così via.

* Mantieni i progetti brevi.

* Laddove possibile, mantieni i rapporti “leggeri” con pochissimi e semplici filtri per migliorare le prestazioni.

</br>
</br>

## Perché queste sono best practice?

**Best practice**

Consulta le note sulla versione del prodotto prima della data di rilascio.



**Ecco perché**

Le note sulla versione illustrano le nuove funzionalità e gli strumenti che verranno introdotti nel sistema Workfront. Esaminando queste note e provando le nuove funzionalità nell’ambiente Sandbox di anteprima, hai la possibilità di scoprirle e fare pratica e di risolvere eventuali bug nei nuovi miglioramenti prima che vengano rilasciati in produzione.

</br>
</br>

**Best practice**

Crea diversi tipi di rapporto delle eccezioni per evidenziare dati e impostazioni mancanti o errati.



**Ecco perché**

Questi rapporti includono quelli che indicano quali utenti devono essere disattivati, quali progetti mostrano una percentuale di completamento del 100% ma non sono contrassegnati come completati, quali modelli non sono mai stati utilizzati e così via.



Inserisci i rapporti come questi e altri su una dashboard e concedi ad altri amministratori di sistema e di gruppo l’accesso a tale dashboard per mantenere un sistema sempre pulito. Ad esempio, Workfront Cleanup Dashboard e Workfront Usage Dashboard includono esempi di rapporto che è possibile creare.



Per ricordarti di controllare questi rapporti, crea un progetto con attività trimestrali e assegnalo a te stesso e agli amministratori di sistema e di gruppo, almeno una volta al trimestre. Accertati che a queste attività siano associate ore pianificate in modo che gli assegnatari di questi elementi di lavoro possano allocare correttamente il tempo.

</br>
</br>

**Best practice**

Mantieni i progetti brevi.



**Ecco perché**

Ogni volta che salvi un progetto o un’attività all’interno del progetto, viene eseguito un calcolo della timeline per aggiornare tutte le dipendenze. A seconda del numero di attività nel progetto, l’esecuzione del ricalcolo può richiedere molto tempo.
