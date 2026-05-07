---
title: Esercizio del modulo Switch
description: Scopri come utilizzare il modulo Switch quando devi eseguire trasformazioni di dati più complesse o dinamiche.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11052
thumbnail: KT11052.png
recommendations: noDisplay,catalog
exl-id: 1b810168-582d-4d7d-b061-d152af546bc8
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
autotag-review: '2026-05-06T16:40:26.747Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 327
ht-degree: 100%

---

# Esercizio del modulo Switch

Scopri come utilizzare il modulo Switch quando devi eseguire trasformazioni di dati più complesse o dinamiche.

## Panoramica dell’esercizio

Cerca i progetti di direct mailing nell’unità di test, quindi modifica il nome di ciascun progetto in base a un valore selezionato in un campo personalizzato allegato al progetto.

![Immagine 1 di Modulo Switch](../12-exercises/assets/switch-module-walkthrough-1.png)

## Passaggi da seguire

1. Crea un nuovo scenario e denominalo “Utilizzo del modulo Switch”.
1. Per il modulo trigger, utilizza il modulo Workfront Search.
1. Imposta la connessione Workfront e imposta il tipo di record su Progetto.
1. Nei criteri di ricerca, specifica che desideri visualizzare solo i progetti con un valore nel campo personalizzato Canale.
1. Per gli output, seleziona ID, Nome, Numero di riferimento e il campo personalizzato Canale.

   ![Immagine 2 di Modulo Switch](../12-exercises/assets/switch-module-walkthrough-2.png)

1. Aggiungi il modulo Switch da Strumenti.
1. Per il campo Input, mappa il campo personalizzato Canale dal modulo di ricerca.

   ![Immagine 3 di Modulo Switch](../12-exercises/assets/switch-module-walkthrough-3.png)

1. Quindi aggiungi dei casi per ogni possibile valore proveniente dal campo personalizzato Canale. Il valore possibile viene inserito nel campo Pattern. Il campo di output deve includere un codice di 3 lettere specifico seguito dal numero di riferimento del progetto e quindi dal nome del progetto.

   **Il pannello di mappatura si presenta simile al seguente:**

   ![Immagine 4 di Modulo Switch](../12-exercises/assets/switch-module-walkthrough-4.png)

1. Puoi aggiungere tutti i casi aggiuntivi che desideri. Osserva il campo Else in basso. Verrà utilizzato se il valore specificato non corrisponde a nessuno dei casi.

   **Aggiorna il nome del progetto in Workfront.**

   ![Immagine 5 di Modulo Switch](../12-exercises/assets/switch-module-walkthrough-5.png)

1. Aggiungi un modulo Workfront Update Record.
1. Nel campo ID, mappalo con l’ID dal modulo trigger.
1. Imposta il Tipo record su Progetto.
1. Seleziona il campo Nome dalla sezione Select Fields to Map (Seleziona campi da mappare) e associalo all’output del modulo Switch.
1. Salva lo scenario ed esegui una volta. Visualizza i nomi dei progetti aggiornati nell’unità di test.
