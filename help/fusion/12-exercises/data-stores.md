---
title: Archiviazione dati
description: Scopri come sincronizzare i nomi aziendali tra due sistemi. (Deve essere compreso tra 60 e 160 caratteri, ma è di 59 caratteri)
feature: Workfront Fusion
role: User
level: Beginner
kt: 11055
thumbnail: KT11055.png
source-git-commit: c348222464180e994e7b414d1b84e07f58b6b2ae
workflow-type: tm+mt
source-wordcount: '878'
ht-degree: 0%

---


# Archiviazione dati

Scopri come sincronizzare i nomi aziendali tra due sistemi.

## Panoramica sull&#39;esercizio

Questa è la prima parte di una sincronizzazione unidirezionale delle aziende in Workfront e in un altro sistema. Per il momento, si sincronizza solo tra un archivio dati Fusion e Workfront. Una tabella in un archivio dati tiene traccia dell’ID Workfront (WFID) e dell’ID società nel file CSV (CID) per ogni azienda. Ciò consente una sincronizzazione bidirezionale a un certo punto in futuro.

![Memorizzazione dei dati Immagine 1](../12-exercises/assets/data-stores-walkthrough-1.png)

## Passaggi da seguire

**Scarica il file da Workfront.**

1. Nella cartella &quot;File di esercizio di fusione&quot; di Workfront, selezionare &quot;_Companies.csv&quot; e fare clic su Dettagli documento.
1. Copia il primo numero ID dall&#39;indirizzo URL.
1. In Fusion, creare un nuovo scenario denominato &quot;Utilizzo degli archivi dati per sincronizzare i dati&quot;.
1. Per il modulo trigger, seleziona il modulo Workfront Download Document .
1. Imposta la connessione Workfront e includi l’ID documento copiato dall’URL Workfront.
1. Denomina questo modulo &quot;Ottieni file società&quot;.
1. Ora aggiungi un modulo CSV parse.
1. Per il campo Numero di colonne, digitare 2.
1. Mappa i dati dal modulo Scarica documento nel campo CSV.
1. Denomina questo modulo &quot;Analizza file di società&quot;.
1. Salva lo scenario e fai clic su Esegui una volta.

   **Creare un archivio dati e una struttura dati.**

1. Aggiungi un modulo di ricerca record dell&#39;archivio dati.
1. Crea un nuovo archivio dati denominato &quot;Sincronizzazione società&quot;.
1. All’interno dell’archivio dati, crea una struttura dati denominata &quot;Sincronizzazione società (struttura)&quot;.
1. Creare quattro campi.

   + CID - L’ID società nel file CSV
   + Nome dell&#39;azienda
   + WFID - ID società Workfront
   + Data di creazione: assicurati che il tipo di dati sia date

   ![Memorizzazione dei dati Immagine 2](../12-exercises/assets/data-stores-walkthrough-2.png)

1. Fare clic su Salva nella struttura dati, quindi impostare la dimensione di archiviazione dati su 1 e salvare l&#39;archivio dati.
1. Continuando nel modulo Archivio dati, imposta un Filtro in cui il CID è uguale all’ID della società dal modulo Parse CSV (Colonna 1).
1. Fai clic su Mostra impostazioni avanzate e seleziona l&#39;opzione per &quot;continuare l&#39;esecuzione dello scenario o del percorso, anche se questo modulo restituisce senza risultati&quot;.

   ![Memorizzazione dei dati Immagine 3](../12-exercises/assets/data-stores-walkthrough-3.png)

1. Rinomina questo modulo &quot;Società corrispondenti&quot;.
1. Aggiungi un modulo di record di Workfront Search.
1. Scegliere Società come tipo di record.
1. I criteri di ricerca sono il nome dell’azienda in Workfront che corrisponde al nome dell’azienda nel file CSV.
1. Per gli output, seleziona il nome della società e l’ID.

   ![Memorizzazione dei dati Immagine 4](../12-exercises/assets/data-stores-walkthrough-4.png)

1. Fare clic su OK e rinominare questo modulo &quot;Società corrispondenti&quot;.

   **Crea percorsi diversi in base all’esistenza della società in Workfront o nell’archivio dati.**

   **Percorso di routing 1: consente di creare una società.**

