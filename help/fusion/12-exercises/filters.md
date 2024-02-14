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
recommendations: noDisplay,noCatalog
exl-id: d2cec1ea-7ff9-48ae-8bfb-0c767d346079
source-git-commit: a4e61514567ac8c2b4ad5c9ecacb87bd83947731
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 98%

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
