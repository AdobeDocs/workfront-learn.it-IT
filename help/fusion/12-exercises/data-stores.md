---
title: Archivi dati
description: Scopri come sincronizzare i nomi delle società tra due sistemi. (Deve essere compreso tra 60 e 160 caratteri, ma è di 59 caratteri)
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11055
thumbnail: KT11055.png
exl-id: e4aa9a97-679a-4575-a2c6-b6ac304ce9c2
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '878'
ht-degree: 0%

---

# Archivi dati

Scopri come sincronizzare i nomi delle società tra due sistemi.

## Panoramica dell’esercizio

Questa è la prima parte di una sincronizzazione unidirezionale delle aziende in Workfront e in un altro sistema. Per il momento, esegue la sincronizzazione solo tra un archivio dati di Fusion e Workfront. Una tabella in un archivio dati tiene traccia del Workfront ID (WFID) e dell’ID azienda nel file CSV (CID) per ogni azienda. Ciò consente una sincronizzazione bidirezionale in futuro.

![Archivio dati Immagine 1](../12-exercises/assets/data-stores-walkthrough-1.png)

## Passaggi da seguire

**Scarica il file da Workfront.**

1. Nella cartella &quot;Fusion Exercise Files&quot; di Workfront, selezionate &quot;_Companies.csv&quot; e fate clic su Dettagli documento.
1. Copia il primo numero ID dall’indirizzo URL.
1. In Fusion, crea un nuovo scenario denominato &quot;Utilizzo degli archivi dati per sincronizzare i dati&quot;.
1. Per il modulo trigger, seleziona il modulo Workfront Download Document.
1. Configura la connessione Workfront e includi l’ID documento copiato dall’URL di Workfront.
1. Denomina questo modulo &quot;Ottieni file società&quot;.
1. Ora aggiungi un modulo CSV di analisi.
1. Per il campo Numero di colonne digitare 2.
1. Mappa i dati dal modulo Scarica documento nel campo CSV.
1. Denomina questo modulo &quot;Analizza file delle società&quot;.
1. Salva lo scenario e fai clic su Esegui una volta.

   **Crea un archivio dati e una struttura dati.**

1. Aggiungi un modulo per i record di ricerca dell’archivio dati.
1. Crea un nuovo archivio dati denominato &quot;Sincronizzazione società&quot;.
1. All&#39;interno dell&#39;archivio dati, creare una struttura di dati denominata &quot;Sincronizzazione società (struc)&quot;.
1. Crea quattro campi.

   + CID: l’ID azienda nel file CSV
   + Nome dell’azienda
   + WFID - ID società Workfront
   + Data di creazione: assicurarsi che il tipo di dati sia data

   ![Archivio dati - Immagine 2](../12-exercises/assets/data-stores-walkthrough-2.png)

1. Fai clic su Salva nella struttura dati, quindi imposta la dimensione di archiviazione dati su 1 e salva l’archivio dati.
1. Continuando nel modulo Archivio dati, imposta un filtro in cui il CID è uguale all’ID della società dal modulo CSV di analisi (colonna 1).
1. Fai clic su Mostra impostazioni avanzate e seleziona l’opzione per &quot;continuare l’esecuzione dello scenario o del percorso, anche se questo modulo non restituisce alcun risultato&quot;.

   ![Archivio dati Immagine 3](../12-exercises/assets/data-stores-walkthrough-3.png)

1. Rinomina questo modulo &quot;Corrispondenza con le aziende&quot;.
1. Aggiungi un modulo record di Workfront Search.
1. Scegliere Società come tipo di record.
1. Criteri di ricerca è il nome dell’azienda in Workfront è uguale al nome dell’azienda nel file CSV.
1. Per gli output, seleziona il nome della società e l’ID.

   ![Archivio dati - Immagine 4](../12-exercises/assets/data-stores-walkthrough-4.png)

1. Fare clic su OK e rinominare il modulo &quot;Corrispondenza società&quot;.

   **Creare percorsi diversi a seconda che l’azienda esista all’interno di Workfront o nell’archivio dati.**

   **Percorso ciclo 1: creare una società.**

