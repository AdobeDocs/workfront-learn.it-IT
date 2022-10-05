---
title: Esplorazione di esecuzioni, cicli e bundle
description: Comprendi il comportamento di esecuzioni, cicli e bundle utilizzando la cronologia di esecuzione di uno scenario.
feature: Workfront Fusion
role: User
level: Beginner
kt: 11050
thumbnail: KT1101.png
source-git-commit: c348222464180e994e7b414d1b84e07f58b6b2ae
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---


# Esplorazione di esecuzioni, cicli e bundle

Comprendi il comportamento di esecuzioni, cicli e bundle utilizzando la cronologia di esecuzione di uno scenario.

## Panoramica sull&#39;esercizio

Esercitarsi con diverse configurazioni di scenario per esplorare utilizzando esecuzioni e cicli.

![Esplorazione di cicli e bundle di esecuzione Immagine 1](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-1.png)

## Passaggi da seguire

1. Clona lo scenario denominato &quot;Condivisione di variabili tra percorsi di indirizzamento&quot;. Denomina il nuovo scenario &quot;Condivisione di variabili tra percorsi di indirizzamento - Test Cicli&quot;.
1. Rimuovi il modulo Invia un messaggio e-mail, in quanto non è necessario per questo test.

   **Imposta lo scenario per elaborare 3 cicli per esecuzione. Elabora 5 progetti in ogni ciclo.**

1. Fai clic sul modulo trigger e modifica il campo Massimale in 5, in modo che in ogni ciclo vengano elaborati solo 5 progetti.
1. Nei criteri di ricerca, rimuovi il secondo filtro che limita la ricerca a un singolo progetto.
1. Fate clic su OK.

1. Nella barra degli strumenti Fusion, aprire le impostazioni Scenario e modificare il campo Numero massimo di cicli da 1 a 3.
1. Fate clic su OK.

   ![Esplorazione di cicli e bundle di esecuzione Immagine 1](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-1.png)


   **Pianifica l&#39;esecuzione dello scenario ogni minuto.**

1. Fai clic sull&#39;icona dell&#39;orologio dal modulo trigger e modifica il campo Minutes a 1 minuto.

   ![Esplorazione di cicli e bundle di esecuzione Immagine 2](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-2.png)

1. Quindi, attiva l&#39;opzione Pianificazione sotto il pulsante Esegui una volta. Salva lo scenario.

   ![Esplorazione di cicli e bundle di esecuzione Immagine 3](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-3.png)

1. Passa alla cronologia di esecuzione per lo scenario e osserva come viene visualizzato un nuovo record di cronologia entro il minuto successivo. Potrebbe essere necessario aggiornare la pagina.

   ![Esplorazione di cicli e bundle di esecuzione Immagine 1](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-4.png)

1. Fare clic sul pulsante Dettagli di un&#39;esecuzione. Fai clic sul collegamento Semplice nel pannello a destra, simile a quello che hai fatto nella sezione della cronologia di esecuzione del corso di formazione Workfront Fusion.
1. I record delle operazioni elaborate sono suddivisi in cicli.

   ![Esplorazione di cicli di esecuzione e bundle Immagine 5](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-5.png)

1. Un menu a discesa in alto a destra nella finestra consente di selezionare uno dei 3 cicli impostati per essere eseguiti ogni volta.

   ![Esplorazione di cicli di esecuzione e bundle Immagine 6](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-6.png)
