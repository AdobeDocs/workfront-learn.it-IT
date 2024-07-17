---
title: Esercizio per l’aggregazione avanzata
description: Chiamare un servizio web per restituire dettagli su più paesi e identificare la popolazione, raggruppata per sottoregione.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11048
thumbnail: KT11048.png
recommendations: noDisplay,noCatalog
exl-id: 5364befa-491d-4b75-b1f0-10244f70ad7c
source-git-commit: a4e61514567ac8c2b4ad5c9ecacb87bd83947731
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 100%

---

# Esercizio per l’aggregazione avanzata

Scopri come utilizzare i raggruppamenti durante l’aggregazione.

## Panoramica dell’esercizio

Chiamare un servizio web per restituire dettagli su più paesi e identificare la popolazione totale di tutti i paesi, raggruppati per sottoregione.

![Aggregazione avanzata Immagine 1](../12-exercises/assets/advanced-aggregation-walkthrough-1.png)

## Passaggi da seguire

**Ottieni i dettagli del paese.**

![Aggregazione avanzata Immagine 2](../12-exercises/assets/advanced-aggregation-walkthrough-2.png)

1. Crea un nuovo scenario e denominalo “Aggregazione avanzata.”
1. Imposta il modulo trigger su un modulo HTTP Crea una richiesta.
1. Utilizza questo URL, `https://restcountries.com/v2/lang/es`, che fornisce un elenco di tutti i paesi in cui si parla lo spagnolo.
1. Lascia il metodo come Get.
1. Fai clic sulla casella di controllo Analizza risposta.
1. Rinomina questo modulo “Ottieni paesi.”
1. Fai clic su Salva ed esegui una volta.

   **L’output è un bundle singolo, ma viene fornito in un array con 24 raccolte, una per ogni paese di lingua spagnola.**

   ![Aggregazione avanzata Immagine 3](../12-exercises/assets/advanced-aggregation-walkthrough-3.png)

   **È necessario raccogliere informazioni sulle sottoregioni per ciascuno dei paesi, a tal fine dovrai effettuare una richiesta HTTP aggiuntiva.**

1. Aggiungi un’altra richiesta per ottenere informazioni sulla sottoregione. Questa restituirà solo il primo paese e per il momento è sufficiente. Aggiungi un altro modulo HTTP Crea una richiesta e utilizza l’URL `https://restcountries.com/v2/name/{country name}`.
1. Per ottenere il nome del primo paese, passa al pannello di mappatura e fai clic su Dati, quindi su Nome nell’array. L’[1] nel campo dati indica che restituirà il primo elemento nell’array.

   + Fai clic sul numero e modifica l’indice se necessario, ma in questo caso è necessario solo il primo elemento.

![Aggregazione avanzata Immagine 4](../12-exercises/assets/advanced-aggregation-walkthrough-4.png)

1. Verifica la risposta di analisi nel pannello di mappatura, quindi fai clic su OK.
1. Rinominala “Ottieni dettagli paese”.
1. Fai clic su Salva, quindi su Esegui una volta.

   + L’output è costituito da informazioni relative a un singolo paese.

1. Per ottenere gli altri paesi, è necessario iterare attraverso l’array. Aggiungi un iteratore che accetta un elenco di elementi e restituisce un bundle per ogni elemento dell’elenco.

   **Aggiungi l’iteratore e l’aggregatore.**

1. Fai clic con il pulsante destro del mouse tra i moduli HTTP e aggiungi il modulo Iterator Flow Control.
1. Nel campo Array, seleziona Dati dal modulo Ottieni paesi.

   ![Aggregazione avanzata Immagine 5](../12-exercises/assets/advanced-aggregation-walkthrough-5.png)

1. Nel modulo Ottieni dettagli paese, aggiorna il campo URL in modo che ottenga il campo del nome dall’iteratore anziché dal modulo Ottieni paesi.

   ![Aggregazione avanzata Immagine 6](../12-exercises/assets/advanced-aggregation-walkthrough-6.png)

1. Ora aggiungi un aggregatore numerico dopo Ottieni dettagli paese per raggruppare e sommare le popolazioni.
1. Il modulo di origine è il modulo iteratore.
1. La funzione di aggregazione è SUM.
1. Il valore è [data:population] dal modulo Ottieni dettagli paese.
1. Fai clic sull’opzione Mostra impostazioni avanzate nella parte inferiore e raggruppa per [data:subregion] dal modulo Ottieni dettagli paese.

   ![Aggregazione avanzata Immagine 7](../12-exercises/assets/advanced-aggregation-walkthrough-7.png)

   **Termina con un aggregatore di testo per aggregare gli elementi raggruppati all’interno dell’aggregatore numerico.**

1. Aggiungi un aggregatore di testo alla fine.
1. Il modulo di origine è l’aggregatore numerico.
1. Nell’area di testo, immetti “La popolazione totale di [KEY] è il [risultato].”

   ![Aggregazione avanzata Immagine 8](../12-exercises/assets/advanced-aggregation-walkthrough-8.png)

1. Salva ed esegui una sola volta.

   + Esamina l’output del modulo finale.
