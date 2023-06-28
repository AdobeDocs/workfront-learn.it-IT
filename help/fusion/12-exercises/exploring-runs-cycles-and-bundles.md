---
title: Esplorazione di esecuzioni, cicli e bundle
description: Comprendi il comportamento di esecuzioni, cicli e bundle utilizzando la cronologia di esecuzione di uno scenario.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11050
thumbnail: KT1101.png
exl-id: f04c84b1-2a3c-418b-9db3-baa74cf364f3
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---

# Esplorazione di esecuzioni, cicli e bundle

Comprendi il comportamento di esecuzioni, cicli e bundle utilizzando la cronologia di esecuzione di uno scenario.

## Panoramica dell’esercizio

Esercitati con diverse configurazioni di scenari per esplorare utilizzando esecuzioni e cicli.

![Esplorazione di cicli di esecuzione e bundle Immagine 1](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-1.png)

## Passaggi da seguire

1. Clonare lo scenario denominato &quot;Condivisione di variabili tra percorsi di routing&quot;. Assegna al nuovo scenario il nome &quot;Condivisione di variabili tra percorsi di routing - Test dei cicli&quot;.
1. Rimuovi il modulo Invia un’e-mail, poiché non è necessario per questo test.

   **Imposta lo scenario per elaborare 3 cicli per esecuzione. Elabora 5 progetti in ogni ciclo.**

1. Fai clic sul modulo di attivazione e modifica il campo Massimo in 5, in modo da elaborare solo 5 progetti in ogni ciclo.
1. Nei criteri di ricerca, rimuovi il secondo filtro che limita la ricerca a un singolo progetto.
1. Fare clic su OK.

1. Nella barra degli strumenti di Fusion, apri le impostazioni Scenario e modifica il campo Numero massimo di cicli da 1 a 3.
1. Fare clic su OK.

   ![Esplorazione di cicli di esecuzione e bundle Immagine 1](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-1.png)


   **Pianifica l’esecuzione dello scenario ogni minuto.**

1. Fai clic sull’icona dell’orologio dal modulo trigger e modifica il campo Minutes (Minuti) in 1 minuto.

   ![Esplorazione di cicli di esecuzione e bundle Immagine 2](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-2.png)

1. Quindi, impostare su On l&#39;opzione Pianificazione sotto il pulsante Esegui una volta. Salva lo scenario.

   ![Esplorazione di cicli di esecuzione e bundle Immagine 3](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-3.png)

1. Vai alla Cronologia di esecuzione per lo scenario e osserva come viene visualizzato un nuovo record della cronologia nel minuto successivo. Potrebbe essere necessario aggiornare la pagina.

   ![Esplorazione di cicli di esecuzione e bundle Immagine 1](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-4.png)

1. Fare clic sul pulsante Dettagli di un&#39;esecuzione. Fai clic sul registro semplice nel pannello a destra, in modo simile a quanto hai fatto nella sezione relativa alla cronologia di esecuzione del corso di formazione su Workfront Fusion.
1. I record delle operazioni elaborate vengono suddivisi in cicli.

   ![Esplorazione di cicli di esecuzione e bundle Immagine 5](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-5.png)

1. Un menu a discesa in alto a destra della finestra consente di selezionare ogni volta uno qualsiasi dei 3 cicli impostati per l&#39;esecuzione.

   ![Esplorazione di cicli di esecuzione e bundle Immagine 6](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-6.png)
