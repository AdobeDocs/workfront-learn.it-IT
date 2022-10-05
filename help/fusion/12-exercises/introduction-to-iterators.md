---
title: Introduzione agli iteratori
description: Scopri come utilizzare le app di tipo iterazione ed eseguire azioni su ogni bundle di informazioni.
feature: Workfront Fusion
role: User
level: Beginner
kt: 11046
thumbnail: KT11046.png
source-git-commit: f367e016498d5c1814cab79e19e6e9001db2851f
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 0%

---


# Introduzione agli iteratori

Scopri come utilizzare le app di tipo iterazione ed eseguire azioni su ogni bundle di informazioni.

## Panoramica sull&#39;esercizio

Osserva un progetto specifico in Workfront, quindi osserva tutte le attività all’interno del progetto. Il modulo dello strumento di incremento verrà utilizzato per contare il numero di attività all’interno del progetto. Infine, utilizzerai il modulo Imposta variabile per sottrarre il Numero di elementi figlio dal Numero di problemi aperti per produrre un valore numerico per ciascuno dei bundle di attività.

![Introduzione agli iteratori Immagine 1](../12-exercises/assets/introduction-to-iterators-walkthrough-1.png)

## Passaggi da seguire

**Leggi un progetto e le attività correlate.**

1. Inizia un nuovo scenario. Denominalo &quot;Introduzione all’iterazione&quot;.
1. Scegli Workfront come modulo trigger, leggi un record.
1. Per Tipo di record, scegliere Progetto.
1. Per Output, scegli ID, nome e descrizione.
1. Nel campo ID, inserisci l&#39;ID progetto del progetto Northstar Fashion Exhibitors Booth dall&#39;istanza dell&#39;unità di prova Workfront.
1. Rinomina questo modulo &quot;Trova progetti WF&quot;.
1. Aggiungi un altro modulo Workfront per leggere le attività correlate a questo progetto. Scegliere il modulo Leggi record correlati.
1. Per Tipo di record, scegliere Progetto.
1. Per l&#39;ID record padre, scegli l&#39;ID dal modulo Leggi un record .
1. Per Raccolte, selezionare Attività.
1. Per Output, selezionare ID, Nome, Descrizione, Numero di elementi figlio, Numero di problemi aperti e Lavoro.
1. Rinomina questo modulo &quot;Leggi le attività del progetto&quot;.
1. Salva lo scenario, quindi fai clic su Esegui una volta per visualizzare gli output.

   + Fai clic sull’ispettore di esecuzione e viene visualizzato un bundle come input (il progetto) e 28 bundle come output (le attività).

   **Conteggio ed elaborazione dei bundle ripetuti.**

1. Aggiungi un altro modulo dopo Leggi record correlati. Scegliere un modulo di strumenti di funzione Increment.

   + Lasciare il campo Reimposta un valore come Mai e fare clic su OK.

1. Rinomina questo modulo &quot;Conta il numero di attività&quot;.
1. Aggiungi un modulo di variabile Set . Imposta il nome della variabile su &quot;Matematica casuale&quot;.
1. Nel campo Valore variabile, sottrarre il numero di elementi secondari aperti dal numero di operazioni opTasks aperte.

   **Dovrebbe essere così:**

   ![Introduzione agli iteratori Immagine 2](../12-exercises/assets/introduction-to-iterators-walkthrough-2.png)

1. Rinomina questo modulo &quot;Matematica casuale&quot;.
1. Salva lo scenario e fai clic su Esegui una volta.

Per ciascuna delle attività prodotte dal modulo di iteratore Read Related Records, Workfront Fusion ha eseguito 28 esecuzioni. Questi 28 bundle continueranno ad essere elaborati in tutto lo scenario a meno che non venga aggiunto un aggregatore per chiudere il ciclo.