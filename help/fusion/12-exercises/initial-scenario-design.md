---
title: Progettazione scenario iniziale
description: Scopri alcuni suggerimenti di base per la navigazione quando accedi a Workfront Fusion per la prima volta, nonché per la creazione del primo scenario.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11038
thumbnail: KT11038.png
exl-id: 8ecf4979-f291-4788-bdaa-ab5485fb0849
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '906'
ht-degree: 0%

---

# Progettazione scenario iniziale

Scopri alcuni suggerimenti di base per la navigazione quando accedi a Workfront Fusion per la prima volta, nonché per la creazione del primo scenario.

## Panoramica dell’esercizio

Crea un nuovo progetto in Workfront per ogni riga nel file CSV dell’elenco dei progetti.

![Immagine progettazione scenario iniziale 1](../12-exercises/assets/initial-scenario-design-1.png)

## Passaggi da seguire

1. Creare una cartella nella sezione Scenario denominata &quot;Esercizi di abilitazione di Fusion&quot;.
1. Fai clic su nella cartella, quindi fai clic su Crea un nuovo scenario.

   ![Immagine progettazione scenario iniziale 2](../12-exercises/assets/initial-scenario-design-2.png)

1. Nella pagina successiva, cerca Workfront e seleziona l’app. Quindi fai clic su Continua.
1. In alto a sinistra nella schermata di Progettazione scenari, rinomina lo scenario in &quot;Progettazione scenario iniziale&quot;
1. Fai clic sul modulo trigger vuoto al centro dello schermo e seleziona l’app Workfront, quindi seleziona il modulo Scarica documento.

   **Autentica la connessione del modulo al tuo account Workfront.**

1. Per creare una connessione per la prima volta, fare clic sul pulsante Aggiungi.

   ![Immagine progettazione scenario iniziale 3](../12-exercises/assets/initial-scenario-design-3.png)

1. Assegna alla connessione un nome, ad esempio &quot;My Workfront 2020&quot;

   ![Immagine progettazione scenario iniziale 4](../12-exercises/assets/initial-scenario-design-4.png)

1. Inserisci l’URL dell’istanza di Workfront, quindi fai clic su Avanti.

   ![Immagine progettazione scenario iniziale 5](../12-exercises/assets/initial-scenario-design-5.png)

1. Inserisci la password e fai clic su Accedi.

   **Connessione stabilita. Immettere ora l&#39;ID del documento che si desidera scaricare da Workfront.**

   ![Immagine progettazione scenario iniziale 7](../12-exercises/assets/initial-scenario-design-7.png)

1. Torna a Workfront. Nella cartella &quot;File di esercizio di fusione&quot;, selezionate &quot;_Fusion2020_Project List.csv&quot; e fate clic su Dettagli documento nel pannello sinistro. Copiare il numero ID del documento dall&#39;indirizzo URL (questo è il primo numero lungo nell&#39;URL).

   ![Immagine progettazione scenario iniziale 8](../12-exercises/assets/initial-scenario-design-8.png)

1. Torna a Fusion e incolla il numero nel campo ID documento, quindi fai clic su OK.
1. Si consiglia di rinominare i moduli durante la creazione. Fai clic con il pulsante destro del mouse sul modulo Workfront e scegli Rinomina. Denomina il modulo &quot;Ottieni elenco progetti&quot;.

   **Ora stai per analizzare il file CSV appena scaricato in modo da poter accedere a ogni riga nel file. Queste informazioni verranno utilizzate quando si crea un progetto da ogni riga.**

1. Fai clic sul lato destro del modulo Workfront per aggiungere un altro modulo. Cerca l’app CSV e seleziona il modulo Parse CSV.
1. Configura il file CSV di analisi per 6 colonne; il file CSV contiene intestazioni, delimitatore virgola Tipo e inserisci Dati nel campo CSV. Quindi fate clic su OK.

   ![Immagine progettazione scenario iniziale 9](../12-exercises/assets/initial-scenario-design-9.png)

