---
title: Progettazione iniziale dello scenario
description: Scopri alcuni suggerimenti di navigazione di base per quando accedi per la prima volta a Workfront Fusion, oltre a creare il tuo primo scenario.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 11038
thumbnail: KT11038.png
exl-id: 8ecf4979-f291-4788-bdaa-ab5485fb0849
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '906'
ht-degree: 0%

---

# Progettazione iniziale dello scenario

Scopri alcuni suggerimenti di navigazione di base per quando accedi per la prima volta a Workfront Fusion, oltre a creare il tuo primo scenario.

## Panoramica sull&#39;esercizio

Crea un nuovo progetto in Workfront per ogni riga nel file CSV dell’elenco dei progetti.

![Immagine iniziale della progettazione dello scenario 1](../12-exercises/assets/initial-scenario-design-1.png)

## Passaggi da seguire

1. Crea una cartella nella sezione Scenario denominata &quot;Esercizi di abilitazione alla fusione&quot;.
1. Fai clic su nella cartella, quindi fai clic su Crea un nuovo scenario.

   ![Immagine iniziale della progettazione dello scenario 2](../12-exercises/assets/initial-scenario-design-2.png)

1. Nella pagina successiva, cerca Workfront e seleziona l’app. Quindi fai clic su Continua.
1. In alto a sinistra della schermata di progettazione dello scenario, rinominare lo scenario in &quot;Progettazione iniziale del scenario&quot;
1. Fai clic sul modulo trigger vuoto al centro dello schermo e seleziona l’app Workfront, quindi seleziona il modulo Scarica documento .

   **Autentica la connessione del modulo all’account Workfront.**

1. Per creare una connessione per la prima volta, fare clic sul pulsante Aggiungi.

   ![Immagine iniziale della progettazione dello scenario 3](../12-exercises/assets/initial-scenario-design-3.png)

1. Assegna un nome alla connessione, ad esempio &quot;My Workfront 2020&quot;

   ![Immagine iniziale della progettazione dello scenario 4](../12-exercises/assets/initial-scenario-design-4.png)

1. Inserisci l’URL della tua istanza Workfront, quindi fai clic su Avanti.

   ![Immagine iniziale della progettazione dello scenario 5](../12-exercises/assets/initial-scenario-design-5.png)

1. Immetti la password e fai clic su Accedi.

   **Il collegamento è stabilito. A questo punto, immetti l&#39;ID documento del documento da scaricare da Workfront.**

   ![Immagine iniziale della progettazione dello scenario 7](../12-exercises/assets/initial-scenario-design-7.png)

1. Torna a Workfront. Nella cartella &quot;File di esercizio di fusione&quot;, selezionare &quot;_Fusion2020_Project List.csv&quot; e fare clic su Dettagli documento nel pannello a sinistra. Copia il numero di ID del documento dall&#39;indirizzo URL (questo è il primo numero lungo nell&#39;URL).

   ![Immagine iniziale della progettazione dello scenario 8](../12-exercises/assets/initial-scenario-design-8.png)

1. Tornare a Fusion e incollare il numero nel campo ID documento e fare clic su OK.
1. È consigliabile rinominare i moduli durante la loro creazione. Fare clic con il pulsante destro del mouse sul modulo Workfront e scegliere Rinomina. Denomina il modulo &quot;Ottieni elenco progetti&quot;.

   **Ora analizzerai il file CSV appena scaricato in modo da poter accedere a ogni riga del file. Queste informazioni vengono utilizzate quando crei un progetto da ogni riga.**

1. Fai clic sul lato destro del modulo Workfront per aggiungere un altro modulo. Cerca l’app CSV e seleziona il modulo Analizza CSV .
1. Imposta Parse CSV per 6 colonne, CSV contiene intestazioni, Comma delimiterType e inserisci i dati nel campo CSV. Quindi fare clic su OK.

   ![Immagine iniziale della progettazione dello scenario 9](../12-exercises/assets/initial-scenario-design-9.png)

