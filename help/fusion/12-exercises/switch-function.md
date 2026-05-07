---
title: Esercizio sulla funzione Switch
description: Scopri come utilizzare la funzionalità switch utilizzando la funzione Switch.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11051
thumbnail: KT1101.png
recommendations: noDisplay,catalog
exl-id: 3142fae2-5210-4f63-9d2c-66dec58867fa
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
autotag-review: '2026-05-06T16:41:24.173Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 240
ht-degree: 100%

---

# Esercizio sulla funzione Switch

Scopri come utilizzare la funzionalità switch utilizzando la funzione Switch.

## Panoramica dell’esercizio

Per semplici modifiche ai dati, utilizza la funzione Switch per trasformare un valore in un altro all’interno di un campo modulo. In questo esercizio, modifica la chiave di due lettere con il nome effettivo dello stato di avanzamento del progetto da inviare tramite e-mail.

![Funzione Switch immagine 1](../12-exercises/assets/switch-function-walkthrough-1.png)

## Passaggi da seguire

1. Clona lo scenario denominato “Sharing variables between routing paths” (Condivisione di variabili tra percorsi di routing).
1. Assegna al nuovo scenario il nome “Condivisione di variabili tra percorsi di indirizzamento - Switch”.
1. Fai clic sul modulo trigger e aggiungi lo stato di avanzamento alla sezione Output.
1. Nel modulo Invia e-mail, aggiungi Stato di avanzamento al campo Contenuto.

   + Se mappi semplicemente il valore proveniente dal modulo di ricerca, per lo stato di avanzamento viene visualizzato un codice di due lettere.
   + Per “cambiare” il codice nel nome completo di ogni possibile stato di avanzamento, utilizza la funzione “switch” dalla scheda Funzioni generali.

1. La funzione switch utilizza il valore o l’espressione Stato di avanzamento come chiave, quindi restituisce il valore di output in base a tale chiave.

   + Un valore chiave è definito nella prima posizione dopo lo Stato di avanzamento (“LT”) con l’output corrispondente definito nella seconda posizione (“In ritardo”).
   + Il valore chiave successivo è definito nella terza posizione, con l’output corrispondente definito nella quarta posizione, ecc., per il numero di chiavi desiderato.

     ![Funzione Switch immagine 2](../12-exercises/assets/switch-function-walkthrough-2.png)
