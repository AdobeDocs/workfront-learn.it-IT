---
title: Utilizzo di JSON
description: Scopri come creare e analizzare JSON all’interno di uno scenario per supportare le tue esigenze di progettazione.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11056
thumbnail: KT11056.png
exl-id: 72d5159e-72e5-4202-90de-753b3d7626de
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# Utilizzo di JSON

Scopri come creare e analizzare JSON all’interno di uno scenario per supportare le tue esigenze di progettazione.

## Panoramica dell’esercizio

Lo scopo di questo esercizio è quello di mostrare concettualmente come utilizzare le informazioni inviate in uno scenario in formato JSON, analizzandole in campi ed elementi che è possibile mappare in tutto lo scenario. Puoi quindi acquisire informazioni da tali array mappati oppure aggregarle in JSON per poi inviarle a un altro sistema che prevede che JSON sia un input di ricezione.

![Utilizzo dell’immagine json 1](../12-exercises/assets/working-with-json-walkthrough-1.png)

## Passaggi da seguire

**Crea una struttura di dati e analizza il JSON.**

1. Crea un nuovo scenario e denominalo &quot;Utilizzo dei dati ad anello JSON&quot;.
1. Per il modulo trigger, utilizza il modulo Imposta variabile.
1. Per Nome variabile, digita in &quot;Dati ad anello&quot;.
1. Per il valore Variable, copia e incolla il contenuto del documento &quot;_Donut Data - Sample JSON.rtf&quot; che si trova nella cartella Fusion Exercise Files (File di esercizio di Fusion) nell’unità di test.

   ![Utilizzo dell’immagine json 2](../12-exercises/assets/working-with-json-walkthrough-2.png)

1. Rinomina questo modulo &quot;JSON da un altro connettore&quot;.
1. Aggiungi un modulo JSON di analisi.
1. Fare clic su Aggiungi per il campo Struttura dati.
1. Seleziona il Generatore e incolla i Dati Anello - Dati JSON di esempio copiati nel campo Dati di esempio.

   ![Utilizzo dell’immagine json 3](../12-exercises/assets/working-with-json-walkthrough-3.png)

1. Fai clic su Salva, per denominare la struttura dati &quot;Dati ad anello&quot;. Quindi fai clic su Salva.
1. Mappa i dati Anello dal modulo Imposta variabile al campo stringa JSON.

   ![Utilizzo dell’immagine json 4](../12-exercises/assets/working-with-json-walkthrough-4.png)

1. Salva lo scenario, quindi fai clic su Esegui una volta per visualizzare l’output.

   **L’output del modulo JSON di analisi deve essere simile al seguente:**

   ![Utilizzo dell’immagine json 5](../12-exercises/assets/working-with-json-walkthrough-5.png)

   **Mappa su specifiche variabili di array.**

1. Aggiungi un router dopo il modulo JSON di analisi.
1. Nel percorso superiore, aggiungi un modulo Imposta variabile.
1. Per il nome della variabile, digita &quot;Tipi di batteria per ciambella&quot;.
1. Per il valore Variable, utilizzate la funzione map per ottenere i tipi di batteria dall&#39;array di batterie.

   ![Utilizzo dell’immagine json 6](../12-exercises/assets/working-with-json-walkthrough-6.png)

1. Fare clic su OK, quindi su Esegui una volta.
1. Apri il controllo di esecuzione per visualizzare il bundle di output per ciascuna delle tre operazioni, mostrando i tipi di pastella per ciascuna.

   ![Utilizzo dell’immagine json 7](../12-exercises/assets/working-with-json-walkthrough-7.png)

   **Aggrega i dati dello scenario in JSON.**

1. Nel percorso di routing inferiore, aggiungi un aggregato al modulo JSON.
1. Per il modulo di origine, scegli l’iteratore, il modulo JSON di analisi.
1. Per la struttura Dati, crea o scegli una struttura dati. Per questo esempio, utilizza i dati Anello.
1. Procedi e mappa direttamente i campi per questo esempio, come mostrato di seguito.
1. Quando si arriva al batter e topping, notare che questi sono array, quindi è necessario fare clic su Aggiungi elemento per mapparli.

   ![Utilizzo dell’immagine json 8](../12-exercises/assets/working-with-json-walkthrough-8.png)

1. Salva lo scenario e fai clic su Esegui una volta.

Osserva la finestra di ispezione dell’esecuzione per il modulo Aggrega a JSON e osserva come è stato possibile aggregare tre bundle in una singola stringa JSON. Puoi quindi inviare questa stringa ad altri sistemi che prevedono JSON.

![Utilizzo dell’immagine json 9](../12-exercises/assets/working-with-json-walkthrough-9.png)
