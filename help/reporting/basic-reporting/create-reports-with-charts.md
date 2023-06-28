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
jira: KT-8860
exl-id: ea3b360b-1fbd-4d1a-b505-b75759d24e41
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---

# Creare rapporti con grafici

Questo video illustra:

* Come i grafici possono migliorare la visualizzazione dei dati
* Come utilizzare gli strumenti per grafici di Workfront

>[!VIDEO](https://video.tv.adobe.com/v/335155/?quality=12&learn=on)

## Attività: aggiungere un grafico a un rapporto

La fine del trimestre è vicina e desideri vedere come i progetti completati di recente si sono attenuti ai loro budget. Crea un report che mostra il costo pianificato rispetto al costo effettivo per i progetti. Desideri visualizzare solo i progetti completati nell’ultimo trimestre. Aggiungere un istogramma combinato utilizzando colori personalizzati.

## Risposta

1. Seleziona **[!UICONTROL Rapporti]** dal **[!UICONTROL Menu principale]**.
1. Fai clic su **[!UICONTROL Nuovo rapporto]** menu e seleziona **[!UICONTROL Progetto]**.
1. In **[!UICONTROL Colonne (visualizzazione)]** , fare clic su **[!UICONTROL Aggiungi colonna]**.
1. Seleziona [!UICONTROL Progetto] > [!UICONTROL Costo Pianificato] e riepiloga questa colonna per **[!UICONTROL Somma]**.
1. Clic **[!UICONTROL Aggiungi colonna]** di nuovo.
1. Seleziona [!UICONTROL Progetto] > [!UICONTROL Costo Reale] e riepiloga questa colonna per **[!UICONTROL Somma]**.

   ![Immagine della schermata per aggiungere colonne a un report](assets/chart-report-columns.png)

1. In **[!UICONTROL Raggruppamenti]** , impostare il report in base al quale eseguire il raggruppamento [!UICONTROL Progetto] > [!UICONTROL Nome].

   ![Immagine della schermata per aggiungere raggruppamenti a un report](assets/chart-report-groupings.png)

1. In **[!UICONTROL Filtri]** , aggiungi due regole di filtro:

   * [!UICONTROL Progetto] > [!UICONTROL Stato equivale a] > [!UICONTROL Completa]
   * [!UICONTROL Progetto] >[!UICONTROL  Data di completamento effettiva] > [!UICONTROL Ultimo Trimestre]

   ![Immagine della schermata per aggiungere filtri a un report](assets/chart-report-filters.png)

1. In **[!UICONTROL Grafico]** , scegli **[!UICONTROL Colonna]** per il tipo di grafico.
1. Per [!UICONTROL Asse (Y) sinistro], scegli [!UICONTROL Progetto] > [!UICONTROL Costo Pianificato].
1. Per [!UICONTROL Asse inferiore (X)], scegli [!UICONTROL Progetto] > [!UICONTROL Nome].
1. Fai clic su **[!UICONTROL Grafico combinato]** e seleziona [!UICONTROL Progetto] > [!UICONTROL Costo Reale] nel **[!UICONTROL Valore]** campo.
1. Fare clic sulla freccia accanto alla casella del colore per modificare [!UICONTROL Costo Reale] colore. Selezionare uno dei colori visualizzati o fare clic sulla casella nell&#39;angolo inferiore destro per visualizzare la tavolozza dei colori.
1. Fai clic su **[!UICONTROL Salva e chiudi]**. Quando viene richiesto il nome di un rapporto, chiamarlo &quot;Costo pianificato vs. Costo effettivo per progetto completato l’ultimo trimestre&quot;.

   ![Immagine della schermata per aggiungere un grafico a un report](assets/chart-report-chart.png)
