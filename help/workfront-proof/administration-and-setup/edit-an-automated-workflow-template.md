---
title: Modificare un modello di workflow automatizzato
description: Scopri come apportare modifiche a un modello di flusso di lavoro per la verifica automatica esistente in [!DNL  Workfront].
activity: use
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
team: Technical Marketing
thumbnail: 335131.png
jira: KT-8831
exl-id: 03841b1f-741d-4427-ae84-ddb9f890fc95
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '581'
ht-degree: 0%

---

# Modificare un modello di workflow automatizzato

Man mano che i processi di revisione e approvazione delle bozze vengono perfezionati o che vengono apportate modifiche organizzative, i modelli di flusso di lavoro automatizzati devono essere aggiornati per riflettere le operazioni correnti dei team che utilizzano Workfront.

Mantenere aggiornati i modelli garantisce la coerenza dei processi di revisione e approvazione, oltre a risparmiare tempo a coloro che caricano le bozze, perché non devono modificare costantemente un flusso di lavoro.

1. Seleziona **[!UICONTROL Bozza]** dal **[!UICONTROL Menu principale]** in [!DNL Workfront].
1. Da qui, seleziona **[!UICONTROL Flussi di lavoro]** nel menu del pannello sinistro.
1. Fai clic sul menu a 3 punti all’estrema destra del nome del modello e seleziona **[!UICONTROL Visualizza dettagli modello]**.

Le opzioni per la condivisione, la copia e l&#39;eliminazione del modello si trovano nella parte superiore della finestra dei dettagli del modello per ogni modello. L’eliminazione di un modello non influisce sulle bozze in corso a cui è applicato tale modello, ma significa che il modello non è più disponibile per l’uso.

![Finestra Dettagli modello](assets/proof-system-setup-edit-templates-details-area.png)

<!--
Lean More URLs
-->

Fare clic sulla freccia per espandere [!UICONTROL Dettagli] per modificare elementi quali il nome del modello o il fuso orario del modello.

## Apportare modifiche agli stadi e ai destinatari

Potrebbero essere necessarie modifiche in [!UICONTROL Flusso di lavoro] area in cui per processo semplificato si intende una scadenza precedente o quando qualcuno si unisce al team e rivedrà le bozze.

Ogni fase di un flusso di lavoro automatizzato ha una propria sezione, che consente di modificare in modo indipendente scadenze, privacy, destinatari della bozza e altre informazioni.

Questo video illustra brevemente alcune delle modifiche che è possibile apportare al [!UICONTROL Flusso di lavoro] area. Consulta l’elenco puntato in questo video, che esamina queste impostazioni. Nessun audio in questo video.

>[!VIDEO](https://video.tv.adobe.com/v/335131/?quality=12&learn=on)

In qualità di revisione, ecco le modifiche che puoi apportare al modello di bozza nel [!UICONTROL Flusso di lavoro] sezione:

* Fai clic su nella [!UICONTROL nome fase] o il [!UICONTROL scadenza] per aggiornare tali informazioni.
* Seleziona la freccia accanto al simbolo [!UICONTROL scadenza] per bloccare la fase, determinare quando è attivata o richiedere una sola decisione.
* Nell’elenco dei destinatari, fai clic su nella [!UICONTROL Ruolo] o [!UICONTROL Avvisi e-mail] per selezionare un&#39;altra opzione.
* Vai al menu a 3 punti all’estrema destra del nome di un destinatario per eliminarlo dall’elenco, renderlo il decisore principale per quella fase del flusso di lavoro, o modifica il ruolo della bozza e le informazioni dell’avviso e-mail.
* Sono disponibili due opzioni per aggiungere i destinatari all’elenco. Dopo aver aperto [!UICONTROL Aggiungi persone all&#39;area di visualizzazione] fare clic sulla fase a cui aggiungerli. Quindi inserisci il loro nome o indirizzo e-mail nell’elenco dei destinatari e assegna un ruolo bozza e un avviso e-mail. Fai clic su [!UICONTROL Aggiungi persone] al termine dell’operazione.
   1. Nell&#39;angolo in alto a destra di ogni sezione di stage, vai al [!UICONTROL Altro] menu e seleziona [!UICONTROL Aggiungi persone all&#39;area di visualizzazione].
   1. Nella parte superiore della sezione [!UICONTROL Flusso di lavoro] area, seleziona [!UICONTROL Aggiungi persone all&#39;area di visualizzazione].

## Condivisione dei modelli

Il [!UICONTROL Condiviso con] area visualizza gli utenti della bozza che possono utilizzare il modello. Per rimuovere gli utenti che non devono più utilizzare il modello, fai clic sul menu a 3 punti all’estrema destra del nome e seleziona [!UICONTROL Rimuovi].

![[!UICONTROL Condiviso con] list](assets/proof-system-setups-edit-template-shared-with.png)

Tuttavia, non è possibile aggiungere persone all&#39;elenco di condivisione da questa sezione. A questo scopo, torna all’inizio della finestra dei dettagli del modello e fai clic su [!UICONTROL Condividi modello] pulsante.

## Sezione attività

[!DNL Workfront] conserva una cronologia di audit relativa a quando sono state apportate modifiche al modello. Puoi vedere la data, chi ha apportato la modifica e alcune brevi informazioni su quali modifiche sono state apportate.

Questa sezione non registra informazioni su quando il modello è stato utilizzato sulle bozze.

![Elenco attività bozza](assets/proof-system-setups-edit-template-activity.png)
