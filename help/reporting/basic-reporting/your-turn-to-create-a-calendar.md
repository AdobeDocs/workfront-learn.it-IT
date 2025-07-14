---
title: 'Attività: creare un rapporto sul calendario'
description: Istruzioni dettagliate su come creare un calendario del cliente con le attività e i problemi incompleti.
activity: use
team: Technical Marketing
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
last-substantial-update: 2025-06-23T00:00:00Z
thumbnail: your-turn-to-create-a-calendar.png
jira: KT-10026
exl-id: 74d57f1a-c6c5-49e0-9529-2e2deb2f273e
source-git-commit: c5f90e3f36744bbcd6cd7ad8044390f4e222008f
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 81%

---

# Attività: creare un rapporto sul calendario

Crea un calendario cliente denominato “Il mio lavoro incompleto”.

Includi un gruppo di calendario denominato “Attività incomplete” che mostra tutte le attività incomplete assegnate a te nei Progetti correnti.

Seleziona il rosso come colore per questi elementi.

Includi un altro gruppo di calendario denominato “Problemi incompleti” che mostra tutti i problemi incompleti assegnati a te nei Progetti correnti. Seleziona blu come colore per questi elementi.

## Risposta

1. Passa all’area Calendari dal menu Principale.
1. Fai clic sul pulsante Nuovo calendario e assegna il nome al calendario “Il mio lavoro incompleto”.
1. Fai clic sul pulsante Aggiungi al calendario, quindi Aggiungi elementi avanzati.
1. Nella finestra Aggiungi elementi al calendario che viene visualizzata, assegna il nome “Attività incomplete” al gruppo.
1. Seleziona il rosso come colore.
1. Modifica il campo Data in Date pianificate.
1. Imposta il campo Mostra solo data di fine nel calendario.
1. Imposta il campo Passa alle date effettive quando disponibile su No.
1. Che cosa aggiungere al calendario? , selezionare Attività. Fare quindi clic sul pulsante Aggiungi attività.
1. Aggiungi tre regole di filtro:

   * Progetto > Stato equivale a > Uguale a > Corrente
   * Utenti dell’assegnazione > ID > Uguale > $$USER.ID
   * Attività > È completa > Uguale > Falso

1. Fai clic su Salva.

   ![Immagine della schermata per aggiungere elementi a un calendario](assets/calendar-activity-1.png)

1. Creare un secondo raggruppamento facendo clic su Aggiungi al calendario, quindi su Aggiungi elementi avanzati.
1. Nella finestra Aggiungi elementi al calendario che viene visualizzata, assegna al gruppo il nome “Problemi incompleti”.
1. Seleziona blu come colore.
1. Modifica il campo Data in Date pianificate.
1. Imposta il campo Mostra solo data di fine nel calendario.
1. Imposta il campo Passa alle date effettive quando disponibile su No.
1. Che cosa aggiungere al calendario? , selezionare Issues. Quindi fai clic sul pulsante Aggiungi problemi.
1. Aggiungi le tre regole di filtro seguenti:

   * Progetto > Stato equivale a > Uguale a > Corrente
   * Utenti dell’assegnazione > ID > Uguale > $$USER.ID
   * Problema > È completo > Uguale > Falso

1. Fai clic su Salva.

   ![Immagine della schermata per aggiungere elementi a un calendario](assets/calendar-activity-2.png)

Poiché hai usato $$USER.ID nei filtri, puoi condividere questo calendario con altri utenti, che visualizzeranno le proprie attività e i propri problemi incompleti.
