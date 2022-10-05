---
title: Funzione switch
description: Scopri come utilizzare la funzionalità switch utilizzando la funzione Switch.
feature: Workfront Fusion
role: User
level: Beginner
kt: 11051
thumbnail: KT1101.png
source-git-commit: f367e016498d5c1814cab79e19e6e9001db2851f
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---


# Funzione switch

Scopri come utilizzare la funzionalità switch utilizzando la funzione Switch.

## Panoramica sull&#39;esercizio

Per semplici modifiche ai dati, utilizzare la funzione Switch per trasformare un valore in un altro all&#39;interno di un campo modulo. In questo esercizio, modifica la chiave a due lettere con il nome effettivo dello stato di avanzamento del progetto per l’invio di un messaggio e-mail.

![Funzione switch Image 1](../12-exercises/assets/switch-function-walkthrough-1.png)

## Passaggi da seguire

1. Clona lo scenario denominato &quot;Condivisione di variabili tra percorsi di indirizzamento&quot;.
1. Denomina il nuovo scenario &quot;Condivisione di variabili tra percorsi di routing - Switch&quot;.
1. Fai clic sul modulo trigger e aggiungi lo stato di avanzamento alla sezione Outputs.
1. Nel modulo Invia un messaggio e-mail, aggiungi Stato di avanzamento al campo Contenuto .

   + Se mappi solo il valore proveniente dal modulo Ricerca, è presente un codice a due lettere per lo stato di avanzamento.
   + Per &quot;cambiare&quot; il codice per il nome completo di ogni possibile stato di avanzamento, utilizzare la funzione &quot;switch&quot; dalla scheda Funzioni generali.

1. La funzione switch utilizza il valore o l&#39;espressione Stato di avanzamento come chiave, quindi restituisce il valore di output in base a tale chiave.

   + Un valore chiave è definito nella prima posizione dopo lo stato di avanzamento (&quot;LT&quot;) con l&#39;output corrispondente definito nella seconda posizione (&quot;In ritardo&quot;).
   + Il valore chiave successivo è definito nella terza posizione, con l&#39;output corrispondente definito nella quarta posizione, ecc., per il numero di chiavi desiderato.

      ![Funzione switch Image 2](../12-exercises/assets/switch-function-walkthrough-2.png)