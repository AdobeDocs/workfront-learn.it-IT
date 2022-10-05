---
title: 'Procedure consigliate: filtri, visualizzazioni e raggruppamenti'
description: Scopri le best practice consigliate dagli esperti di Adobe Workfront sull’impostazione, la gestione e l’utilizzo di filtri, visualizzazioni e raggruppamenti Workfront.
feature: Reports and Dashboards
role: Admin, Leader, User
level: Beginner
kt: 10911
exl-id: 845aa0b4-3fe9-4bc1-9dde-2f22c537e758
source-git-commit: 444f059d3cc26d8e3074a7145bc5419407c786cf
workflow-type: tm+mt
source-wordcount: '700'
ht-degree: 0%

---

# Procedure consigliate: filtri, visualizzazioni e raggruppamenti

## Qual è una &quot;best practice&quot; di Adobe Workfront?

Le migliori pratiche sono linee guida che rappresentano un&#39;azione efficace ed efficiente; sono facilmente adottati da te e dagli utenti della tua azienda; e può essere replicato correttamente in tutta l’organizzazione.

Quando si esaminano queste raccomandazioni, tenere presente che alcune best practice di Workfront sono universali, mentre altre potrebbero essere più specifiche per l’argomento. Utilizza queste best practice come framework per guidare le impostazioni e l’utilizzo del sistema Workfront.

## Navigazione in questa pagina

Scorrendo questa pagina, troverai innanzitutto un elenco di alto livello contenente tutte le best practice per l’argomento. Questo ti consente di rivedere le raccomandazioni senza immergerti nei dettagli del &quot;perché&quot;.

Perché queste best practice? area, disponibile dopo l’elenco di alto livello, fornisce maggiori dettagli su alcune delle best practice e sui motivi per cui vengono considerate un processo, uno strumento, ecc., dovresti considerare l’implementazione con la tua istanza Workfront.

</br>
</br>

## Best practice per filtri, viste e raggruppamenti

* Puoi ridurre il numero di rapporti personalizzati creati sfruttando filtri, visualizzazioni e raggruppamenti in un elenco di oggetti per ottenere i dati necessari.

* I controlli elenco nei modelli layout consentono di nascondere i filtri, le visualizzazioni e i raggruppamenti non necessari per gli oggetti di uso comune (progetti, attività, programmi, ecc.).

* Puoi condividere filtri, viste e raggruppamenti personalizzati relativi ai flussi di lavoro e ai processi della tua organizzazione tramite i controlli elenco sui modelli di layout.

* Quando si creano filtri per lo stato del progetto, lo stato dell&#39;attività o dello stato del problema, utilizzare (oggetto)>>Stato Equivale con il nome dell&#39;origine del campo/campo con il modificatore Equal, anziché il nome dell&#39;origine del campo o del campo di stato Progetto>>Stato.

</br>
</br>

## Perché queste best practice sono?

**Best practice**

Puoi ridurre il numero di rapporti personalizzati creati sfruttando filtri, visualizzazioni e raggruppamenti in un elenco di oggetti per ottenere i dati necessari.

**Ecco perché**

La creazione di rapporti di utilizzo una tantum per ogni segmento di dati che desideri visualizzare richiede molto tempo e ottimizza il sistema Workfront.

</br>
</br>

**Best practice**

I controlli elenco nei modelli layout consentono di nascondere i filtri, le visualizzazioni e i raggruppamenti non necessari per gli oggetti di uso comune (progetti, attività, programmi, ecc.).

**Ecco perché**

Meno è di più. Le opzioni di filtro, visualizzazione e raggruppamento di elenchi che non sono rilevanti per i flussi di lavoro giornalieri degli utenti si limitano agli elenchi, facilitando agli utenti la ricerca di ciò di cui hanno bisogno più rapidamente.

</br>
</br>

**Best practice**

Puoi condividere filtri, viste e raggruppamenti personalizzati relativi ai flussi di lavoro e ai processi della tua organizzazione tramite i controlli elenco sui modelli di layout.

**Ecco perché**

Se hai creato filtri, visualizzazioni e raggruppamenti che visualizzano informazioni specifiche dei processi giornalieri degli utenti, è facile condividerli attraverso i modelli di layout. In questo modo, tutti gli utenti a cui è stato assegnato un modello di layout dispongono di opzioni di filtro, visualizzazione e raggruppamento pertinenti per i propri flussi di lavoro.

La personalizzazione delle informazioni che si desidera rendere visibili agli utenti tramite i modelli di layout consente inoltre agli amministratori di sistema e di gruppo di risparmiare tempo perché non dovranno condividere singolarmente ogni filtro, visualizzazione o opzione di raggruppamento.

</br>
</br>

**Best practice**

Quando si creano filtri per lo stato del progetto, lo stato dell&#39;attività o dello stato del problema, utilizzare (oggetto)>>Stato Equivale con il nome dell&#39;origine del campo/campo con il modificatore Equal, anziché il nome dell&#39;origine del campo o del campo di stato Progetto>>Stato.

**Ecco perché**

Utilizzando (oggetto)>>Equula con, vengono inclusi nelle impostazioni di stato tutti gli stati personalizzati a cui è stato assegnato lo stato specifico nel campo Equazioni con . Quando si imposta il filtro come (oggetto)>>Stato > Uguale (Equal), è necessario selezionare uno stato specifico per il filtro. Questo potrebbe rappresentare un problema di manutenzione se devi tenere conto di questi nuovi stati in diversi filtri. Ogni filtro deve essere aperto e aggiornato con il nuovo stato .

Ad esempio, se desideri visualizzare tutti i progetti correnti, puoi impostare il filtro per leggere Progetto >>Stato > Uguale > Corrente. Tuttavia, se un utente aggiunge uno stato personalizzato denominato Attivo e lo equa Corrente, tale filtro non troverà progetti con lo stato Attivo. Tuttavia, se si utilizza Progetto >>Equazioni stato con > Uguale > Corrente, il filtro trova gli oggetti con lo stato Corrente o Attivo perché entrambi hanno Corrente nel campo Equazioni con.
