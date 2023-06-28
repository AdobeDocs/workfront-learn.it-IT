---
title: 'Best practice: filtri, visualizzazioni e raggruppamenti'
description: Esplora le best practice consigliate dagli esperti di Adobe Workfront in merito alla configurazione, alla gestione e all’utilizzo di filtri, visualizzazioni e raggruppamenti Workfront.
feature: Reports and Dashboards
role: Admin, Leader, User
level: Beginner
jira: KT-10911
exl-id: 845aa0b4-3fe9-4bc1-9dde-2f22c537e758
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '700'
ht-degree: 0%

---

# Best practice: filtri, visualizzazioni e raggruppamenti

## Cos’è una &quot;best practice&quot; di Adobe Workfront?

Le best practice sono linee guida che rappresentano una linea di condotta efficace ed efficiente, sono facilmente adottabili da te e dagli utenti della tua azienda e possono essere replicate correttamente all’interno dell’organizzazione.

Mentre esamini questi consigli, tieni presente che alcune best practice di Workfront sono universali, mentre altre potrebbero essere più specifiche per l’argomento. Utilizza queste best practice come framework per guidare le impostazioni e l’utilizzo del sistema Workfront.

## Navigazione in questa pagina

Scorrendo questa pagina, troverai innanzitutto un elenco di alto livello di tutte le best practice per l’argomento. Questo ti consente di rivedere i consigli senza immergerti nei dettagli di &quot;perché&quot;.

La sezione &quot;Perché sono queste best practice?&quot; , disponibile dopo l’elenco di alto livello, fornisce maggiori dettagli su alcune delle best practice e sul perché sono considerate un processo, uno strumento, ecc., è consigliabile implementarle con l’istanza di Workfront.

</br>
</br>

## Best practice per filtri, visualizzazioni e raggruppamenti

* Riduci il numero di report personalizzati creati sfruttando filtri, viste e raggruppamenti in un elenco di oggetti per ottenere i dati necessari.

* Utilizzare i controlli elenco nei modelli di layout per nascondere filtri, visualizzazioni e raggruppamenti non necessari per gli oggetti di uso comune (progetti, attività, programmi, ecc.).

* Puoi condividere filtri, visualizzazioni e raggruppamenti personalizzati in base ai flussi di lavoro e ai processi della tua organizzazione, tramite i controlli elenco sui modelli di layout.

* Quando si creano filtri per lo stato di un progetto, di un&#39;attività o di un problema, utilizzare il modificatore (oggetto)>>Stato corrisponde al nome campo/origine campo con uguale, anziché il nome campo/origine campo Progetto>>Stato.

</br>
</br>

## Perché si tratta di procedure ottimali?

**Best practice**

Riduci il numero di report personalizzati creati sfruttando filtri, viste e raggruppamenti in un elenco di oggetti per ottenere i dati necessari.

**Ecco perché**

La creazione di rapporti di utilizzo una tantum per ogni segmento di dati che si desidera visualizzare richiede molto tempo e rende il sistema Workfront più complesso.

</br>
</br>

**Best practice**

Utilizzare i controlli elenco nei modelli di layout per nascondere filtri, visualizzazioni e raggruppamenti non necessari per gli oggetti di uso comune (progetti, attività, programmi, ecc.).

**Ecco perché**

Meno è di più. Quando si nascondono opzioni di filtro, visualizzazione e raggruppamento di elenchi che non sono rilevanti per i flussi di lavoro giornalieri degli utenti, gli elenchi vengono limitati in modo da facilitare agli utenti la ricerca di ciò di cui hanno bisogno più rapidamente.

</br>
</br>

**Best practice**

Puoi condividere filtri, visualizzazioni e raggruppamenti personalizzati in base ai flussi di lavoro e ai processi della tua organizzazione, tramite i controlli elenco sui modelli di layout.

**Ecco perché**

Se hai creato filtri, viste e raggruppamenti che visualizzano informazioni specifiche dei processi giornalieri degli utenti, è facile condividerli attraverso i modelli di layout. In questo modo, tutti gli utenti assegnati al modello di layout avranno a disposizione opzioni di filtro, visualizzazione e raggruppamento rilevanti per i propri flussi di lavoro.

La personalizzazione delle informazioni che si desidera rendere visibili agli utenti tramite i modelli di layout consente inoltre di risparmiare tempo agli amministratori di sistema e di gruppo, in quanto non dovranno condividere ogni filtro, visualizzazione o opzione di raggruppamento singolarmente.

</br>
</br>

**Best practice**

Quando si creano filtri per lo stato di un progetto, di un&#39;attività o di un problema, utilizzare il modificatore (oggetto)>>Stato corrisponde al nome campo/origine campo con uguale, anziché il nome campo/origine campo Progetto>>Stato.

**Ecco perché**

Utilizzando (object)>>Equivale a, si includono tutti gli stati personalizzati a cui è assegnato lo stato specifico nel campo Equivale a nelle impostazioni dello stato. Mentre l&#39;impostazione del filtro come (oggetto)>>Stato > Uguale richiede la selezione di statuti specifici per il filtro. Questo potrebbe rappresentare un problema di manutenzione se devi tenere conto di questi nuovi stati in vari filtri. Ogni filtro deve essere aperto e aggiornato con il nuovo stato.

Ad esempio, per visualizzare tutti i progetti correnti, puoi impostare il filtro su Leggi progetto>>Stato > Uguale > Corrente. Tuttavia, se qualcuno aggiunge uno stato personalizzato denominato Attivo e lo identifica a Corrente, tale filtro non troverà i progetti con lo stato Attivo. Tuttavia, se si utilizza Progetto>>Stato equivale a > Uguale a > Corrente, il filtro trova gli oggetti con lo stato Corrente o Attivo perché entrambi hanno Corrente nel campo Equivale a.
