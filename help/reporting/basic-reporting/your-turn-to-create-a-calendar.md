---
title: Il turno per creare un calendario
description: Scopri come creare un calendario del cliente che mostra le attività e i problemi incompleti.
activity: use
team: Technical Marketing
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
thumbnail: your-turn-to-create-a-calendar.png
kt: 10026
exl-id: 74d57f1a-c6c5-49e0-9529-2e2deb2f273e
source-git-commit: 252ba3ba44f22519a35899fcda9c6bca597a6c2c
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 1%

---

# Il turno per creare un calendario

In questa attività otterrai un’esperienza nella creazione del tuo calendario.

## Attività: Crea un calendario

Crea un calendario cliente denominato &quot;Lavoro incompleto&quot;.

Includi un gruppo di calendario denominato &quot;Attività incomplete&quot; che mostra tutte le attività incomplete assegnate a te sui progetti correnti.

Selezionare rosso come colore per questi elementi.

Includi un altro gruppo di calendario denominato &quot;Problemi incompleti&quot; che mostra tutti i problemi incompleti assegnati ai progetti correnti. Seleziona blu come colore per questi elementi.

## Risposta

1. Selezionare l&#39;area Calendari dal menu Principale.
1. Fai clic sul pulsante Nuovo calendario e assegna un nome al calendario &quot;Lavoro incompleto&quot;.
1. Nel primo raggruppamento, fai clic su Aggiungi elementi avanzati.
1. Nella finestra Aggiungi elementi al calendario visualizzata, denominare il gruppo &quot;Attività incomplete&quot;.
1. Selezionare il rosso come colore.
1. Cambia il campo Data in Date pianificate.
1. Imposta il campo Sul calendario, mostra solo la data di fine.
1. Imposta il campo Passa alle date effettive quando disponibile su No.

   ![Immagine della schermata per aggiungere elementi a un calendario](assets/calendar-activity-1.png)

1. In Cosa desideri aggiungere al calendario? selezionare Attività.
1. Aggiungi tre regole di filtro:

   * Progetto > Equivale A Stato Con > Uguale > Corrente
   * Utenti assegnazione > ID > Uguale > $$USER.ID
   * Attività > Completa > Uguale > Falso

1. Fai clic su Salva.

   ![Immagine della schermata per aggiungere elementi a un calendario](assets/calendar-activity-2.png)

1. Crea un secondo raggruppamento facendo clic su Aggiungi al calendario.
1. In questo raggruppamento, fai clic su Aggiungi elementi avanzati.
1. Nella finestra Aggiungi elementi al calendario visualizzata, denominare il gruppo &quot;Problemi incompleti&quot;.
1. Seleziona blu come colore.
1. Cambia il campo Data in Date pianificate.
1. Imposta il campo Sul calendario, mostra solo la data di fine.
1. Imposta il campo Passa alle date effettive quando disponibile su No.
1. In Cosa desideri aggiungere al calendario? selezionare Problemi.
1. Aggiungi le tre regole di filtro seguenti:

   * Progetto > Equivale A Stato Con > Uguale > Corrente
   * Utenti assegnazione > ID > Uguale > $$USER.ID
   * Problema > Completo > Uguale > Falso

1. Fai clic su Salva.

   ![Immagine della schermata per aggiungere elementi a un calendario](assets/calendar-activity-3.png)

Poiché hai utilizzato $$USER.ID nei filtri, puoi condividere questo calendario con altri e vedranno le loro attività e problemi incompleti.
