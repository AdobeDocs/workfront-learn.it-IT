---
title: Aggiungere formattazione condizionale di base
description: Scopri come utilizzare le regole di colonna per modificare il colore del testo, la formattazione e i colori di sfondo in un rapporto o in una visualizzazione, in base ai criteri impostati.
activity: use
feature: Reports and Dashboards
thumbnail: 335149.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
kt: 8855
exl-id: bf9a4cf4-b073-4f7e-8516-e7843f4dc20f
doc-type: video
source-git-commit: 0ee80dceb8208bd0360fd8c9ab68fb8a73677a9d
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 0%

---

# Aggiungere formattazione condizionale di base a una visualizzazione

La formattazione condizionale viene eseguita creando regole di colonna. Le regole di colonna consentono di formattare una colonna in modo specifico in base ai criteri impostati.

Questo video illustra:

* Definizione della formattazione condizionale in una visualizzazione
* Come creare e modificare la formattazione condizionale

>[!VIDEO](https://video.tv.adobe.com/v/335149/?quality=12&learn=on)

## Riepilogo

Per creare la formattazione condizionale:

1. Scegliere la colonna in cui visualizzare la formattazione
1. Decidere quali condizioni modificare la formattazione
1. Decidere quale tipo di modifica della formattazione funzionerà meglio

   * colore di sfondo
   * colore del testo
   * testo sostitutivo
   * mostra un&#39;icona

## Attività: aggiungere la formattazione condizionale a una visualizzazione

Creare una visualizzazione delle attività denominata &quot;Standard + Avanzamento&quot; utilizzando la visualizzazione Standard esistente e aggiungendo questa formattazione condizionale alla [!UICONTROL Nome] colonna.

1. Aggiungi una regola di colonna che attivi lo sfondo del campo in rosso quando lo stato di avanzamento dell’attività è In ritardo.
1. Aggiungi una regola di colonna che girerà in giallo lo sfondo del campo quando lo stato di avanzamento è Indietro o A rischio.

Ciò consente di individuare le attività con problemi senza includere nella visualizzazione la colonna relativa allo stato di avanzamento.

## Risposta

![Immagine della schermata per creare una nuova regola di colonna](assets/conditional-formatting-exercise.png)

1. In un report elenco attività, passare alla **[!UICONTROL Visualizza]** menu a discesa e selezionare **[!UICONTROL Nuova visualizzazione]**.
1. Denomina la visualizzazione &quot;Standard + Progress&quot;.
1. Utilizza le colonne predefinite fornite.
1. Seleziona la [!UICONTROL Nome attività] colonna. Questa è la colonna a cui si desidera applicare la formattazione condizionale, pertanto appare rossa o gialla se lo stato di avanzamento dell&#39;attività non è On Time.
1. Clic **[!UICONTROL Opzioni avanzate]** nell’angolo in alto a destra della finestra di report builder.
1. Clic **[!UICONTROL Aggiungi una regola per questa colonna]**.
1. Avvia la regola di colonna modificando [!UICONTROL Attività] > [!UICONTROL Nome] nella parte superiore della finestra per [!UICONTROL Attività] > [!UICONTROL Stato di avanzamento]. Fai clic sul pulsante **[!UICONTROL X]** icona accanto a [!UICONTROL Attività] > [!UICONTROL Nome] per eliminarlo dal campo.
1. Digita &quot;progress&quot; nel campo, quindi seleziona [!UICONTROL Stato di avanzamento] sotto [!UICONTROL Attività] origine del campo.
1. Seleziona **[!UICONTROL In Ritardo]** nel campo a destra della [!UICONTROL Uguale] qualificatore.
1. Scegli uno sfondo rosso nel [!UICONTROL Colore testo] riga.
1. Clic **[!UICONTROL Aggiungi regola]** per salvare la regola di colonna.
1. Ora fai clic su **[!UICONTROL Aggiungi regola colonna]** per aggiungere un&#39;altra regola.
1. Come prima, elimina [!UICONTROL Attività] > [!UICONTROL Nome] dal campo criteri. Sostituiscilo con [!UICONTROL Stato di avanzamento] sotto [!UICONTROL Attività] origine del campo.
1. Seleziona entrambi [!UICONTROL A Rischio] e [!UICONTROL Dietro] nel campo a destra del qualificatore Uguale.
1. Scegli uno sfondo giallo nel [!UICONTROL Colore testo] riga.
1. Clic **[!UICONTROL Aggiungi regola]** per salvare la regola di colonna.
1. Clic **[!UICONTROL Salva visualizzazione]** per salvare la visualizzazione.
