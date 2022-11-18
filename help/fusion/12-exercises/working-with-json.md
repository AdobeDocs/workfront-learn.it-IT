---
title: Utilizzo di JSON
description: Scopri come creare e analizzare JSON in uno scenario per soddisfare le tue esigenze di progettazione.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 11056
thumbnail: KT11056.png
exl-id: 72d5159e-72e5-4202-90de-753b3d7626de
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# Utilizzo di JSON

Scopri come creare e analizzare JSON in uno scenario per soddisfare le tue esigenze di progettazione.

## Panoramica sull&#39;esercizio

Lo scopo di questo esercizio è quello di mostrare concettualmente come utilizzare le informazioni inviate in uno scenario in formato JSON, analizzandole in campi ed elementi mappabili in tutto lo scenario. Quindi puoi acquisire informazioni da tali array mappati o aggregare le informazioni in JSON per poi essere inviate a un altro sistema che prevede JSON come input di ricezione.

![Utilizzo dell’immagine 1 di json](../12-exercises/assets/working-with-json-walkthrough-1.png)

## Passaggi da seguire

**Crea una struttura di dati e analizza JSON.**

1. Crea un nuovo scenario e denominalo &quot;Utilizzo dei dati di Donut JSON&quot;.
1. Per il modulo trigger, utilizza il modulo Imposta variabile .
1. Per il nome della variabile, digita &quot;Dati Anello&quot;.
1. Per il valore Variable, copia e incolla il contenuto del documento &quot;_Donut Data - Sample JSON.rtf&quot; che si trova nella cartella Fusion Experience Files nell&#39;unità di test.

   ![Utilizzo dell&#39;immagine 2 di json](../12-exercises/assets/working-with-json-walkthrough-2.png)

1. Rinomina questo modulo &quot;JSON da un altro connettore.&quot;
1. Aggiungi un modulo Parse JSON .
1. Fare clic su Aggiungi per il campo Struttura dati.
1. Seleziona il Generatore e incolla i dati JSON campione Donut Data copiati nel campo Sample data .

   ![Utilizzo di json Image 3](../12-exercises/assets/working-with-json-walkthrough-3.png)

1. Fai clic su Salva, denominando la struttura dati &quot;Dati di Donut&quot;. Quindi fai clic su Salva.
1. Mappa i dati Anello dal modulo Imposta variabile al campo stringa JSON.

   ![Utilizzo dell&#39;immagine 4 di json](../12-exercises/assets/working-with-json-walkthrough-4.png)

1. Salva lo scenario, quindi fai clic su Esegui una volta per visualizzare l&#39;output.

   **L’output del modulo Parse JSON deve essere simile al seguente:**

   ![Utilizzo dell&#39;immagine 5 di json](../12-exercises/assets/working-with-json-walkthrough-5.png)

   **Mappatura su variabili di array specifiche.**

1. Aggiungi un router dopo il modulo Parse JSON.
1. Nel percorso superiore, aggiungi un modulo di variabile Set .
1. Per il nome della variabile, digitare &quot;Tipi di batter per ciambella&quot;.
1. Per il valore Variable, utilizza la funzione map per ottenere i tipi di batter dall’array Batters.

   ![Utilizzo dell&#39;immagine 6 di json](../12-exercises/assets/working-with-json-walkthrough-6.png)

1. Fare clic su OK, quindi su Esegui una volta.
1. Aprire l&#39;ispettore di esecuzione per visualizzare il bundle di output per ciascuna delle tre operazioni, mostrando i tipi di batter per ciascuna.

   ![Utilizzo dell&#39;immagine 7 di json](../12-exercises/assets/working-with-json-walkthrough-7.png)

   **Aggrega dati di scenario in JSON.**

1. Nel percorso di indirizzamento inferiore, aggiungi un Aggregate al modulo JSON.
1. Per il modulo Sorgente, scegli l’iteratore, il modulo Parse JSON.
1. Per la struttura Dati, creare o scegliere una struttura dati qualsiasi. Per questo esempio, utilizza i dati Anello .
1. Esegui la mappatura dei campi direttamente per questo esempio, come mostrato di seguito.
1. Quando si arriva a batter e topping, notare che questi sono array, quindi è necessario fare clic su Aggiungi elemento per mapparli.

   ![Utilizzo dell&#39;immagine json 8](../12-exercises/assets/working-with-json-walkthrough-8.png)

1. Salva lo scenario e fai clic su Esegui una volta.

Osserva l’ispettore di esecuzione per il modulo Aggregate to JSON e osserva come sei stato in grado di aggregare tre bundle in una singola stringa JSON. Puoi quindi inviare questa stringa ad altri sistemi che si aspettano JSON.

![Utilizzo di json Image 9](../12-exercises/assets/working-with-json-walkthrough-9.png)
