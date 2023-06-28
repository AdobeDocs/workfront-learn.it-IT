---
title: Filtri
description: Scopri come utilizzare il filtro tra i moduli per consentire solo determinati tipi di bundle tramite.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11040
thumbnail: KT1101.png
exl-id: d2cec1ea-7ff9-48ae-8bfb-0c767d346079
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 0%

---

# Filtri

Scopri come utilizzare il filtro tra i moduli per consentire solo determinati tipi di bundle tramite.

## Panoramica dell’esercizio

Aggiungi un filtro tra i due moduli nello scenario di mappatura di base Beyond per creare solo progetti con un colore di progetto &quot;Rosso&quot; nel file CSV.

![Filtri Immagine 1](../12-exercises/assets/filters-walkthrough-1.png)

## Passaggi da seguire

1. Crea un clone dello scenario &quot;Oltre la mappatura di base&quot; e denominalo &quot;Utilizzando il potente filtro&quot;.

   **Aggiungi un filtro prima del modulo Crea progetti Workfront per consentire la creazione solo di progetti rossi.**

   ![Filtri Immagine 2](../12-exercises/assets/filters-walkthrough-2.png)

1. Aggiungi un filtro facendo clic sulla linea tratteggiata che collega i moduli o facendo clic sulla chiave inglese e selezionando Imposta un filtro.
1. Utilizza il campo Etichetta per denominare il filtro &quot;Solo progetti rossi&quot;.
1. Nel campo Condizione mappare il campo Colore progetto (colonna 3 nel file CSV). Selezionare l&#39;operatore Uguale a (senza distinzione maiuscole/minuscole), quindi digitare &quot;rosso&quot;.
1. Fare clic su OK.

   ![Filtri Immagine 3](../12-exercises/assets/filters-walkthrough-3.png)

   **Verifica il filtro e i risultati.**

1. Fai clic su Salva per salvare lo scenario, quindi su Esegui una volta.
1. Fai clic sul controllo di esecuzione per il filtro per vedere in che modo ogni bundle è stato esaminato dal filtro e ha superato o non è riuscito a passare al modulo Crea progetti Workfront.

   ![Filtri Immagine 4](../12-exercises/assets/filters-walkthrough-4.png)

1. Trova i progetti creati nell’istanza Workfront.
