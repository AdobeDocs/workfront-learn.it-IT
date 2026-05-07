---
title: Esercizio sull’esplorazione di esecuzioni, cicli e bundle
description: Comprendi il comportamento di esecuzioni, cicli e bundle utilizzando la cronologia di esecuzione di uno scenario.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11050
thumbnail: KT1101.png
recommendations: noDisplay,catalog
exl-id: f04c84b1-2a3c-418b-9db3-baa74cf364f3
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: c3a155b4-a54b-4a82-a3d2-c8f0f971673e
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-06T16:43:39.670Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 344
ht-degree: 100%

---

# Esercizio sull’esplorazione di esecuzioni, cicli e bundle

Comprendi il comportamento di esecuzioni, cicli e bundle utilizzando la cronologia di esecuzione di uno scenario.

## Panoramica dell’esercizio

Esercitati con diverse configurazioni di scenari per esplorare utilizzando esecuzioni e cicli.

![Immagine 1 di Esplorazione di esecuzioni, cicli e bundle](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-1.png)

## Passaggi da seguire

1. Clona lo scenario denominato “Sharing variables between routing paths” (Condivisione di variabili tra percorsi di routing). Assegna al nuovo scenario il nome “Sharing variables between routing paths - Cycles test” (Condivisione di variabili tra percorsi di routing - Test cicli).
1. Rimuovi il modulo Send an email (Invia un’e-mail), poiché non è necessario per questo test.

   **Configura lo scenario per elaborare 3 cicli per esecuzione. Elabora 5 progetti in ogni ciclo.**

1. Fai clic sul modulo di attivazione e modifica il campo Maximal (Massimo) in 5, in modo da elaborare solo 5 progetti in ogni ciclo.
1. Nei criteri di ricerca, rimuovi il secondo filtro che limita la ricerca a un singolo progetto.
1. Fai clic su OK.

1. Nella barra degli strumenti di Fusion, apri le impostazioni Scenario e modifica il campo Max number of cycles (Numero massimo di cicli) da 1 a 3.
1. Fai clic su OK.

   ![Immagine 1 di Esplorazione di esecuzioni, cicli e bundle](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-1.png)


   **Pianifica l’esecuzione dello scenario ogni minuto.**

1. Fai clic sull’icona dell’orologio dal modulo trigger e modifica il campo Minutes (Minuti) su 1 minuto.

   ![Immagine 2 di Esplorazione di esecuzioni, cicli e bundle](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-2.png)

1. Successivamente, premi il pulsante di attivazione Pianificazione sotto il pulsante Run once (Esegui una volta) per attivarlo. Salva lo scenario.

   ![Immagine 3 di Esplorazione di esecuzioni, cicli e bundle](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-3.png)

1. Vai alla Cronologia delle esecuzioni per lo scenario e osserva come viene visualizzato un nuovo record della cronologia entro il minuto successivo. Potrebbe essere necessario aggiornare la pagina.

   ![Immagine 1 di Esplorazione di esecuzioni, cicli e bundle](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-4.png)

1. Fai clic sul pulsante dei dettagli di un’esecuzione. Fai clic sul registro semplice nel pannello a destra, in modo simile a quanto fatto nella sezione relativa alla cronologia di esecuzione del corso di formazione su Workfront Fusion.
1. I record delle operazioni elaborate vengono suddivisi in cicli.

   ![Immagine 5 di Esplorazione di esecuzioni, cicli e bundle](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-5.png)

1. Un menu a discesa in alto a destra della finestra consente di selezionare ogni volta uno dei 3 cicli impostati per l’esecuzione.

   ![Immagine 6 di Esplorazione di esecuzioni, cicli e bundle](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-6.png)
