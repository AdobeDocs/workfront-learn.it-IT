---
title: Tocca a te creare un rapporto sul calendario
description: Scopri come creare un calendario del cliente con le attività e i problemi incompleti.
activity: use
team: Technical Marketing
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
thumbnail: your-turn-to-create-a-calendar.png
jira: KT-10026
exl-id: 74d57f1a-c6c5-49e0-9529-2e2deb2f273e
source-git-commit: e5017c98275f3b3853d7a37ee9d1d77d8d7f9098
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 1%

---

# Tocca a te creare un rapporto sul calendario

In questa attività ti occuperai della creazione del tuo calendario.

## Attività: creare un calendario

Crea un calendario cliente denominato &quot;Il mio lavoro incompleto&quot;.

Includere un gruppo di calendari denominato &quot;Attività non completate&quot; che mostra tutte le attività incomplete assegnate all&#39;utente nei progetti correnti.

Selezionate il rosso come colore per questi elementi.

Includi un altro gruppo di calendari denominato &quot;Problemi incompleti&quot; che mostra tutti i problemi incompleti assegnati all’utente nei progetti correnti. Selezionate blu come colore per questi elementi.

## Risposta

1. Passare all&#39;area Calendari dal menu Principale.
1. Fare clic sul pulsante Nuovo calendario e denominare il calendario &quot;Il mio lavoro incompleto&quot;.
1. Nel primo raggruppamento fare clic su Aggiungi elementi avanzati.
1. Nella finestra Aggiungi elementi al calendario visualizzata, assegna al gruppo il nome &quot;Attività non completate&quot;.
1. Selezionate il rosso come colore.
1. Modifica il campo Data in Date pianificate.
1. Impostare il campo Mostra solo data di fine nel calendario.
1. Impostare il campo Passa alle date effettive quando disponibile su No.

   ![Immagine della schermata per aggiungere elementi a un calendario](assets/calendar-activity-1.png)

1. In Cosa si desidera aggiungere al calendario? , selezionare Attività.
1. Aggiungi tre regole di filtro:

   * Progetto > Stato equivale a > Uguale a > Corrente
   * Utenti assegnazione > ID > Uguale > $$USER.ID
   * Task > È completo > Uguale > Falso

1. Fai clic su Salva.

   ![Immagine della schermata per aggiungere elementi a un calendario](assets/calendar-activity-2.png)

1. Creare un secondo raggruppamento facendo clic su Aggiungi al calendario.
1. In questo raggruppamento, fai clic su Aggiungi elementi avanzati.
1. Nella finestra Aggiungi elementi al calendario visualizzata, assegna al gruppo il nome &quot;Problemi incompleti&quot;.
1. Selezionate blu come colore.
1. Modifica il campo Data in Date pianificate.
1. Impostare il campo Mostra solo data di fine nel calendario.
1. Impostare il campo Passa alle date effettive quando disponibile su No.
1. In Cosa si desidera aggiungere al calendario? , selezionare Issues.
1. Aggiungi le tre regole di filtro seguenti:

   * Progetto > Stato equivale a > Uguale a > Corrente
   * Utenti assegnazione > ID > Uguale > $$USER.ID
   * Problema > È completo > Uguale > Falso

1. Fai clic su Salva.

   ![Immagine della schermata per aggiungere elementi a un calendario](assets/calendar-activity-3.png)

Poiché hai usato $$USER.ID nei filtri, puoi condividere questo calendario con altri utenti, che visualizzeranno le proprie attività e i propri problemi incompleti.
