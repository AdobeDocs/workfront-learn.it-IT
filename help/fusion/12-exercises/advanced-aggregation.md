---
title: Aggregazione avanzata
description: Chiama un servizio web per restituire dettagli su più paesi e identificare la popolazione, raggruppata per sottoregione.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11048
thumbnail: KT11048.png
exl-id: 5364befa-491d-4b75-b1f0-10244f70ad7c
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 0%

---

# Aggregazione avanzata

Scopri come utilizzare i raggruppamenti durante l’aggregazione.

## Panoramica dell’esercizio

Chiama un servizio web per restituire dettagli su più paesi e identificare la popolazione totale di tutti i paesi, raggruppati per sottoregione.

![Immagine aggregazione avanzata 1](../12-exercises/assets/advanced-aggregation-walkthrough-1.png)

## Passaggi da seguire

**Ottieni i dettagli del paese.**

![Immagine aggregazione avanzata 2](../12-exercises/assets/advanced-aggregation-walkthrough-2.png)

1. Crea un nuovo scenario e denominalo &quot;Aggregazione avanzata&quot;.
1. Imposta il modulo trigger su HTTP. Effettua una richiesta.
1. Utilizza questo URL, `https://restcountries.com/v2/lang/es`, che fornisce un elenco di tutti i paesi in cui si parla lo spagnolo.
1. Lascia il metodo come Get.
1. Fai clic sulla casella di controllo Analizza risposta.
1. Rinomina questo modulo &quot;Ottieni Paesi&quot;.
1. Fai clic su Salva ed esegui una volta.

   **L’output è un singolo bundle, ma viene fornito in un array con 24 raccolte, una per ogni paese di lingua spagnola.**

   ![Immagine aggregazione avanzata 3](../12-exercises/assets/advanced-aggregation-walkthrough-3.png)

   **È necessario raccogliere informazioni sulle sottoregioni per ciascuno dei paesi, quindi è necessario effettuare una richiesta HTTP aggiuntiva.**

1. Aggiungi un’altra richiesta per ottenere informazioni sulle regioni secondarie. Tornerà solo il primo paese, ma per ora va bene. Aggiungi un altro HTTP Crea un modulo di richiesta e utilizza l’URL `https://restcountries.com/v2/name/{country name}`.
1. Per ottenere il nome del primo paese, vai al pannello di mappatura e fai clic su Dati, quindi su Nome nell’array. Il [1] nel campo dati indica che restituirà il primo elemento dell’array.

   + Fare clic sul numero e modificare l&#39;indice se necessario, ma in questo caso si desidera solo il primo elemento.

![Immagine aggregazione avanzata 4](../12-exercises/assets/advanced-aggregation-walkthrough-4.png)

1. Verifica la risposta di analisi nel pannello di mappatura, quindi fai clic su OK.
1. Rinomina &quot;Ottieni dettagli paese&quot;.
1. Fai clic su Salva, quindi su Esegui una volta.

   + L&#39;output è costituito da informazioni relative a un singolo paese.

1. Per ottenere gli altri paesi, è necessario scorrere l&#39;array. Aggiungi un iteratore che accetta un elenco di elementi e restituisce un bundle per ogni elemento dell’elenco.

   **Aggiungi l’iteratore e l’aggregatore.**

1. Fare clic con il pulsante destro del mouse tra i moduli HTTP e aggiungere il modulo Iterator Flow Control.
1. Nel campo Array, selezionare Dati dal modulo Ottieni paesi.

   ![Immagine aggregazione avanzata 5](../12-exercises/assets/advanced-aggregation-walkthrough-5.png)

1. Nel modulo Ottieni dettagli paese, aggiorna il campo URL in modo che ottenga il campo del nome dall’iteratore anziché dal modulo Ottieni paesi.

   ![Immagine aggregazione avanzata 6](../12-exercises/assets/advanced-aggregation-walkthrough-6.png)

1. Ora aggiungi un aggregatore numerico dopo Ottieni dettagli paese per raggruppare e sommare le popolazioni.
1. Il modulo di origine è il modulo iteratore.
1. La funzione di aggregazione è SOMMA.
1. Il valore è [dati:popolazione] dal modulo Ottieni dettagli paese.
1. Fare clic sull&#39;opzione Mostra impostazioni avanzate nella parte inferiore e raggruppare per [dati:sottoregione] dal modulo Ottieni dettagli paese.

   ![Immagine aggregazione avanzata 7](../12-exercises/assets/advanced-aggregation-walkthrough-7.png)

   **Terminare con un aggregatore di testo per aggregare gli elementi raggruppati all&#39;interno dell&#39;aggregatore numerico.**

1. Aggiunge un aggregatore di testo alla fine.
1. Il modulo di origine è l’aggregatore numerico.
1. Nell&#39;area di testo, inserire &quot;La popolazione totale di [CHIAVE] è [risultato].&quot;

   ![Immagine aggregazione avanzata 8](../12-exercises/assets/advanced-aggregation-walkthrough-8.png)

1. Salva ed esegui una sola volta.

   + Esamina l’output del modulo finale.
