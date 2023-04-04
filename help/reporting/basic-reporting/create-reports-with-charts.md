---
title: Creare rapporti con grafici
description: Scopri come i grafici possono migliorare la visualizzazione dei dati e come utilizzare gli strumenti per grafici in Workfront.
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335153.png
kt: 8860
exl-id: ea3b360b-1fbd-4d1a-b505-b75759d24e41
doc-type: video
source-git-commit: 650e4d346e1792863930dcebafacab4c88f2a8bc
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---

# Creare rapporti con grafici

In questo video imparerai:

* Come i grafici possono migliorare la visualizzazione dei dati
* Come utilizzare gli strumenti per grafici di Workfront

>[!VIDEO](https://video.tv.adobe.com/v/335155/?quality=12&learn=on)

## Attività: Aggiungere un grafico a un report

La fine del trimestre si avvicina e vuoi vedere come i progetti completati di recente sono bloccati ai loro budget. Crea un rapporto che mostri il costo pianificato rispetto al costo effettivo dei progetti. Desideri visualizzare solo i progetti completati nell’ultimo trimestre. Aggiungi un grafico a colonne combinato utilizzando colori personalizzati.

## Risposta

1. Seleziona **[!UICONTROL Rapporti]** dal **[!UICONTROL Menu principale]**.
1. Fai clic sul pulsante **[!UICONTROL Nuovo rapporto]** menu e seleziona **[!UICONTROL Progetto]**.
1. In **[!UICONTROL Colonne (visualizzazione)]** scheda , fai clic su **[!UICONTROL Aggiungi colonna]**.
1. Seleziona [!UICONTROL Progetto] > [!UICONTROL Costo pianificato] e riepilogare questa colonna per **[!UICONTROL Somma]**.
1. Fai clic su **[!UICONTROL Aggiungi colonna]** di nuovo.
1. Seleziona [!UICONTROL Progetto] > [!UICONTROL Costo effettivo] e riepilogare questa colonna per **[!UICONTROL Somma]**.

   ![Immagine della schermata per aggiungere colonne a un report](assets/chart-report-columns.png)

1. In **[!UICONTROL Raggruppamenti]** imposta il rapporto su raggruppa per [!UICONTROL Progetto] > [!UICONTROL Nome].

   ![Immagine della schermata per aggiungere raggruppamenti a un rapporto](assets/chart-report-groupings.png)

1. In **[!UICONTROL Filtri]** , aggiungi due regole di filtro:

   * [!UICONTROL Progetto] > [!UICONTROL Lo Stato Equivale A] > [!UICONTROL Completa]
   * [!UICONTROL Progetto] >[!UICONTROL  Data completamento effettivo] > [!UICONTROL Ultimo trimestre]

   ![Immagine della schermata per aggiungere filtri a un rapporto](assets/chart-report-filters.png)

1. In **[!UICONTROL Grafico]** scheda, scegli **[!UICONTROL Colonna]** per il tipo di grafico.
1. Per [!UICONTROL Asse sinistro (Y)], scegli [!UICONTROL Progetto] > [!UICONTROL Costo pianificato].
1. Per [!UICONTROL Asse inferiore (X)], scegli [!UICONTROL Progetto] > [!UICONTROL Nome].
1. Fai clic sul pulsante **[!UICONTROL Grafico a combinazione]** e seleziona [!UICONTROL Progetto] > [!UICONTROL Costo effettivo] in **[!UICONTROL Valore]** campo .
1. Fare clic sulla freccia accanto alla casella del colore per modificare la [!UICONTROL Costo effettivo] colore. Selezionare uno dei colori visualizzati oppure fare clic sulla casella nell&#39;angolo in basso a destra per visualizzare la palette di colori.
1. Fai clic su **[!UICONTROL Salva e chiudi]**. Quando viene richiesto il nome di un report, chiamalo &quot;Pianificato rispetto al costo effettivo per progetto completato nel trimestre scorso&quot;.

   ![Immagine della schermata per aggiungere un grafico a un report](assets/chart-report-chart.png)
