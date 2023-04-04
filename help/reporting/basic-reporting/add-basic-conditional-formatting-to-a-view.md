---
title: Aggiungi formattazione condizionale di base
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
source-git-commit: 650e4d346e1792863930dcebafacab4c88f2a8bc
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# Aggiungere formattazione condizionale di base a una visualizzazione

La formattazione condizionale viene eseguita creando regole di colonna. Le regole colonna consentono di formattare una colonna in un modo specifico in base ai criteri impostati.

In questo video imparerai:

* Visualizzazione della formattazione condizionale
* Come creare e modificare la formattazione condizionale

>[!VIDEO](https://video.tv.adobe.com/v/335149/?quality=12&learn=on)

## Attività: Aggiungere formattazione condizionale a una visualizzazione

Creare una visualizzazione attività denominata &quot;Standard + Avanzamento&quot; utilizzando la visualizzazione Standard esistente e aggiungendo la formattazione condizionale [!UICONTROL Nome] colonna.

1. Aggiungi una regola di colonna che diventerà rossa lo sfondo del campo quando lo stato di avanzamento dell’attività è in ritardo.
1. Aggiungi una regola di colonna per giallo di sfondo del campo quando lo stato di avanzamento è Behind o At Risk (Dietro o A rischio).

Questo ti aiuterà a individuare le attività con problemi senza includere nella tua visualizzazione la colonna per lo stato di avanzamento.

## Risposta

![Immagine della schermata per creare una nuova regola di colonna](assets/conditional-formatting-exercise.png)

1. In un rapporto dell&#39;elenco delle attività, passare alla sezione **[!UICONTROL Visualizza]** menu a discesa e seleziona **[!UICONTROL Nuova vista]**.
1. Denomina la visualizzazione &quot;Standard + Progress&quot;.
1. Utilizza le colonne predefinite fornite.
1. Seleziona la [!UICONTROL Nome attività] colonna. Questa è la colonna a cui si desidera applicare la formattazione condizionale, in modo che venga visualizzata in rosso o giallo se lo stato di avanzamento dell’attività non è In tempo.
1. Fai clic su **[!UICONTROL Opzioni avanzate]** nell’angolo in alto a destra della finestra del generatore di report.
1. Fai clic su **[!UICONTROL Aggiungi una regola per questa colonna]**.
1. Avvia la regola della colonna modificando [!UICONTROL Attività] > [!UICONTROL Nome] nella parte superiore della finestra [!UICONTROL Attività] > [!UICONTROL Stato di avanzamento]. Fai clic sul pulsante **[!UICONTROL X]** accanto a [!UICONTROL Attività] > [!UICONTROL Nome] per eliminarlo dal campo.
1. Digita &quot;progress&quot; nel campo , quindi seleziona [!UICONTROL Stato di avanzamento] in [!UICONTROL Attività] origine del campo.
1. Seleziona **[!UICONTROL In ritardo]** nel campo a destra del [!UICONTROL Uguale] qualificatore.
1. Scegli uno sfondo rosso nella sezione [!UICONTROL Colore testo] fila.
1. Fai clic su **[!UICONTROL Aggiungi regola]** per salvare la regola colonna.
1. Ora fai clic su **[!UICONTROL Aggiungi regola colonna]** per aggiungere un&#39;altra regola.
1. Come prima, elimina [!UICONTROL Attività] > [!UICONTROL Nome] dal campo criteri . Sostituisci con [!UICONTROL Stato di avanzamento] in [!UICONTROL Attività] origine del campo.
1. Seleziona entrambi [!UICONTROL A rischio] e [!UICONTROL Dietro] nel campo a destra del qualificatore Equal.
1. Scegli uno sfondo giallo nel [!UICONTROL Colore testo] fila.
1. Fai clic su **[!UICONTROL Aggiungi regola]** per salvare la regola colonna.
1. Fai clic su **[!UICONTROL Salva visualizzazione]** per salvare la visualizzazione.
