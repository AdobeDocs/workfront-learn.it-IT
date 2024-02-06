---
title: Funzione switch
description: Scopri come utilizzare la funzionalità switch utilizzando la funzione Switch.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11051
thumbnail: KT1101.png
exl-id: 3142fae2-5210-4f63-9d2c-66dec58867fa
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: ht
source-wordcount: '234'
ht-degree: 100%

---

# Funzione switch

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
