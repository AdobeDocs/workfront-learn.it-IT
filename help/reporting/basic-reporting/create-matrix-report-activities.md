---
title: Creare attività di report matrice
description: Esercitarsi a creare rapporti matrice con istruzioni dettagliate.
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335156.png
jira: KT-8861
hidefromtoc: true
source-git-commit: 915b28bbbf138fa84dce6d1915387fbe22c63362
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 66%

---

# Creare attività di report matrice

Esercitarsi a creare rapporti matrice con istruzioni dettagliate.

## Attività 1: creare un rapporto matrice

Crea un rapporto matrice che mostri quante richieste sono presenti in ogni stato, ordinate per coda di richieste. Questo offre un’istantanea rapida della quantità di lavoro in arrivo e del modo in cui te la stai tenendo al passo.

Desideri che le code di richiesta vengano visualizzate nei raggruppamenti di righe. Lo stato viene visualizzato come raggruppamenti di colonne. Denomina il rapporto &quot;Richieste per stato e Coda richieste&quot;.

## Risposta 1

1. Seleziona **[!UICONTROL Rapporti]** dal **[!UICONTROL Menu principale]**.
1. Fai clic sull’opzione **[!UICONTROL Nuovo rapporto]** e seleziona **[!UICONTROL Problema]**.
1. Passa alla scheda **[!UICONTROL Raggruppamenti]** e fai clic su **[!UICONTROL Passa al raggruppamento di matrici]**.
1. Per [!UICONTROL Raggruppamenti righe], seleziona **[!UICONTROL Progetto]** > **[!UICONTROL Nome]**.
1. Per [!UICONTROL Raggruppamento colonne], seleziona **[!UICONTROL Problema]** > **[!UICONTROL Stato]**.

   ![Immagine della schermata per creare un nuovo raggruppamento di rapporti sui problemi](assets/matrix-report-groupings.png)

1. Passa alla scheda **[!UICONTROL Filtri]**.
1. Per assicurarti di visualizzare solo le richieste nelle code di richieste attive, aggiungi le seguenti regole di filtro:

   * [!UICONTROL Progetto] > [!UICONTROL Stato equivale a] > [!UICONTROL Uguale a] > [!UICONTROL Corrente]
   * [!UICONTROL Definizione coda] > [!UICONTROL È pubblico] > [!UICONTROL Non uguale a] > [!UICONTROL Nessuno] (Questo è il modo in cui sappiamo che un progetto è in realtà una coda di richieste, poiché la Definizione della coda viene assegnata a una delle opzioni pubbliche).

1. Fai clic su **[!UICONTROL Salva Chiudi]**. Quando viene richiesto il nome di un report, digitare &quot;Richieste per stato e Coda richieste&quot;.

   ![Immagine della schermata per creare un nuovo filtro per la segnalazione dei problemi](assets/matrix-report-filters.png)
