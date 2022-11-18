---
title: Pattern di routing
description: Potenzia il concetto di route di routing e fallback senza dover trattare con altre API.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 11044
thumbnail: KT11044.png
exl-id: d8218115-5180-4e64-8ec1-d2d6afc88d23
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 0%

---

# Pattern di routing

Potenzia il concetto di route di routing e fallback senza dover trattare con altre API.

## Panoramica sull&#39;esercizio

Utilizza il modulo Imposta variabile per inviare un numero attraverso più percorsi per vedere come si comportano i filtri e i fallback durante il routing.

![Pattern di routing Immagine 1](../12-exercises/assets/routing-patterns-walkthrough-1.png)

## Passaggi da seguire

1. Crea un nuovo scenario e chiamalo &quot;Pattern di routing e fallback&quot;.
1. Per il trigger, aggiungi il modulo di strumento Imposta variabile . Inserire &quot;Il mio numero&quot; per il nome della variabile, lasciare la durata della variabile come un ciclo e impostare il campo Variabile su &quot;75&quot;.

   ![Pattern di routing Immagine 2](../12-exercises/assets/routing-patterns-walkthrough-2.png)

1. Aggiungi un altro modulo e scegli il modulo Router. Per entrambi i percorsi, scegli lo strumento Incrementa funzione e fai clic su OK senza apportare alcuna modifica per ciascuno di essi.

   + Per il primo percorso, crea un filtro, rinominalo &quot;Less than 100&quot; e imposta la condizione su [Numero personale] Meno di 100.

   + Per il secondo percorso, crea un filtro, denominalo &quot;Less than 1000&quot; e imposta la condizione su [Numero personale] Meno di 1000. Assicurati di utilizzare l’operatore Numerico per entrambi.

   ![Pattern di routing Immagine 3](../12-exercises/assets/routing-patterns-walkthrough-3.png)

   ![Pattern di routing Immagine 4](../12-exercises/assets/routing-patterns-walkthrough-4.png)

1. Fai clic su Esegui una volta e guarda il bundle passare il percorso &quot;Meno di 100&quot;.
1. Quindi, cambia il campo del modulo Imposta variabile a 950 ed Esegui di nuovo. Guarda che scorre lungo il secondo percorso.
1. Fare clic sul router e aggiungere un altro percorso. Aggiungi il modulo dello strumento della funzione Increment . Per il filtro, fai clic sulla casella di controllo &quot;Il percorso di fallback&quot;. Osserva come la freccia che punta a quel percorso si trasforma in un accento circonflesso, indicando che si tratta del percorso di fallback.

   ![Pattern di routing Immagine 5](../12-exercises/assets/routing-patterns-walkthrough-5.png)

1. Cambia il numero della variabile Set a 9500 ed Esegui una volta. Poiché il numero non è inferiore a 100 o meno di 1000, il bundle viaggia lungo il percorso di fallback.

Se aggiungi un altro percorso con un modulo strumento di funzione Increment, ma non imposta alcun filtro, cosa succede quando fai di nuovo clic su Esegui? Un bundle andrà mai lungo il percorso di fallback con il quarto percorso aggiunto?

+ No, perché senza set di filtri, ogni bundle andrà sempre in questo percorso invece del percorso di fallback.
