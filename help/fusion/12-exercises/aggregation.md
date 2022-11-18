---
title: Aggregazione
description: Scopri come aggregare più bundle di informazioni in un unico valore.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 11047
thumbnail: KT11047.png
exl-id: 4626b623-8b05-41be-9cfc-917e28222855
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Aggregazione

Scopri come aggregare più bundle di informazioni in un unico valore.

## Panoramica sull&#39;esercizio

Utilizzando lo scenario &quot;Introduzione all’iterazione&quot; generato nell’ultimo esercizio, aggrega le ore pianificate per ogni attività di lavoro del progetto e invia un messaggio e-mail con tali informazioni.

![Immagine di aggregazione 1](../12-exercises/assets/aggregation-walkthrough-1.png)

## Passaggi da seguire

**Aggiungi un filtro e SOMMA le ore pianificate.**

1. Clonare lo scenario &quot;Introduzione all’iterazione&quot; creato nell’esercizio precedente e denominarlo &quot;Introduzione all’aggregazione&quot;.
1. Aggiungi un filtro tra il modulo Attività del progetto di lettura e il modulo Conteggio del numero di attività. Denomina il filtro &quot;Solo attività in corso&quot;.
1. Imposta la condizione su Numero di elementi figlio [Operatore numerico: Uguale a] 0.

   ![Immagine di aggregazione 2](../12-exercises/assets/aggregation-walkthrough-2.png)

1. Dopo il modulo Matematica casuale, aggiungi un modulo di strumenti Aggregatore numerico.
1. Impostare il modulo di origine su Leggi attività del progetto.
1. Impostare la funzione Aggregate su SUM.
1. Impostare il valore sul campo Lavoro dal modulo Attività del progetto di lettura.
1. Rinomina questo modulo &quot;SOMMA di tutte le ore di pianificazione delle attività&quot;.

   ![Immagine di aggregazione 3](../12-exercises/assets/aggregation-walkthrough-3.png)

   **Osserva l’ombreggiatura che mostra che l’aggregazione termina l’iterazione.**

   ![Immagine di aggregazione 4](../12-exercises/assets/aggregation-walkthrough-4.png)

   **Invia un’e-mail con ore aggregate.**

1. Aggiungi un modulo Invia un’e-mail dall’app E-mail, dopo l’aggregatore numerico.
1. Invia l&#39;e-mail a te stesso.
1. L&#39;oggetto è &quot;Dettagli progetto&quot;.
1. Nel campo Contenuto , inserisci &quot;Esiste un progetto denominato [nome del progetto] con un numero totale di [risultato] orario previsto.&quot; &quot;[nome del progetto]&quot; è tratto dal modulo Read a Record e &quot;[risultato]&quot; è tratto dal modulo aggregatore.

   ![Immagine di aggregazione 5](../12-exercises/assets/aggregation-walkthrough-5.png)

1. Salva ed esegui una volta. Trova l’e-mail nella tua casella in entrata.

All’interno dell’iterazione, è possibile accedere ai singoli bundle. Ma al di fuori dell’iterazione, nel modulo Invia un’e-mail è possibile accedere solo ai campi aggregati.