1. Aggiungere un modulo router a destra del modulo record di Workfront Search.
1. Aggiungi un modulo Workfront Create Record al percorso superiore.
1. Impostare il tipo di record su Società.
1. Selezionare Nome dai campi da mappare. Mappa il campo del nome sull’output del modulo CSV Analisi (Colonna 2).
1. Rinomina questo modulo &quot;Crea società&quot;.

   ![Memorizzazione dei dati Immagine 5](../12-exercises/assets/data-stores-walkthrough-5.png)

1. Aggiungi un filtro dopo il router per creare una società solo se non è già in Workfront. Denomina &quot;Not in Workfront&quot;.
1. Imposta la condizione sull’ID dal modulo Workfront Search e non esiste.

   ![Memorizzazione dei dati Immagine 6](../12-exercises/assets/data-stores-walkthrough-6.png)

   **Prepara l&#39;aggiornamento dell&#39;archivio dati nel percorso successivo.**

1. Aggiungi un modulo di variabile Set alla fine del percorso superiore.
1. Imposta il nome della variabile su &quot;Workfront ID&quot;.
1. Imposta il valore Variable sull’ID dal modulo Create company (Crea società).
1. Rinomina questo modulo &quot;Imposta Workfront ID&quot;.

   **Percorso di routing 2 - Aggiornare l&#39;archivio dati.**

1. Crea un filtro per il percorso di indirizzamento 2. Denomina &quot;Non nell&#39;archivio dati&quot;.

1. Imposta la condizione sulla chiave dal modulo Archivio dati e non esiste.

   ![Archivio dati Immagine 7](../12-exercises/assets/data-stores-walkthrough-7.png)

1. Il primo modulo in questo percorso è il modulo della variabile Get.
1. Imposta il nome della variabile su &quot;Workfront ID&quot;.
1. Rinomina questo modulo &quot;Ottieni ID Workfront&quot;.
1. Aggiungi un altro modulo dall’app Data Store e sostituisci un record.
1. Nel campo Archivio dati, scegli Sincronizzazione società. Si tratta dell&#39;archivio dati creato in precedenza.
1. Lascia vuoto il campo Chiave .
1. Mappa il campo CID dalla colonna 1 nel modulo Analizza CSV .
1. Mappa il campo del nome della società dalla colonna 2 nel modulo CSV Analisi.
1. Mappa il campo WFID dal modulo Get Workfront ID.
1. Per il campo Data creazione, utilizzare la funzione formatDate della scheda Data e ora per formattare la data corrente come MM/GG/AAAA.

   ![Memorizzazione dei dati Immagine 8](../12-exercises/assets/data-stores-walkthrough-8.png)

1. Fai clic su OK e rinomina questo modulo &quot;Crea voce aziendale&quot;.

   **Percorso di routing 3-Sincronizza l&#39;archivio dati tra sistemi.**

1. Iniziare creando un filtro sul percorso di routing 3. Denomina &quot;Società esistente, non in archivio dati&quot;.
1. Imposta la condizione sulla chiave dal modulo di ricerca record dell&#39;archivio dati e non esiste.
1. Fai clic sul pulsante Aggiungi regola AND e specifica che il nome della società dal file CSV (Colonna 2) è uguale al nome della società che si trova nel modulo Workfront Search.

   ![Archivio dati Immagine 9](../12-exercises/assets/data-stores-walkthrough-9.png)

1. Ora aggiungi un altro modulo Aggiungi/sostituisci un record clonando quello alla fine del percorso di routing 2.
1. Trascinare il modulo clonato in posizione alla fine del percorso di routing 3. Elimina il modulo vuoto presente.
1. Fai clic sul modulo clonato. Tutti i campi devono rimanere uguali, tranne il campo WFID. Mappa dal modulo di ricerca delle aziende corrispondenti.

   ![Archivio dati Immagine 10](../12-exercises/assets/data-stores-walkthrough-10.png)

1. Fai clic su OK e rinomina questo modulo &quot;Crea voce aziendale&quot;.
