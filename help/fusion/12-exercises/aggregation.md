---
title: Esercizio sull’aggregazione
description: Scopri come aggregare più bundle di informazioni in un unico valore.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11047
thumbnail: KT11047.png
recommendations: noDisplay,catalog
exl-id: 4626b623-8b05-41be-9cfc-917e28222855
source-git-commit: f033b210268e8979ee15abe812e6ad85673eeedb
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 100%

---

# Esercizio sull’aggregazione

Scopri come aggregare più bundle di informazioni in un unico valore.

## Panoramica dell’esercizio

Utilizzando lo scenario “Introduzione all’iterazione” creato nell’ultimo esercizio, aggrega le ore pianificate per ogni attività lavorativa del progetto e invia un’e-mail con tali informazioni.

![Immagine aggregazione 1](../12-exercises/assets/aggregation-walkthrough-1.png)

## Passaggi da seguire

**Aggiungi un filtro e SOMMA le ore pianificate.**

1. Clona lo scenario “Introduzione all’iterazione” creato nell’esercizio precedente e denominarlo “Introduzione all’aggregazione.”
1. Aggiungi un filtro tra il modulo Attività di lettura progetto e il modulo Conteggio del numero di attività. Denomina il filtro “Solo le attività in esecuzione”.
1. Imposta la condizione su Numero di elementi figlio [Operatore numerico: uguale a] 0.

   ![Immagine aggregazione 2](../12-exercises/assets/aggregation-walkthrough-2.png)

1. Dopo il modulo Math casuale, aggiungi un modulo dello strumento Aggregatore numerico.
1. Imposta il modulo di origine su Attività di lettura progetto.
1. Imposta la funzione Aggrega su SOMMA.
1. Imposta il valore nel campo Lavoro dal modulo Attività di lettura progetto.
1. Rinomina questo modulo “SOMMA di tutte le ore del piano di attività”.

   ![Immagine aggregazione 3](../12-exercises/assets/aggregation-walkthrough-3.png)

   **Nota l’ombreggiatura che indica che l’aggregazione termina l’iterazione.**

   ![Immagine aggregazione 4](../12-exercises/assets/aggregation-walkthrough-4.png)

   **Invia un’e-mail con le ore aggregate.**

1. Aggiungi un modulo Invia un messaggio e-mail dall’app E-mail, dopo l’aggregatore numerico.
1. Invia l’e-mail a te stesso.
1. L’oggetto è &quot;Dettagli progetto&quot;.
1. Nel campo Contenuto, inserisci “Esiste un progetto chiamato [nome del progetto] che ha un numero totale di [risultato] ore pianificate”. Il “[nome progetto]” viene preso dal modulo Leggi un record e il “[risultato]” viene preso dal modulo aggregatore.

   ![Immagine aggregazione 5](../12-exercises/assets/aggregation-walkthrough-5.png)

1. Salva ed esegui una sola volta. Trova l’e-mail nella tua casella in entrata.

All’interno dell’iterazione, è possibile accedere ai singoli bundle. Ma al di fuori dell’iterazione, nel modulo Invia un’e-mail è possibile accedere solo ai campi aggregati.
