---
title: Introduzione ai connettori universali
description: Amplia la tua comprensione dell’utilizzo dei connettori universali REST e dell’utilizzo dei dati restituiti.
feature: Workfront Fusion
role: User
level: Beginner
kt: 11042
thumbnail: KT11042.png
source-git-commit: 1f7a4da813805691fc0e52d3ad1ea708f9e07a9a
workflow-type: tm+mt
source-wordcount: '591'
ht-degree: 0%

---


# Introduzione ai connettori universali

Amplia la tua comprensione dell’utilizzo dei connettori universali REST e dell’utilizzo dei dati restituiti.

## Panoramica sull&#39;esercizio

Utilizzando un carattere Pokemon in un foglio di calcolo, chiama l’API Poke tramite un connettore HTTP per raccogliere e pubblicare ulteriori informazioni su quel carattere.

![Introduzione ai connettori universali Immagine 1](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-1.png)

## Passaggi da seguire

**Scarica il file CSV da Workfront.**

1. Nella cartella &quot;File di esercizio di fusione&quot; di Workfront, selezionare &quot;_Fusion2020_Shipping Manifest.csv&quot; e fare clic su Dettagli documento.
1. Copia il primo numero ID dall&#39;indirizzo URL.
1. Crea un nuovo scenario in Workfront Fusion. Denomina &quot;Utilizzo di connettori universali&quot;.
1. Inizia con il modulo Scarica documento dall’app Workfront.
1. Imposta la connessione Workfront e includi l&#39;ID documento copiato dall&#39;URL Workfront.
1. Rinomina questo modulo &quot;Scarica manifesto di spedizione&quot;.

   ![Introduzione ai connettori universali Immagine 9](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-9.png)

   **Analizzare i dati del manifesto di spedizione.**

1. Aggiungi un altro modulo, selezionando Analizza CSV.
1. Imposta Analizza CSV per 11 colonne. Seleziona la casella CSV contiene intestazioni . Scegli Comma delimiterType e inserisci i dati dal modulo Scarica documento nel campo CSV.

   ![Introduzione ai connettori universali Immagine 2](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-2.png)

1. Rinomina questo modulo &quot;Analizza manifesto di spedizione&quot;.
1. Salva lo scenario e fai clic su Esegui una volta per visualizzare i dati dal file CSV nei passaggi successivi.

   **Ottieni i dati Pokemon utilizzando il connettore universale.**

1. Aggiungi un modulo HTTP Make a Request (Crea richiesta modulo).
1. Nel campo URL utilizza https://pokeapi.co/api/v2/pokemon/[Carattere], dove [Carattere] è mappato alla colonna 3 dal modulo CSV parse.
1. Selezionare la casella di controllo Analizza risposta.
1. Seleziona Mostra impostazioni avanzate e seleziona la casella accanto a &quot;Valuta tutti gli stati come errori&quot;.
1. Fai clic su OK e rinomina il modulo &quot;Ottieni informazioni Pokemon&quot;.

   **Il pannello di mappatura deve essere simile al seguente:**

   ![Introduzione ai connettori universali Immagine 3](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-3.png)

   **In questa parte dell’esercizio, desideri elaborare solo la riga 1 nel file CSV.**

1. Aggiungi un filtro prima del modulo Get Pokemon info. Denomina &quot;Solo riga 1&quot;.
1. Imposta la condizione per consentire il passaggio solo dell&#39;ID numero 1. L’ID numero 1 si trova nella riga 1 e il campo ID si trova nella colonna 1 del file CSV.

   ![Introduzione ai connettori universali Immagine 4](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-4.png)

1. Salva lo scenario.
1. Fai clic su Esegui una volta e osserva il messaggio di errore ricevuto nel modulo di richiesta HTTP Make a .

   >[!IMPORTANT]
   >
   >Nel campo URL dati di input, il nome del carattere è maiuscolo. Questo non funziona per effettuare quella chiamata API perché i nomi dei caratteri devono essere minuscoli.

   ![Introduzione ai connettori universali Immagine 5](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-5.png)

1. Utilizza il pannello di mappatura nel campo HTTP Make a request URL (Crea un URL di richiesta) per rendere il [Carattere] tutte le lettere minuscole utilizzando **Lower** funzione .

   ![Introduzione ai connettori universali Immagine 6](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-6.png)

   **Mappa le informazioni dall’API utilizzando il modulo Imposta più variabili .**

1. Aggiungi il modulo Set multiple variables dopo Get Pokemon info. Nome, altezza, peso e capacità della mappa.
1. Poiché il campo Abilities è un array, ricorda di utilizzare la funzione map per accedere al nome di ogni funzionalità dell&#39;array.

   ![Introduzione ai connettori universali Immagine 7](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-7.png)

   **Esegui lo scenario senza il filtro per individuare un altro errore.**

1. Per elaborare tutte le righe nel file CSV, elimina il filtro denominato Only row 1:

   + Fai clic sull’icona del filtro per modificarlo.
   + Elimina l’etichetta del filtro.
   + Elimina la condizione .
   + Fate clic su OK.

1. Salva lo scenario e fai clic su Esegui una volta.
1. Si verifica un errore nel modulo Get Pokemon info. Vedete che un personaggio supereroe è stato passato all&#39;API Pokemon.

   >[!NOTE]
   >
   >Nella procedura dettagliata relativa ai router verrà illustrato come risolvere questo errore creando un percorso separato per elaborare i supereroi.

   ![Introduzione ai connettori universali Immagine 8](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-8.png)