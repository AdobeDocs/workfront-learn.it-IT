---
title: Creare rapporti con le attività dei grafici
description: Esercitarsi a creare report con grafici, con istruzioni dettagliate.
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335153.png
jira: KT-8860
hidefromtoc: true
source-git-commit: 915b28bbbf138fa84dce6d1915387fbe22c63362
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 81%

---

# Creare rapporti con le attività dei grafici

Esercitarsi a creare report con grafici, con istruzioni dettagliate.

## Attività 1: aggiungere un grafico a un rapporto

La fine del trimestre è vicina e desideri vedere se è stato rispettato il budget dei progetti completati di recente. Crea un report che mostri il costo pianificato rispetto al costo effettivo dei progetti. Desideri visualizzare solo i progetti completati nell’ultimo trimestre. Aggiungi un istogramma combinato utilizzando colori personalizzati.

## Risposta 1

1. Seleziona **[!UICONTROL Rapporti]** dal **[!UICONTROL Menu principale]**.
1. Fai clic sul menu **[!UICONTROL Nuovo rapporto]** e seleziona **[!UICONTROL Progetto]**.
1. Nella scheda **[!UICONTROL Colonne (Visualizzazione)]**, fai clic su **[!UICONTROL Aggiungi colonna]**.
1. Seleziona [!UICONTROL Progetto] > [!UICONTROL Costo pianificato] e riepiloga questa colonna per **[!UICONTROL Somma]**.
1. Fai di nuovo clic su **[!UICONTROL Aggiungi colonna]**.
1. Seleziona [!UICONTROL Progetto] > [!UICONTROL Costo effettivo] e riepiloga questa colonna per **[!UICONTROL Somma]**.

   ![Immagine della schermata per aggiungere colonne a un rapporto](assets/chart-report-columns.png)

1. Nella scheda **[!UICONTROL Raggruppamenti]**, imposta il rapporto in base al quale eseguire il raggruppamento per [!UICONTROL Progetto] > [!UICONTROL Nome].

   ![Immagine della schermata per aggiungere raggruppamenti a un rapporto](assets/chart-report-groupings.png)

1. Nella scheda **[!UICONTROL Filtri]**, aggiungi due regole di filtro:

   * [!UICONTROL Progetto] > [!UICONTROL Stato equivale a] > [!UICONTROL Completato]
   * [!UICONTROL Progetto] > [!UICONTROL  Data di completamento effettiva] > [!UICONTROL Ultimo Trimestre]

   ![Immagine della schermata per aggiungere filtri a un rapporto](assets/chart-report-filters.png)

1. Nella scheda **[!UICONTROL Grafico]**, scegli **[!UICONTROL Colonna]** per il tipo di grafico.
1. Per [!UICONTROL Asse sinistro (Y)], scegli [!UICONTROL Progetto] > [!UICONTROL Costo pianificato].
1. Per [!UICONTROL Asse inferiore (X)], scegli [!UICONTROL Progetto] > [!UICONTROL Nome].
1. Fai clic sul pulsante **[!UICONTROL Grafico combinato]** e seleziona [!UICONTROL Progetto] > [!UICONTROL Costo effettivo] nel campo **[!UICONTROL Valore]**.
1. Fai clic sulla freccia accanto alla casella del colore per cambiare il colore di [!UICONTROL Costo effettivo]. Seleziona uno dei colori visualizzati o fai clic sulla casella nell’angolo in basso a destra per visualizzare la tavolozza dei colori.
1. Fai clic su **[!UICONTROL Salva + Chiudi]**. Quando viene richiesto il nome di un rapporto, chiamarlo &quot;Costo pianificato vs. Costo effettivo per progetto completato l’ultimo trimestre&quot;.

   ![Immagine della schermata per aggiungere un grafico a un rapporto](assets/chart-report-chart.png)
