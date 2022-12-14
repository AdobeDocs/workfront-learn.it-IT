---
title: Filtri
description: Scopri come utilizzare il filtro tra i moduli per consentire solo alcuni tipi di bundle attraverso.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 11040
thumbnail: KT1101.png
exl-id: d2cec1ea-7ff9-48ae-8bfb-0c767d346079
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Filtri

Scopri come utilizzare il filtro tra i moduli per consentire solo alcuni tipi di bundle attraverso.

## Panoramica sull&#39;esercizio

Aggiungi un filtro tra i due moduli nello scenario di mappatura &quot;Oltre la base&quot; per creare solo progetti con un colore di progetto &quot;Rosso&quot; nel file CSV.

![Filtri Immagine 1](../12-exercises/assets/filters-walkthrough-1.png)

## Passaggi da seguire

1. Crea un clone dello scenario &quot;Oltre la mappatura di base&quot; e denominalo &quot;Utilizzo del filtro potente&quot;.

   **Aggiungi un filtro prima del modulo Crea progetti Workfront per consentire la creazione solo di progetti rossi.**

   ![Filtri Immagine 2](../12-exercises/assets/filters-walkthrough-2.png)

1. Aggiungi un filtro facendo clic sulla linea tratteggiata che collega i moduli o facendo clic sulla chiave e selezionando Imposta un filtro.
1. Usa il campo Etichetta per denominare il filtro &quot;Solo progetti rossi&quot;.
1. Nel campo Condizione , mappa il campo Colore progetto (Colonna 3 nel file CSV). Selezionare l&#39;operatore Uguale a (senza distinzione maiuscole/minuscole), quindi digitare &quot;rosso&quot;.
1. Fate clic su OK.

   ![Filtri Immagine 3](../12-exercises/assets/filters-walkthrough-3.png)

   **Verifica il filtro e i risultati.**

1. Fai clic su Salva per salvare lo scenario e quindi su Esegui una volta.
1. Fai clic sul controllo di esecuzione del filtro per vedere come ogni bundle è stato esaminato dal filtro e passato o non è riuscito a passare al modulo Crea progetti Workfront.

   ![Filtri immagine 4](../12-exercises/assets/filters-walkthrough-4.png)

1. Trova i progetti creati nella tua istanza Workfront.