1. Aggiungere un modulo router a destra del modulo record di Workfront Search.
1. Aggiungi un modulo Workfront Create Record al percorso principale.
1. Impostare il tipo di record su Società.
1. Seleziona Nome da Campi da mappare. Mappa il campo del nome sull’output del modulo CSV di analisi (colonna 2).
1. Rinomina questo modulo &quot;Crea azienda&quot;.

   ![Archivio dati - Immagine 5](../12-exercises/assets/data-stores-walkthrough-5.png)

1. Aggiungere un filtro dopo il router per creare una società solo se non è già in Workfront. Denominalo &quot;Not in Workfront&quot;.
1. Imposta la condizione sull’ID dal modulo di ricerca di Workfront e non esiste.

   ![Archivio dati - Immagine 6](../12-exercises/assets/data-stores-walkthrough-6.png)

   **Prepara l’aggiornamento dell’archivio dati nel percorso successivo.**

1. Aggiungi un modulo Imposta variabile alla fine del percorso principale.
1. Imposta il nome della variabile su &quot;Workfront ID&quot;.
1. Imposta il valore Variable sull’ID dal modulo Create company (Crea azienda).
1. Rinomina il modulo &quot;Set Workfront ID&quot;.

   **Percorso di indirizzamento 2: aggiorna l’archivio dati.**

1. Creare un filtro nel percorso di routing 2. Denomina &quot;Not in data store&quot; (Non nell’archivio dati).

1. Imposta la Condizione sulla Chiave dal modulo Archivio dati e non esiste.

   ![Archivio dati - Immagine 7](../12-exercises/assets/data-stores-walkthrough-7.png)

1. Il primo modulo di questo percorso è il modulo variabile Get.
1. Imposta il nome della variabile su &quot;Workfront ID&quot;.
1. Rinomina questo modulo &quot;Ottieni ID Workfront&quot;.
1. Aggiungi un altro modulo dall’app Data Store e aggiungi/sostituisci un record.
1. Nel campo Archivio dati scegliere Sincronizzazione società. Archivio dati creato in precedenza.
1. Lascia vuoto il campo Chiave.
1. Mappa il campo CID dalla colonna 1 nel modulo CSV di analisi.
1. Mappa il campo del nome della società dalla colonna 2 nel modulo CSV di analisi.
1. Mappa il campo WFID dal modulo Get Workfront ID.
1. Per il campo Data di creazione, utilizzare la funzione formatDate della scheda Data e ora per formattare la data corrente come MM/GG/AAAA.

   ![Archivio dati - Immagine 8](../12-exercises/assets/data-stores-walkthrough-8.png)

1. Fare clic su OK e rinominare il modulo &quot;Crea voce società&quot;.

   **Percorso di routing 3: sincronizza l&#39;archivio dati tra i sistemi.**

1. Iniziare creando un filtro sul percorso di routing 3. Denomina l&#39;azienda &quot;Esiste, non nell&#39;archivio dati&quot;.
1. Imposta la Condizione sulla Chiave dal modulo Record di ricerca dell’archivio dati e non esiste.
1. Fai clic sul pulsante Aggiungi regola AND e specifica che il nome della società dal file CSV (colonna 2) è uguale al nome della società trovato nel modulo Workfront Search.

   ![Archivio dati - Immagine 9](../12-exercises/assets/data-stores-walkthrough-9.png)

1. Aggiungere un altro modulo Aggiungi/sostituisci un modulo record clonando quello alla fine del percorso di routing 2.
1. Trascinare il modulo clonato in posizione alla fine del percorso di routing 3. Elimina il modulo vuoto presente.
1. Fai clic sul modulo clonato. Tutti i campi devono rimanere invariati, ad eccezione del campo WFID. Mappalo dal modulo di ricerca Aziende corrispondenti.

   ![Archivia dati - Immagine 10](../12-exercises/assets/data-stores-walkthrough-10.png)

1. Fare clic su OK e rinominare il modulo &quot;Crea voce società&quot;.
