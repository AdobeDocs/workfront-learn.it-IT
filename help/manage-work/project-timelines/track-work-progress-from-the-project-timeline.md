---
title: Tracciare l’avanzamento dalla timeline del progetto
description: Scopri come tenere traccia dell’avanzamento del lavoro dalla timeline del progetto in [!DNL  Workfront] utilizzo di percentuale di completamento, stato, assegnazioni o vincoli.
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: track-work-progress-from-the-project-timeline.jpeg
type: Tutorial
role: User
last-substantial-update: 2023-08-16T00:00:00Z
level: Intermediate
jira: KT-10150
exl-id: c8793f49-24b8-48cc-af84-5239234ead0e
source-git-commit: e25a7c0119567c068504edcb8c3ddd29622d52c5
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 0%

---

# Tracciare l’avanzamento dalla timeline del progetto

Assicurarsi che le attività stiano procedendo nel modo desiderato per raggiungere le scadenze del progetto. Durante la scansione [!UICONTROL Attività] , sono disponibili diverse funzioni in [!DNL  Workfront] che consentono di monitorare lo stato di avanzamento e di avanzamento del lavoro.

## Percentuale completata

La percentuale di completamento di ogni attività di lavoro viene talvolta utilizzata per misurare l&#39;avanzamento del lavoro. È importante notare che... questo campo deve essere regolato manualmente, in quanto è la stima dell&#39;assegnatario di quanto sono lunghi.

>[!TIP]
>
>Sebbene sia necessario aggiornare manualmente la percentuale di completamento delle attività di lavoro, la percentuale di completamento di un&#39;attività padre viene calcolata da Workfront in base alla percentuale di completamento e alla durata o alle ore pianificate di ogni attività figlio. Ciò significa che sarà possibile ottenere una maggiore precisione percentuale di completamento se si suddividono attività di grandi dimensioni in sottoattività più piccole.


![Elenco attività progetto visualizzato [!UICONTROL Percentuale completamento] colonna](assets/planner-fund-task-percent-complete.png)

Esistono tre casi in cui la percentuale di completamento cambia automaticamente:

* Quando l&#39;attività [!UICONTROL Stato] è impostato su Completato, la percentuale di completamento diventa 100.
* Se l&#39;attività [!UICONTROL Stato] torna a Nuovo, la percentuale di completamento viene reimpostata su 0.
* In un task padre quando la percentuale di completamento di un task figlio cambia.

## Stato

Includi [!UICONTROL Stato] colonna in a [!UICONTROL Visualizza] per vedere rapidamente quali attività sono state avviate, quali sono in corso e quali sono completate. È anche possibile impostare la formattazione condizionale in un [!UICONTROL Visualizza] per colorare ogni stato, semplificando la decifrazione delle informazioni.

## Assegnazioni attività

Durante la revisione del progetto, esaminare le assegnazioni delle attività. Forse il lavoro è rimasto indietro perché nessuno è stato assegnato all&#39;attività. O forse la persona assegnata non aveva le giuste abilità per completare il lavoro. Aggiungere più persone a un&#39;attività o riassegnare le attività per assicurarsi che il lavoro venga completato.

## Vincolo attività

A volte i vincoli delle attività vengono modificati e non se ne rende conto. I vincoli possono influire sul comportamento della linea temporale, pertanto è necessario assicurarsi che siano impostati nel modo desiderato.

![Elenco attività progetto con colonna vincolo attività](assets/planner-fund-task-constraint.png)

Creare una visualizzazione personalizzata che includa [!UICONTROL Vincolo attività] per visualizzare queste informazioni nell&#39;elenco delle attività. Se il progetto è stato pianificato da una data di inizio, si desidera che le attività abbiano [!UICONTROL Il Prima Possibile] ([!UICONTROL ASAP]).

Per ulteriori dettagli sui vincoli delle attività, vedere [Comprendere e gestire i tipi di durata e i vincoli delle attività](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/manage-work/intermediate-projects/understand-and-manage-duration-types-and-task-constraints.html).