1. Rinomina questo modulo &quot;Analizza elenco progetti&quot;.
1. Nella parte inferiore di Progettazione scenari fare clic su Salva per salvare lo scenario.
1. Fai clic su Esegui una volta per visualizzare l’output.

   >[!NOTE]
   >
   >Ignora l’avviso che un trasformatore non deve essere l’ultimo modulo (questo è vero, ma non importa per questo test). Fare clic su Esegui comunque.

   ![Immagine progettazione scenario iniziale 10](../12-exercises/assets/initial-scenario-design-10.png)

1. Apri il controllo di esecuzione sul modulo CSV di analisi per visualizzare gli input e gli output del modulo. Esiste un bundle (un file CSV) come input e diversi bundle come output (un bundle per ogni riga nel file CSV). Dovrebbe essere simile al seguente:

   ![Immagine progettazione scenario iniziale 11](../12-exercises/assets/initial-scenario-design-11.png)

   **Aggiungi un modulo per creare un progetto per ogni riga nel file CSV.**

1. Aggiungi un altro modulo. Seleziona l’app Workfront e scegli il modulo Crea record.
1. Impostare il tipo di record come Progetto.

   >[!TIP]
   >
   >Per cercarla, inizia a digitare alcune lettere, ad esempio *proj*, per andare dritto a questo.

1. Quindi utilizzate Comando/Ctrl+G per trovare Nome (nome del progetto). Seleziona la casella accanto a Nome; il campo viene visualizzato di seguito.
1. Ora seleziona le caselle accanto a Data inizio pianificata e Priorità.
1. Fai clic sul campo Nome per visualizzare il pannello di mappatura. Fai clic sul campo Colonna 1 dal modulo CSV di analisi per aggiungerlo al campo Nome. Questo è il nome del progetto dal file CSV.
1. Per Data inizio pianificata, fai clic sulla Colonna 5 del modulo Analisi CSV.
1. Per Priorità, scegliere Normale dal menu a discesa.

   **Il pannello di mappatura deve essere simile al seguente:**

   ![Immagine progettazione scenario iniziale 12](../12-exercises/assets/initial-scenario-design-12.png)

1. Fare clic su OK.

   >[!NOTE]
   >
   >Se non si fa clic su OK e si torna accidentalmente alla finestra di progettazione, il lavoro non viene salvato e sarà necessario eseguire nuovamente la mappatura.

1. Fai clic con il pulsante destro del mouse sul modulo Workfront e rinominalo &quot;Create Workfront projects&quot; (Crea progetti).
1. Salva lo scenario e fai clic sul pulsante Esegui una volta.
1. Fare clic sul controllo di esecuzione in alto a destra dell&#39;ultimo modulo.

   + Vedrai che sono state eseguite 20 operazioni. Ogni operazione richiedeva un bundle, ovvero una riga, dal file CSV come un bundle di input e output, ovvero un progetto creato in Workfront. L’ID del progetto creato viene visualizzato con il bundle di output.

   ![Immagine progettazione scenario iniziale 13](../12-exercises/assets/initial-scenario-design-13.png)

   **Utilizzo delle note**

1. Le note contribuiscono a creare maggiore visibilità nella progettazione dello scenario. Per aggiungere una nota al modulo Crea progetti Workfront, fai clic con il pulsante destro del mouse e seleziona Aggiungi una nota. Viene visualizzato un pannello a destra della finestra di progettazione che consente di aggiungere una nota al modulo. Digita in &quot;Crea un progetto con nome, data di inizio pianificata e priorità mappata dal file CSV&quot;.
1. Aggiungi un’altra nota per descrivere l’azione del modulo trigger (il primo modulo Workfront).
1. Chiudete il pannello delle note facendo clic sulla X nell&#39;angolo in alto a destra.

   + Per accedere nuovamente alle note, fare clic sul pulsante note nella barra degli strumenti inferiore oppure fare clic con il pulsante destro del mouse su un modulo e aggiungere una nuova nota.
   + Le note sono ordinate in ordine cronologico inverso.
   + Una volta aggiunte le note, sul pulsante Note viene visualizzato un punto arancione.

   ![Immagine progettazione scenario iniziale 14](../12-exercises/assets/initial-scenario-design-14.png)

1. Salvare lo scenario facendo clic sul pulsante Salva nella barra degli strumenti dei controlli.
1. Puoi visualizzare i progetti creati nella tua istanza di Workfront.