1. Rinomina questo modulo &quot;Analizza elenco progetti&quot;.
1. Nella parte inferiore della finestra di progettazione dello scenario, fare clic su Salva per salvare lo scenario.
1. Fai clic su Esegui una volta per visualizzare l’output.

   >[!NOTE]
   >
   >Ignorare l&#39;avviso secondo cui un trasformatore non deve essere l&#39;ultimo modulo (questo è vero, ma non ha importanza per questo test). Fai clic su Esegui comunque.

   ![Immagine iniziale di progettazione dello scenario 10](../12-exercises/assets/initial-scenario-design-10.png)

1. Apri la finestra di ispezione di esecuzione del modulo Parse CSV per visualizzare gli input e gli output del modulo. C&#39;è un bundle (un file CSV) come input e diversi bundle come output (un bundle per ogni riga nel file CSV). Dovrebbe assomigliare a questo:

   ![Immagine iniziale di progettazione dello scenario 11](../12-exercises/assets/initial-scenario-design-11.png)

   **Aggiungi un modulo per creare un progetto per ogni riga nel file CSV.**

1. Aggiungi un altro modulo. Seleziona l’app Workfront e scegli il modulo Crea record .
1. Imposta il tipo di record come Progetto.

   >[!TIP]
   >
   >Cerca iniziando a digitare alcune lettere, ad esempio *proj*, per andare subito.

1. Quindi premi Cmd/Ctrl+G per trovare Nome (nome del progetto). Selezionare la casella accanto a Nome; il campo viene visualizzato di seguito.
1. Ora seleziona le caselle accanto a Data inizio pianificata e Priorità.
1. Fai clic nel campo Nome per visualizzare il pannello di mappatura. Fai clic sul campo Colonna 1 del modulo Analisi CSV per aggiungerlo al campo Nome . Questo è il nome del progetto dal file CSV.
1. Per la data di inizio pianificata, fai clic su Colonna 5 nel modulo Analizza CSV .
1. Per Priorità, scegliere Normale dal menu a discesa.

   **Il pannello di mappatura deve essere simile al seguente:**

   ![Immagine iniziale di progettazione dello scenario 12](../12-exercises/assets/initial-scenario-design-12.png)

1. Fate clic su OK.

   >[!NOTE]
   >
   >Se non si fa clic su OK e si fa clic accidentalmente sul designer, il lavoro non viene salvato e sarà necessario eseguire nuovamente la mappatura.

1. Fai clic con il pulsante destro del mouse sul modulo Workfront e rinominalo &quot;Crea progetti Workfront&quot;.
1. Salva lo scenario e fai clic sul pulsante Esegui una volta .
1. Fai clic sull’ispettore di esecuzione in alto a destra dell’ultimo modulo.

   + Vedrai 20 operazioni eseguite. Ciascuna operazione ha preso un bundle, il che significa una riga, dal file CSV come input e output un bundle, che era un progetto creato in Workfront. L&#39;ID progetto del progetto creato viene visualizzato con il bundle di output.

   ![Immagine iniziale della progettazione dello scenario 13](../12-exercises/assets/initial-scenario-design-13.png)

   **Utilizzo delle note**

1. Le note aiutano a creare una maggiore visibilità nella progettazione dello scenario. Per aggiungere una nota al modulo Crea progetti Workfront, fai clic con il pulsante destro del mouse e seleziona Aggiungi una nota. Viene visualizzato un pannello a destra della finestra di progettazione, che consente di aggiungere una nota al modulo. Digita &quot;Crea un progetto con Nome, Data inizio pianificata e Priorità mappate dal file CSV&quot;.
1. Aggiungi un’altra nota per descrivere l’attività del modulo trigger (il primo modulo Workfront).
1. Per chiudere il pannello delle note, fai clic sulla X nell’angolo in alto a destra.

   + Accedi nuovamente alle note facendo clic sul pulsante delle note nella barra degli strumenti inferiore o facendo clic con il pulsante destro del mouse su un modulo e aggiungendo una nuova nota.
   + Le note sono ordinate in ordine cronologico inverso.
   + Una volta aggiunte le note, sul pulsante Note viene visualizzato un punto arancione.

   ![Immagine iniziale di progettazione dello scenario 14](../12-exercises/assets/initial-scenario-design-14.png)

1. Salvare lo scenario facendo clic sul pulsante Salva nella barra degli strumenti dei controlli.
1. Puoi visualizzare i progetti creati nella tua istanza Workfront.
