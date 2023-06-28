---
title: Aaggregazione
description: Scopri come aggregare più bundle di informazioni in un unico valore.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11047
thumbnail: KT11047.png
exl-id: 4626b623-8b05-41be-9cfc-917e28222855
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 0%

---

# Aaggregazione

Scopri come aggregare più bundle di informazioni in un unico valore.

## Panoramica dell’esercizio

Utilizzando lo scenario &quot;Introduzione all’iterazione&quot; creato nell’ultimo esercizio, aggrega le ore pianificate per ogni attività lavorativa del progetto e invia un’e-mail con tali informazioni.

![Immagine aggregazione 1](../12-exercises/assets/aggregation-walkthrough-1.png)

## Passaggi da seguire

**Aggiungi un filtro e SOMMA le ore pianificate.**

1. Clonare lo scenario &quot;Introduzione all&#39;iterazione&quot; creato nell&#39;esercizio precedente e denominarlo &quot;Introduzione all&#39;aggregazione&quot;.
1. Aggiungi un filtro tra il modulo Attività di Leggi progetto e il modulo Conteggia il numero di attività. Denomina il filtro &quot;Solo le attività in esecuzione&quot;.
1. Imposta la condizione su Numero di elementi figlio [Operatore numerico: uguale a] 0.

   ![Immagine aggregazione 2](../12-exercises/assets/aggregation-walkthrough-2.png)

1. Dopo il modulo Math casuale, aggiungere un modulo dello strumento Aggregatore numerico.
1. Impostare il modulo di origine su Attività di lettura progetto.
1. Impostare la funzione Aggregate su SUM.
1. Impostare il valore nel campo Lavoro dal modulo Attività di lettura progetto.
1. Rinominare questo modulo &quot;SOMMA di tutte le ore del piano di attività&quot;.

   ![Immagine aggregazione 3](../12-exercises/assets/aggregation-walkthrough-3.png)

   **Si noti l&#39;ombreggiatura che indica che l&#39;aggregazione termina l&#39;iterazione.**

   ![Immagine aggregazione 4](../12-exercises/assets/aggregation-walkthrough-4.png)

   **Invia un’e-mail con ore aggregate.**

1. Aggiungi un modulo Invia un messaggio e-mail dall’app E-mail, dopo l’aggregatore numerico.
1. Invia l’e-mail a te stesso.
1. L&#39;oggetto è &quot;Dettagli progetto&quot;.
1. Nel campo Contenuto, inserisci &quot;Esiste un progetto denominato [nome progetto] che ha un numero totale di [risultato] ore pianificate.&quot; La &quot;[nome progetto]&quot; viene preso dal modulo Read a Record e &quot;[risultato]&quot; viene preso dal modulo aggregatore.

   ![Immagine aggregazione 5](../12-exercises/assets/aggregation-walkthrough-5.png)

1. Salva ed esegui una sola volta. Trova l’e-mail nella tua casella in entrata.

All’interno dell’iterazione, è possibile accedere ai singoli bundle. Ma al di fuori dell’iterazione, nel modulo Send an email (Invia un’e-mail) è possibile accedere solo ai campi aggregati.
