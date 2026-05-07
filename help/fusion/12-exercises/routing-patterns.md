---
title: Esercizio sui modelli di indirizzamento
description: Rafforza il concetto di instradamento e percorso di fallback senza dover gestire altre API.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11044
thumbnail: KT11044.png
recommendations: noDisplay,catalog
exl-id: d8218115-5180-4e64-8ec1-d2d6afc88d23
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: c3a155b4-a54b-4a82-a3d2-c8f0f971673e
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-06T16:42:16.496Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 361
ht-degree: 100%

---

# Esercizio sui modelli di indirizzamento

Rafforza il concetto di instradamento e percorso di fallback senza dover gestire altre API.

## Panoramica dell’esercizio

Utilizza il modulo Imposta variabile per inviare un numero attraverso più percorsi e vedere come si comportano i filtri e i fallback durante l’indirizzamento.

![Immagine 1 di Pattern di instradamento](../12-exercises/assets/routing-patterns-walkthrough-1.png)

## Passaggi da seguire

1. Crea un nuovo scenario e chiamalo “Pattern di instradamento e fallback”.
1. Per il trigger, aggiungi il modulo dello strumento Set Variable (Imposta variabile). Inserisci “Il mio numero” come nome della variabile, lascia la durata della variabile impostata su un ciclo e imposta il valore della variabile su “75”.

   ![Immagine 2 di Pattern di instradamento](../12-exercises/assets/routing-patterns-walkthrough-2.png)

1. Aggiungi un altro modulo e scegli il modulo Router (Instradamento). Per entrambi i percorsi, seleziona lo strumento Increment function (Funzione incremento) e fai clic su OK senza apportare alcuna modifica per ciascuno di essi.

   + Per il primo percorso, crea un filtro, chiamalo “Meno di 100” e imposta la condizione su [Il mio numero] Less than (Meno di) 100.

   + Per il secondo percorso, crea un filtro, chiamalo “Meno di 1000” e imposta la condizione su [Il mio numero] Less than (Meno di) 1000. Assicurati di utilizzare l’operatore numerico per entrambi.

   ![Immagine 3 di Pattern di instradamento](../12-exercises/assets/routing-patterns-walkthrough-3.png)

   ![Immagine 4 di Pattern di instradamento](../12-exercises/assets/routing-patterns-walkthrough-4.png)

1. Fai clic su Run once (Esegui una volta) e osserva il bundle passare lungo il percorso “Meno di 100”.
1. Quindi modifica il campo del modulo Set Variable (Imposta variabile) su 950 e seleziona di nuovo Run once (Esegui una volta). Guarda come scorre lungo il secondo percorso.
1. Fai clic sul router e aggiungi un altro percorso. Aggiungi il modulo dello strumento Increment function (Funzione incremento). Per il filtro, fai clic sulla casella di controllo “The fallback route” (Il percorso di fallback). Osserva come la freccia che punta a quel percorso cambia in un punto di inserimento, indicando che si tratta del percorso di fallback.

   ![Pattern di indirizzamento Immagine 5](../12-exercises/assets/routing-patterns-walkthrough-5.png)

1. Modifica il numero della variabile Imposta su 9500 ed Esegui una volta. Poiché il numero non è inferiore a 100 o a 1000, il bundle viaggia lungo il percorso di fallback.

Se aggiungi un altro percorso con un modulo dello strumento Funzione incremento, ma non imposti alcun filtro, cosa accadrà quando fai clic su Esegui una volta? Un bundle passerà mai lungo il percorso di fallback con il quarto percorso aggiunto?

+ No, perché senza filtro impostato, ogni bundle seguirà sempre questo percorso invece del percorso di fallback.
