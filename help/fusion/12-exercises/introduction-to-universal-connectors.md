---
title: Esercizio sull’introduzione ai connettori universali
description: Approfondisci le tue conoscenze sull’utilizzo dei connettori universali REST e sull’utilizzo dei dati restituiti.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11042
thumbnail: KT11042.png
recommendations: noDisplay,noCatalog
exl-id: eb442c3e-26f3-44b7-9937-ed4eeba39fb1
source-git-commit: a4e61514567ac8c2b4ad5c9ecacb87bd83947731
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 100%

---

# Esercizio sull’introduzione ai connettori universali

Approfondisci le tue conoscenze sull’utilizzo dei connettori universali REST e sull’utilizzo dei dati restituiti.

## Panoramica dell’esercizio

Utilizzando un carattere Pokemon in un foglio di calcolo, richiama l’API Poke tramite un connettore HTTP per raccogliere e pubblicare ulteriori informazioni su tale carattere.

![Introduzione ai connettori universali Immagine 1](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-1.png)

## Passaggi da seguire

**Scarica il file CSV da Workfront.**

1. Nella cartella &quot;Fusion Exercise Files&quot; di Workfront, seleziona &quot;_Fusion2020_Shipping Manifest.csv&quot; e fai clic su Dettagli documento.
1. Copia il primo numero ID dall’indirizzo URL.
1. Crea un nuovo scenario in Workfront Fusion. Denominalo &quot;Utilizzo di connettori universali&quot;.
1. Inizia con il modulo Scarica documento dall’app Workfront.
1. Configura la connessione Workfront e includi l’ID documento copiato dall’URL di Workfront.
1. Rinomina questo modulo &quot;Scarica manifesto di spedizione&quot;.

   ![Introduzione ai connettori universali Immagine 9](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-9.png)

   **Analizza i dati del manifesto di spedizione.**

1. Aggiungi un altro modulo, selezionando Analizza CSV.
1. Imposta Analizza CSV per 11 colonne. Verifica se la casella CSV contiene intestazioni. Scegli il tipo di delimitatore virgola e inserisci i dati del modulo Scarica documento nel campo CSV.

   ![Introduzione ai connettori universali Immagine 2](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-2.png)

1. Rinomina questo modulo &quot;Analizza manifesto di spedizione&quot;.
1. Salva lo scenario e fai clic su Esegui una volta in modo da visualizzare i dati dal file CSV nei passaggi successivi.

   **Ottieni i dati Pokemon utilizzando il connettore universale.**

1. Aggiungi un modulo HTTP Crea una richiesta.
1. Nel campo URL utilizza `https://pokeapi.co/api/v2/pokemon/[Character]`, dove [Carattere] è mappato alla colonna 3 dal modulo Analizza CSV.
1. Seleziona la casella di controllo Analizza risposta.
1. Seleziona Mostra impostazioni avanzate, quindi seleziona la casella accanto a &quot;Valuta tutti gli stati come errori&quot;.
1. Fai clic su OK e rinomina il modulo &quot;Ottieni informazioni Pokemon&quot;.

   **Il pannello di mappatura dovrebbe essere simile al seguente:**

   ![Introduzione ai connettori universali Immagine 3](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-3.png)

   **In questa parte dell’esercizio, desideri elaborare solo la riga 1 nel file CSV.**

1. Aggiungi un filtro prima del modulo informativo Ottieni Pokemon. Denominalo “Solo riga 1”.
1. Imposta la condizione per consentire il passaggio solo dell’ID numero 1. L’ID numero 1 si trova nella riga 1 e il campo ID si trova nella colonna 1 del file CSV.

   ![Introduzione ai connettori universali Immagine 4](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-4.png)

1. Salva lo scenario.
1. Fai clic su Esegui una volta e osserva il messaggio di errore ricevuto nel modulo HTTP Crea una richiesta.

   >[!IMPORTANT]
   >
   >Nota che nel campo URL dei dati di input il nome del carattere è in maiuscolo. Questa operazione non funziona per effettuare tale chiamata API perché i nomi dei caratteri devono essere minuscoli.

   ![Introduzione ai connettori universali Immagine 5](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-5.png)

1. Utilizza il pannello di mappatura nel campo HTTP Crea un URL di richiesta per rendere il campo [Carattere] tutto in lettere minuscole utilizzando la funzione **lower**.

   ![Introduzione ai connettori universali Immagine 6](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-6.png)

   **Mappa le informazioni dall’API utilizzando il modulo Imposta più variabili.**

1. Aggiungi il modulo Imposta più variabili dopo Ottieni informazioni su Pokemon. Nome mappa, altezza, peso e capacità.
1. Poiché il campo Abilità è un array, ricorda di utilizzare la funzione di mappatura per accedere al nome di ogni capacità nell’array.

   ![Introduzione ai connettori universali Immagine 7](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-7.png)

   **Esegui lo scenario senza il filtro per individuare un altro errore.**

1. Per elaborare tutte le righe del file CSV, elimina il filtro Solo riga 1:

   + Fai clic sull’icona del filtro per modificarlo.
   + Elimina l’etichetta del filtro.
   + Elimina la condizione.
   + Fai clic su OK.

1. Salva lo scenario e fai clic su Esegui una volta.
1. Si verifica un errore nel modulo Ottieni informazioni Pokemon. Vedi che un personaggio supereroe è stato passato all’API Pokemon.

   >[!NOTE]
   >
   >Nella procedura dettagliata Routers verrà illustrato come risolvere questo errore creando un percorso separato per l’elaborazione dei supereroi.

   ![Introduzione ai connettori universali Immagine 8](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-8.png)
