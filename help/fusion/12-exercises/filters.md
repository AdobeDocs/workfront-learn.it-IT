---
title: Esercizio sui filtri
description: Scopri come utilizzare il filtro tra i moduli per consentire solo determinati tipi di bundle.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11040
thumbnail: KT1101.png
recommendations: noDisplay,catalog
exl-id: d2cec1ea-7ff9-48ae-8bfb-0c767d346079
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: c3a155b4-a54b-4a82-a3d2-c8f0f971673e
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-06T16:43:22.961Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 230
ht-degree: 100%

---

# Esercizio sui filtri

Scopri come utilizzare il filtro tra i moduli per consentire solo determinati tipi di bundle.

## Panoramica dell’esercizio

Aggiungi un filtro tra i due moduli nello scenario Oltre la mappatura di base per creare solo progetti con un colore di progetto “Rosso” nel file CSV.

![Immagine 1 Filtri](../12-exercises/assets/filters-walkthrough-1.png)

## Passaggi da seguire

1. Crea un clone dello scenario “Oltre la mappatura di base” e denominalo “Utilizzo del filtro potente”.

   **Aggiungi un filtro prima del modulo Crea progetti Workfront per consentire solo la creazione di progetti rossi.**

   ![Filtri immagine 2](../12-exercises/assets/filters-walkthrough-2.png)

1. Aggiungi un filtro facendo clic sulla linea tratteggiata che collega i moduli o facendo clic sull’icona a forma di chiave inglese e selezionando Imposta un filtro.
1. Utilizza il campo Etichetta per denominare il filtro “Solo progetti rossi”.
1. Nel campo Condizione, mappa il campo Colore progetto (colonna 3 nel file CSV). Seleziona l’operatore Uguale a (senza distinzione maiuscole/minuscole), quindi digita “rosso”.
1. Fai clic su OK.

   ![Filtri immagine 3](../12-exercises/assets/filters-walkthrough-3.png)

   **Verifica il filtro e i risultati.**

1. Fai clic su Salva per salvare lo scenario, quindi su Esegui una volta.
1. Fai clic sul controllo di esecuzione per il filtro per vedere in che modo ogni pacchetto è stato esaminato dal filtro e ha superato o non è riuscito a passare al modulo Crea progetti di Workfront.

   ![Filtri immagine 4](../12-exercises/assets/filters-walkthrough-4.png)

1. Trova i progetti creati nell’istanza Workfront.
