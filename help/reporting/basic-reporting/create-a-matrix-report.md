---
title: Creare un rapporto sulla matrice
description: Scopri quando un rapporto sulla matrice può essere utile e come creare un rapporto sulla matrice in Workfront.
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335156.png
kt: 8861
exl-id: e893d94a-e808-4bc1-bc6e-f46a5582b55d
source-git-commit: 252ba3ba44f22519a35899fcda9c6bca597a6c2c
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---

# Creare un rapporto sulla matrice

In questo video imparerai:

* Quando un rapporto di matrice può essere utile
* E come creare un rapporto sulla matrice

>[!VIDEO](https://video.tv.adobe.com/v/335156/?quality=12)

## Attività: Creare un rapporto sulla matrice

Crea un rapporto di matrice che mostra quante richieste ci sono in ogni stato, ordinate per coda di richiesta. Questo ti offre un rapido quadro della quantità di lavoro in arrivo e di come ti stai adeguando.

Le code di richiesta devono essere visualizzate sui raggruppamenti di righe. Lo stato viene visualizzato come raggruppamento di colonne. Denomina il report &quot;Richieste per stato e coda richieste&quot;.

## Risposta

1. Seleziona **[!UICONTROL Rapporti]** dal **[!UICONTROL Menu principale]**.
1. Fai clic sul pulsante **[!UICONTROL Nuovo rapporto]** e seleziona **[!UICONTROL Problema]**.
1. Vai a **[!UICONTROL Raggruppamenti]** e fai clic su **[!UICONTROL Passa al raggruppamento a matrice]**.
1. Per [!UICONTROL Raggruppamenti di righe], seleziona **[!UICONTROL Progetto]** > **[!UICONTROL Nome]**.
1. Per [!UICONTROL Raggruppamento colonne], seleziona **[!UICONTROL Problema]** > **[!UICONTROL Stato]**.

   ![Immagine della schermata per creare un nuovo raggruppamento di rapporti sui problemi](assets/matrix-report-groupings.png)

1. Vai a **[!UICONTROL Filtri]** scheda .
1. Per assicurarti di vedere solo le richieste nelle code di richiesta attive, aggiungi le seguenti regole di filtro:

   * [!UICONTROL Progetto] > [!UICONTROL Lo Stato Equivale A] > [!UICONTROL Uguale] > [!UICONTROL Corrente]
   * [!UICONTROL Definizione coda] > [!UICONTROL È pubblico] > [!UICONTROL Diverso] > [!UICONTROL Nessuno] Questo è il modo in cui sappiamo che un progetto è in realtà una coda di richiesta, in quanto la Definizione della coda viene assegnata a una delle opzioni pubbliche.

1. Fai clic su **[!UICONTROL Salva e chiudi]**. Quando viene richiesto il nome di un report, digitare &quot;Richieste per stato e coda richieste&quot;.

   ![Immagine della schermata per creare un nuovo filtro per la segnalazione dei problemi](assets/matrix-report-filters.png)
