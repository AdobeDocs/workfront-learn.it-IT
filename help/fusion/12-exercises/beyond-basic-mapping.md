---
title: Esercizio oltre la mappatura di base
description: Scopri come utilizzare le formule del pannello di mappatura per manipolare o convertire i campi inviati a un modulo.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11039
thumbnail: KT11039.png
recommendations: noDisplay,catalog
exl-id: 979d794d-b936-402e-b07c-71e999f40780
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: c3a155b4-a54b-4a82-a3d2-c8f0f971673e
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-06T16:44:57.573Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 314
ht-degree: 100%

---

# Esercizio oltre la mappatura di base

Scopri come utilizzare le formule del pannello di mappatura per manipolare o convertire i campi inviati a un modulo.

## Panoramica dell’esercizio

Modifica il nome del progetto, la data di inizio pianificata e la priorità dagli esercizi di procedura dettagliata Oltre la mappatura di base utilizzando le formule del pannello di mappatura.

![Immagine 1 Oltre la mappatura di base](../12-exercises/assets/beyond-basic-mapping-walkthrough-1.png)

## Passaggi da seguire

**Crea un clone dello scenario di progettazione iniziale.**

1. Seleziona l’opzione Clona a destra della progettazione dello scenario iniziale nella sezione dello scenario, come illustrato di seguito. Denominalo “Oltre la mappatura di base”.

   ![Immagine 2 Oltre la mappatura di base](../12-exercises/assets/beyond-basic-mapping-walkthrough-2.png)

   **Ora utilizzeremo il pannello di mappatura nel modulo Crea progetti Workfront per configurare i campi Nome del progetto, Data di inizio pianificata e Priorità.**

1. Fai clic sul modulo Crea progetti Workfront per modificare le impostazioni. Utilizzando il pannello di mappatura, imposta il campo Nome su “[Nome progetto personale] da [Sponsor]”.

   + [Nome progetto personale] è la colonna 1 del modulo Analizza CSV, mentre [Sponsor] è la colonna 6. Il termine “per” è solo scritto tra le due colonne.

1. Passa quindi alla Data di inizio pianificata e utilizza la formula addDays per aggiungere 15 giorni al campo, come descritto nel video della procedura dettagliata relativa a Oltre la mappatura di base.
1. Trova il campo Priorità e attiva il pulsante Mappa in alto a destra del campo. Il menu dell’elenco a discesa diventa un numero. Crea un’istruzione “if” per etichettare un progetto come priorità Alta(4) se il livello di affidabilità del file CSV è inferiore a 100, altrimenti può essere Normale(2).

   + Il valore di affidabilità è riportato nella colonna 4.

   **A questo punto, il pannello di mappatura sarà simile al seguente:**

   ![Immagine 3 Oltre la mappatura di base](../12-exercises/assets/beyond-basic-mapping-walkthrough-3.png)

1. Fai clic su OK e quindi su Esegui una volta.
1. Trova il progetto nell’istanza Workfront per assicurarti che tutto sia stato mappato correttamente.
1. Salva lo scenario.
