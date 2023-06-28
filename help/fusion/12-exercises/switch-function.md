---
title: Funzione switch
description: Scopri come utilizzare la funzionalità di switch utilizzando la funzione Switch.
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
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---

# Funzione switch

Scopri come utilizzare la funzionalità di switch utilizzando la funzione Switch.

## Panoramica dell’esercizio

Per semplici modifiche ai dati, utilizza la funzione Switch per trasformare un valore in un altro all’interno di un campo modulo. In questo esercizio, modifica la chiave di due lettere con il nome effettivo dello stato di avanzamento del progetto da inviare tramite e-mail.

![Funzione switch Image 1](../12-exercises/assets/switch-function-walkthrough-1.png)

## Passaggi da seguire

1. Clonare lo scenario denominato &quot;Condivisione di variabili tra percorsi di routing&quot;.
1. Assegna al nuovo scenario il nome &quot;Condivisione di variabili tra percorsi di routing - Switch&quot;.
1. Fai clic sul modulo trigger e aggiungi lo stato di avanzamento alla sezione Output.
1. Nel campo Invia un modulo e-mail, aggiungi Stato di avanzamento al contenuto.

   + Se mappi semplicemente il valore proveniente dal modulo di ricerca, viene visualizzato un codice di due lettere per lo stato di avanzamento.
   + Per &quot;cambiare&quot; il codice per il nome completo di ogni possibile stato di avanzamento, utilizzare la funzione &quot;cambiare&quot; dalla scheda Funzioni generali.

1. La funzione switch utilizza il valore o l&#39;espressione Stato di avanzamento come chiave, quindi restituisce il valore di output in base a tale chiave.

   + Un valore chiave è definito nella prima posizione dopo lo stato di avanzamento (&quot;LT&quot;) con l&#39;output corrispondente definito nella seconda posizione (&quot;Late&quot;).
   + Il valore chiave successivo è definito nella terza posizione, con l&#39;output corrispondente definito nella quarta posizione, ecc., per il numero di chiavi desiderato.

     ![Funzione switch Image 2](../12-exercises/assets/switch-function-walkthrough-2.png)
