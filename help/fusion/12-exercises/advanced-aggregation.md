---
title: Aggregazione avanzata
description: Invoca un servizio Web per restituire i dettagli relativi a più paesi e identificare la popolazione, raggruppata per sottoregione.
feature: Workfront Fusion
role: User
level: Beginner
kt: 11048
thumbnail: KT11048.png
exl-id: 5364befa-491d-4b75-b1f0-10244f70ad7c
source-git-commit: ca56810c9eab36175a6280e319b5fd2aba90b2f2
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 0%

---

# Aggregazione avanzata

Scopri come utilizzare i raggruppamenti durante l’aggregazione.

## Panoramica sull&#39;esercizio

Invoca un servizio Web per restituire i dettagli relativi a più paesi e identificare la popolazione totale di tutti i paesi, raggruppata per subregione.

![Immagine di aggregazione avanzata 1](../12-exercises/assets/advanced-aggregation-walkthrough-1.png)

## Passaggi da seguire

**Visualizza i dettagli del paese.**

![Immagine di aggregazione avanzata 2](../12-exercises/assets/advanced-aggregation-walkthrough-2.png)

1. Crea un nuovo scenario e denominalo &quot;Aggregazione avanzata&quot;.
1. Imposta il modulo trigger su un HTTP - Esegui un modulo di richiesta.
1. Utilizza questo URL, `https://restcountries.com/v2/lang/es`, che fornisce un elenco di tutti i paesi in cui si parla lo spagnolo.
1. Lasciare il metodo come Get.
1. Fai clic sulla casella di controllo Analizza risposta .
1. Rinomina questo modulo &quot;Ottieni Paesi&quot;.
1. Fai clic su Salva ed esegui una volta.

   **L&#39;output è un singolo bundle, ma viene in un array con 24 collezioni, una per ogni paese di lingua spagnola.**

   ![Immagine di aggregazione avanzata 3](../12-exercises/assets/advanced-aggregation-walkthrough-3.png)

   **È necessario raccogliere informazioni sulle subaree per ciascuno dei paesi, in modo da effettuare una richiesta HTTP aggiuntiva.**

1. Aggiungi un’altra richiesta per ottenere informazioni sulla subarea. Restituirà solo il primo paese, ma per ora va bene. Aggiungi un altro modulo di richiesta HTTP e utilizza l’URL `https://restcountries.com/v2/name/{country name}`.
1. Per ottenere il nome del primo paese, vai al pannello di mappatura e fai clic su Dati, quindi su Nome nella matrice. La [1] nel campo dati indica che restituirà il primo elemento della matrice.

   + Fare clic sul numero e modificare l&#39;indice se necessario, ma in questo caso si desidera solo il primo elemento.

![Immagine di aggregazione avanzata 4](../12-exercises/assets/advanced-aggregation-walkthrough-4.png)

1. Selezionate Analizza risposta nel pannello di mappatura, quindi fate clic su OK.
1. Rinomina questo messaggio &quot;Ottieni dettagli paese&quot;.
1. Fai clic su Salva, quindi Esegui una volta.

   + Il risultato è l&#39;informazione per un singolo paese.

1. Per ottenere gli altri paesi, è necessario eseguire iterazioni attraverso l&#39;array. Aggiungi un iteratore, che prende un elenco di cose e produce un bundle per ogni voce dell&#39;elenco.

   **Aggiungi l’iteratore e l’aggregatore.**

1. Fai clic con il pulsante destro del mouse tra i moduli HTTP e aggiungi il modulo Iterator Flow Control .
1. Nel campo Array, selezionare Dati dal modulo Get countries.

   ![Immagine di aggregazione avanzata 5](../12-exercises/assets/advanced-aggregation-walkthrough-5.png)

1. Nel modulo Get Country Details (Ottieni dettagli paese), aggiornare il campo URL in modo che il campo nome venga rimosso dall&#39;iteratore anziché dal modulo Get countries (Ottieni paesi).

   ![Immagine di aggregazione avanzata 6](../12-exercises/assets/advanced-aggregation-walkthrough-6.png)

1. Ora aggiungi un aggregatore numerico dopo Ottieni dettagli paese per raggruppare e sommare le popolazioni.
1. Il modulo di origine è il modulo iteratore.
1. La funzione aggregata è SOMMA.
1. Il valore è [dati:popolazione] dal modulo Get Country Details.
1. Fai clic sull’opzione Mostra impostazioni avanzate in basso e raggruppa per [dati:subarea] dal modulo Get Country Details.

   ![Immagine di aggregazione avanzata 7](../12-exercises/assets/advanced-aggregation-walkthrough-7.png)

   **Completa con un aggregatore di testo per aggregare ciò che hai raggruppato all’interno dell’aggregatore numerico.**

1. Aggiungi un aggregatore di testo alla fine.
1. Il modulo di origine è l&#39;aggregatore numerico.
1. Nell&#39;area Testo, inserire &quot;La popolazione totale di [CHIAVE] è [risultato].&quot;

   ![Immagine di aggregazione avanzata 8](../12-exercises/assets/advanced-aggregation-walkthrough-8.png)

1. Salva ed esegui una volta.

   + Esamina l&#39;output del modulo finale.
