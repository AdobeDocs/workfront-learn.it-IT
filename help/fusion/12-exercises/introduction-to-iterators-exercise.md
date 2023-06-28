---
title: Introduzione all’esercizio Iteratori
description: Scopri come utilizzare le app di tipo iterazione ed eseguire azioni su ogni pacchetto di informazioni.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11046
thumbnail: KT11046.png
exl-id: 8d751885-372a-4716-9542-079cc3d36caf
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 0%

---

# Introduzione agli iteratori

Scopri come utilizzare le app di tipo iterazione ed eseguire azioni su ogni pacchetto di informazioni.

## Panoramica dell’esercizio

Osserva un progetto specifico in Workfront, quindi osserva tutte le attività all’interno di quel progetto. Il modulo dello strumento Incrementa consente di contare il numero di attività all&#39;interno del progetto. Infine, utilizzerai il modulo Imposta variabile per sottrarre il Numero di elementi figlio dal Numero di problemi aperti per produrre un valore numerico per ciascuno dei bundle di attività.

![Introduzione agli iteratori Immagine 1](../12-exercises/assets/introduction-to-iterators-walkthrough-1.png)

## Passaggi da seguire

**Leggi un progetto e le attività correlate.**

1. Inizia un nuovo scenario. Denominalo &quot;Introduzione all’iterazione&quot;.
1. Scegli Workfront come modulo trigger e leggi un record.
1. In Tipo di record, scegliere Progetto.
1. Per Output, scegliete ID, Nome e Descrizione.
1. Nel campo ID, inserisci l’ID del progetto dello stand Northstar Fashion Exhibitors dalla tua istanza dell’unità di test di Workfront.
1. Rinominare questo modulo &quot;Find WF Projects&quot; (Trova progetti WF).
1. Aggiungi un altro modulo Workfront per leggere le attività relative a questo progetto. Scegliere il modulo Leggi record correlati.
1. In Tipo di record, scegliere Progetto.
1. Per l&#39;ID record padre, scegliere l&#39;ID dal modulo Leggi record.
1. Per Raccolte, selezionare Attività.
1. Per Output, selezionare ID, Nome, Descrizione, Numero di figli, Numero di problemi aperti e Lavoro.
1. Rinomina questo modulo &quot;Attività del progetto di lettura&quot;.
1. Salva lo scenario, quindi fai clic su Esegui una volta per visualizzare gli output.

   + Fai clic sulla finestra di ispezione dell’esecuzione per visualizzare un bundle come input (il progetto) e 28 bundle come output (le attività).

   **Contare ed elaborare i bundle iterati.**

1. Aggiungi un altro modulo dopo Leggi record correlati. Scegliete un modulo per gli strumenti della funzione Incrementa.

   + Lasciare il campo Reimposta un valore come Mai e fare clic su OK.

1. Rinomina questo modulo &quot;Conteggio del numero di attività&quot;.
1. Aggiungi un modulo Imposta variabile. Imposta il nome della variabile su &quot;Random Math&quot; (Matematica casuale).
1. Nel campo Valore variabile, sottrarre il numero di elementi figlio aperti dal numero di operazioni opTasks aperte.

   **Dovrebbe essere simile al seguente:**

   ![Introduzione agli iteratori Immagine 2](../12-exercises/assets/introduction-to-iterators-walkthrough-2.png)

1. Rinomina questo modulo &quot;Random Math&quot; (Matematica casuale).
1. Salva lo scenario e fai clic su Esegui una volta.

Per ciascuna delle attività prodotte dal modulo iteratore Read Related Records, Workfront Fusion ha eseguito 28 esecuzioni. Questi 28 bundle continueranno a essere elaborati durante lo scenario a meno che non venga aggiunto un aggregatore per chiudere il loop.
