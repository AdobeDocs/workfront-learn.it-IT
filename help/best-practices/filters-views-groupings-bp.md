---
title: Best practice - Filtri, viste e raggruppamenti
description: Esplora le best practice consigliate dagli esperti di Adobe Workfront in merito alla configurazione, alla gestione e all’utilizzo di filtri, viste e raggruppamenti in Workfront.
feature: Reports and Dashboards
role: Admin, Leader, User
level: Beginner
jira: KT-10911
exl-id: 845aa0b4-3fe9-4bc1-9dde-2f22c537e758
source-git-commit: 0ff5accae867f07cc31ac2be7b0c12981412346e
workflow-type: ht
source-wordcount: '785'
ht-degree: 100%

---

# Best practice - Filtri, viste e raggruppamenti

## Che cos’è una “best practice” di Adobe Workfront?

Le best practice sono linee guida che rappresentano una linea d’azione efficace ed efficiente; sono facilmente adottabili da te e dagli utenti della tua azienda; e possono essere replicate con successo in tutta l’organizzazione.

Mentre esamini questi consigli, tieni presente che alcune best practice di Workfront sono universali mentre altre potrebbero essere più specifiche per un dato argomento. Utilizza queste best practice come una base comune per le impostazioni e l’utilizzo del sistema Workfront.

## Esplorazione di questa pagina

Scorrendo questa pagina, troverai innanzitutto un elenco di alto livello di tutte le best practice relative all’argomento. Questo ti consente di rivedere i consigli senza immergerti nei dettagli delle motivazioni.

“Perché queste sono best practice?” che si trova dopo l’elenco di alto livello, fornisce maggiori dettagli su alcune delle best practice e sul motivo per cui sono considerate un processo, uno strumento ecc. da implementare con la tua istanza di Workfront.

</br>
</br>

## Best practice per filtri, viste e raggruppamenti

* Riduci il numero di report personalizzati creati sfruttando i filtri, le viste e i raggruppamenti in un elenco di oggetti per ottenere i dati necessari.

* Utilizza i controlli elenco nei modelli di layout per nascondere filtri, viste e raggruppamenti non necessari per oggetti di uso comune (progetti, attività, programmi, ecc.).

* Tramite i controlli elenco sui modelli di layout, puoi condividere filtri, viste e raggruppamenti personalizzati in base ai flussi di lavoro e ai processi della tua organizzazione.

* Durante la creazione di filtri per lo stato di un progetto, di un’attività o di un problema, utilizza il modificatore (oggetto)>>Stato corrisponde a origine campo/nome campo con modificatore uguale, anziché Progetto>>Stato origine campo/nome campo.

</br>
</br>

## Perché queste sono best practice?

**Best practice**

Riduci il numero di report personalizzati creati sfruttando i filtri, le viste e i raggruppamenti in un elenco di oggetti per ottenere i dati necessari.

**Ecco perché**

La creazione di rapporti di utilizzo singoli per ogni segmento di dati che desideri visualizzare richiede molto tempo e rende il sistema Workfront più complesso.

Per istruzioni su come creare rapporti con prompt, consulta il capitolo “Come impostare e utilizzare i prompt dei rapporti” nel video [Comprendere le impostazioni dei rapporti](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/report-settings.html?lang=it).

Per istruzioni su come creare rapporti con prompt personalizzati, consulta [Creare prompt personalizzati](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/intermediate-reporting/custom-prompts.html?lang=it).

</br>
</br>

**Best practice**

Utilizza i controlli elenco nei modelli di layout per nascondere filtri, viste e raggruppamenti non necessari per oggetti di uso comune (progetti, attività, programmi, ecc.).

**Ecco perché**

Meno è meglio. Quando si nascondono opzioni di filtro, vista e raggruppamento di elenchi che non sono rilevanti per i flussi di lavoro giornalieri degli utenti, gli elenchi sono ridotti ed è più semplice e veloce cercare ciò di cui si ha bisogno.

Per istruzioni su come nascondere filtri, viste o raggruppamenti con i modelli di layout, consulta [Personalizzare gli elenchi dei report con i modelli di layout](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/administration-and-setup/layout-templates/customize-reporting-lists-with-layout-templates.html?lang=it).

</br>
</br>

**Best practice**

Tramite i controlli elenco sui modelli di layout, puoi condividere filtri, viste e raggruppamenti personalizzati in base ai flussi di lavoro e ai processi della tua organizzazione.

**Ecco perché**

Se hai creato filtri, viste e raggruppamenti che mostrano informazioni specifiche dei processi giornalieri degli utenti, è facile condividerli attraverso i modelli di layout. In questo modo, tutti gli utenti assegnati al modello di layout avranno a disposizione opzioni di filtro, vista e raggruppamento rilevanti per i propri flussi di lavoro.

La personalizzazione delle informazioni che desideri rendere visibili agli utenti tramite i modelli di layout consente inoltre di risparmiare tempo agli amministratori di sistema e di gruppo, in quanto non dovranno condividere ogni opzione di filtro, vista o raggruppamento singolarmente.

Per istruzioni su come condividere filtri, viste o raggruppamenti con i modelli di layout, consulta [Personalizzare gli elenchi dei rapporti con i modelli di layout](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/administration-and-setup/layout-templates/customize-reporting-lists-with-layout-templates.html?lang=it).

</br>
</br>

**Best practice**

Durante la creazione di filtri per lo stato di un progetto, di un’attività o di un problema, utilizza il modificatore (oggetto)>>Stato corrisponde a origine campo/nome campo con modificatore uguale, anziché Progetto>>Stato origine campo/nome campo.

**Ecco perché**

Utilizzando (oggetto)>>Uguale a, includi tutti gli stati personalizzati a cui è assegnato lo stato specifico nel campo Uguale a nelle impostazioni dello stato. Mentre l’impostazione del filtro come (oggetto)>>Stato > Uguale richiede la selezione di statuti specifici per il filtro. Se devi tenere conto di questi nuovi stati in vari filtri, questo potrebbe presentare un problema relativo alla manutenzione. Ogni filtro dovrà essere aperto e aggiornato con il nuovo stato.

Ad esempio, per visualizzare tutti i progetti correnti, puoi impostare il filtro in modo che risulti Progetto>>Stato > Uguale > Corrente. Tuttavia, se qualcuno aggiunge uno stato personalizzato denominato Attivo e lo rende uguale a Corrente, tale filtro non troverà i progetti con lo stato Attivo. Comunque, se utilizzi Progetto>>Stato Uguale a > Uguale > Corrente, in questo caso il filtro trova gli oggetti con lo stato Corrente o Attivo perché entrambi hanno Corrente nel campo Uguale a.
