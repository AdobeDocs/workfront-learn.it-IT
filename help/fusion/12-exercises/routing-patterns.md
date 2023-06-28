---
title: Modelli di instradamento
description: Rafforza il concetto di route e route di fallback senza dover gestire altre API.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11044
thumbnail: KT11044.png
exl-id: d8218115-5180-4e64-8ec1-d2d6afc88d23
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 0%

---

# Modelli di instradamento

Rafforza il concetto di route e route di fallback senza dover gestire altre API.

## Panoramica dell’esercizio

Utilizza il modulo Imposta variabile per inviare un numero attraverso più percorsi e vedere come si comportano i filtri e i fallback durante il routing.

![Modelli di indirizzamento Immagine 1](../12-exercises/assets/routing-patterns-walkthrough-1.png)

## Passaggi da seguire

1. Crea un nuovo scenario e chiamalo &quot;Indirizzamento di pattern e fallback&quot;.
1. Per il trigger, aggiungi il modulo dello strumento Imposta variabile. Inserire &quot;Il mio numero&quot; per il nome della variabile, lasciare la durata della variabile come un ciclo e impostare il campo Variabile su &quot;75&quot;.

   ![Modelli di indirizzamento Immagine 2](../12-exercises/assets/routing-patterns-walkthrough-2.png)

1. Aggiungi un altro modulo e scegli il modulo Router. Per entrambi i tracciati, selezionate lo strumento funzione Incremento (Increment) e fate clic su OK senza apportare alcuna modifica per ciascuno di essi.

   + Per il primo percorso, crea un filtro, chiamalo &quot;Meno di 100&quot; e imposta la condizione su [Il mio numero] Meno di cento.

   + Per il secondo percorso, crea un filtro, denominalo &quot;Meno di 1000&quot; e imposta la condizione su [Il mio numero] Meno di mille. Assicurati di utilizzare l’operatore Numerico per entrambi.

   ![Modelli di indirizzamento Immagine 3](../12-exercises/assets/routing-patterns-walkthrough-3.png)

   ![Modelli di indirizzamento Immagine 4](../12-exercises/assets/routing-patterns-walkthrough-4.png)

1. Fai clic su Esegui una volta e osserva il bundle passare lungo il percorso &quot;Meno di 100&quot;.
1. Quindi imposta il campo del modulo Variabile su 950 ed Esegui di nuovo. Guardate come scorre lungo il secondo percorso.
1. Fare clic sul router e aggiungere un altro percorso. Aggiungete il modulo dello strumento della funzione Incrementa (Increment). Per il filtro, fare clic sulla casella di controllo &quot;Percorso di fallback&quot;. Osserva come la freccia che punta a quel percorso cambia in un punto di inserimento, indicando che si tratta della route di fallback.

   ![Modelli di indirizzamento Immagine 5](../12-exercises/assets/routing-patterns-walkthrough-5.png)

1. Imposta il numero della variabile su 9500 ed Esegui una volta. Poiché il numero non è inferiore a 100 o a 1000, il bundle viaggia lungo la route di fallback.

Se aggiungete un altro tracciato con un modulo utensile della funzione Incremento ma non impostate alcun filtro, cosa accade quando fate di nuovo clic su Esegui (Run)? Un bundle passerà mai lungo la rotta di fallback con la quarta rotta aggiunta?

+ No, perché senza filtro impostato, ogni bundle seguirà sempre questo percorso invece del percorso di fallback.
