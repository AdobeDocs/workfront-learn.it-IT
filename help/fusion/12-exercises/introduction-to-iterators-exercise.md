---
title: Introduzione all’esercizio sugli Iteratori
description: Scopri come utilizzare le app di tipo iterazione ed eseguire azioni su ogni bundle di informazioni.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11046
thumbnail: KT11046.png
recommendations: noDisplay,noCatalog
exl-id: 8d751885-372a-4716-9542-079cc3d36caf
source-git-commit: a4e61514567ac8c2b4ad5c9ecacb87bd83947731
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 100%

---

# Introduzione all’esercizio sugli Iteratori

 Scopri come utilizzare le app di tipo iterazione ed eseguire azioni su ogni bundle di informazioni.

## Panoramica dell’esercizio

Esamina un progetto specifico in Workfront, quindi esamina tutte le attività all’interno di tale progetto. Utilizzerai il modulo dello strumento di incremento per contare il numero di attività all’interno del progetto. Infine, utilizzerai il modulo Imposta variabile per sottrarre il numero di elementi figlio dal Numero di problemi aperti per produrre un valore numerico per ciascuno dei bundle delle attività.

![Introduzione agli iteratori Immagine 1](../12-exercises/assets/introduction-to-iterators-walkthrough-1.png)

## Passaggi da seguire

**Leggi un progetto e le attività correlate.**

1. Avvia un nuovo scenario. Denominalo “Introduzione all’iterazione.”
1. Scegli Workfront come modulo trigger e Leggi un record.
1. Per il Tipo di record, scegli Progetto.
1. Per Output, scegli ID, Nome e Descrizione.
1. Nel campo ID, inserisci l’ID del progetto Northstar Fashion Exhibitors Booth dall’istanza dell’unità di test di Workfront.
1. Rinomina questo modulo “Find WF Projects.”
1. Aggiungi un altro modulo Workfront per leggere le attività relative a questo progetto. Scegli il modulo Leggi record correlati.
1. Per il Tipo di record, scegli Progetto.
1. Per l’ID del record principale, scegli l’ID dal modulo Leggi record.
1. Per Raccolte, seleziona Attività.
1. Per Output, seleziona ID, Nome, Descrizione, Numero di elementi figlio, Numero di problemi aperti e Lavoro.
1. Rinomina questo modulo “Attività del progetto di lettura.”
1. Salva lo scenario, quindi fai clic su Esegui una volta per visualizzare gli output.

   + Fai clic sulla finestra di ispezione dell’esecuzione per visualizzare un bundle come input (il progetto) e 28 bundle come output (le attività).

   **Conta ed elabora i pacchetti iterati.**

1. Aggiungi un altro modulo dopo Leggi record correlati. Scegli un modulo per gli strumenti della funzione Incremento.

   + Lascia il campo Reimposta un valore come Mai e fai clic su OK.

1. Rinomina questo modulo “Count the # of tasks.”
1. Aggiungi un modulo Imposta variabile. Imposta il nome della variabile su “Matematica casuale.”
1. Nel campo Valore variabile, sottrai il numero di elementi figlio aperti dal numero di operazioni opTasks aperte.

   **Dovrebbe essere simile al seguente:**

   ![Introduzione agli iteratori Immagine 2](../12-exercises/assets/introduction-to-iterators-walkthrough-2.png)

1. Rinomina questo modulo “Random Math.”
1. Salva lo scenario e fai clic su Esegui una volta.

Per ciascuna delle attività prodotte dal modulo iteratore Leggi record correlati, Workfront Fusion ha eseguito 28 esecuzioni. Questi 28 bundle continueranno a essere elaborati durante lo scenario a meno che non venga aggiunto un aggregatore per chiudere il ciclo.
