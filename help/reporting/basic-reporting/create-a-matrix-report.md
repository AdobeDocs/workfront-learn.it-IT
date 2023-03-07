---
title: Creare un rapporto matrice
description: Scopri quando un rapporto matrice può essere utile e come crearlo in Workfront.
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335156.png
kt: 8861
exl-id: e893d94a-e808-4bc1-bc6e-f46a5582b55d
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---

# Creare un rapporto matrice

Questo video illustra:

* Quando un report matrice può essere utile
* E come creare un rapporto matrice

>[!VIDEO](https://video.tv.adobe.com/v/335156/?quality=12)

## Attività: creare un rapporto matrice

Crea un report matrice che mostra il numero di richieste in ogni stato, ordinate in base alla coda di richieste. Questo offre un’istantanea rapida della quantità di lavoro in arrivo e di come te la stai tenendo al passo.

Si desidera che le code di richieste vengano visualizzate nei raggruppamenti di righe. Lo stato viene visualizzato come raggruppamenti di colonne. Denomina il rapporto &quot;Richieste per stato e Coda richieste&quot;.

## Risposta

1. Seleziona **[!UICONTROL Rapporti]** dal **[!UICONTROL Menu principale]**.
1. Fai clic su **[!UICONTROL Nuovo rapporto]** e seleziona **[!UICONTROL Problema]**.
1. Vai a **[!UICONTROL Raggruppamenti]** e fai clic su **[!UICONTROL Passa al raggruppamento di matrici]**.
1. Per [!UICONTROL Raggruppamenti di righe], seleziona **[!UICONTROL Progetto]** > **[!UICONTROL Nome]**.
1. Per [!UICONTROL Raggruppamento colonne], seleziona **[!UICONTROL Problema]** > **[!UICONTROL Stato]**.

   ![Immagine della schermata per creare un nuovo raggruppamento di rapporti sui problemi](assets/matrix-report-groupings.png)

1. Vai a **[!UICONTROL Filtri]** scheda.
1. Per assicurarsi di visualizzare solo le richieste nelle code di richieste attive, aggiungi le seguenti regole di filtro:

   * [!UICONTROL Progetto] > [!UICONTROL Stato equivale a] > [!UICONTROL Uguale] > [!UICONTROL Corrente]
   * [!UICONTROL Definizione coda] > [!UICONTROL È pubblico] > [!UICONTROL Not Equal] > [!UICONTROL Nessuno] (Questo è il modo in cui sappiamo che un progetto è in realtà una coda di richieste, poiché la Definizione della coda viene assegnata a una delle opzioni pubbliche).

1. Fai clic su **[!UICONTROL Salva e chiudi]**. Quando viene richiesto il nome di un report, digitare &quot;Richieste per stato e Coda richieste&quot;.

   ![Immagine della schermata per creare un nuovo filtro per la segnalazione dei problemi](assets/matrix-report-filters.png)
