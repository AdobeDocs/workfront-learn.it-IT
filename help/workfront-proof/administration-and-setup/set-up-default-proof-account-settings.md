---
title: Imposta le impostazioni predefinite dell’account della bozza
description: Scopri come impostare impostazioni account predefinite da applicare globalmente a tutti gli utenti di bozze e verifiche .
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
thumbnail: set-up-proof-actual-default-settings.png
jira: KT-10236
last-substantial-update: 2024-01-23T00:00:00Z
exl-id: 6eda8bcd-ab0f-4e02-9080-64b6051b327f
source-git-commit: 731005176bc02e3a4d26d00373931fa7444afeea
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 0%

---

# Imposta le impostazioni predefinite dell’account della bozza

Definisci le impostazioni account predefinite da applicare globalmente a tutti gli utenti di bozze e bozze: paese, lingua e fuso orario. Se gli utenti dispongono di più fusi orari o paesi, puoi modificare queste impostazioni sul profilo utente di ogni singolo utente, se necessario.

![Finestra Impostazioni account per la verifica](assets/proof-system-setups-default-account-settings.png)

1. Seleziona **[!UICONTROL Bozza]** da [!DNL Workfront's] [!UICONTROL Menu principale].
1. Seleziona **[!UICONTROL Impostazioni account]** nella barra di navigazione superiore.
1. Seleziona la **[!UICONTROL Dettagli]** scheda.
1. Vai a [!UICONTROL Paese] e seleziona **[!UICONTROL Modifica]**. Scegli il paese in cui si trovano la maggior parte degli utenti di bozze come impostazione predefinita.
1. Seleziona **[!UICONTROL Salva]** per tale impostazione.
1. Vai a [!UICONTROL Lingua predefinita] e seleziona **[!UICONTROL Modifica]**. Scegli la lingua predefinita dalla maggior parte degli utenti di verifica.
1. Seleziona **[!UICONTROL Salva]** per tale impostazione.
1. Vai a [!UICONTROL Fuso orario predefinito] e seleziona **[!UICONTROL Modifica]**. Scegli il fuso orario predefinito in cui si troveranno la maggior parte degli utenti di verifica. Questo sarà il fuso orario riconosciuto dai flussi di lavoro bozza configurati manualmente. Si applica anche ai modelli di flusso di lavoro della bozza, ma per ogni modello può essere impostato un fuso orario.
1. Seleziona **[!UICONTROL Salva]** per tale impostazione.

## Best practice


| Best practice | Ecco perché |
|---|---|
| Regola le impostazioni di back-end della bozza in modo che gli utenti possano visualizzare le scadenze in un formato di orologio di 12 ore. | Seleziona l’opzione F j, Y, gi:a nelle impostazioni della bozza per gli utenti che desiderano visualizzare le scadenze/ore della bozza in formato AM/PM. Per le aree che utilizzano un orologio da 12 ore, questo aiuta a chiarire le scadenze. <br> <br>Nota: per trovare questa impostazione, vai al menu principale di Workfront > Strumenti di correzione > Impostazioni account > Utenti > e modifica il campo Formato data per ogni utente. |
| Stabilisci una scadenza predefinita per la bozza come parte delle impostazioni di sistema. | Quando viene impostata una scadenza predefinita della bozza (data di caricamento + x numero di giorni lavorativi), se il creatore della bozza dimentica di aggiungere una scadenza, Workfront la applica automaticamente a ogni bozza caricata. <br> <br>Nota: per trovare questa impostazione, vai al campo Menu principale di Workfront > Strumenti di correzione > Impostazioni account > Impostazioni > Impostazioni bozza > Scadenza (+ giorni lavorativi). |
| Nascondi l’opzione di decisione Bozza non rilevante. | Questa opzione di decisione causa spesso confusione tra gli approvatori, in quanto spesso le organizzazioni non definiscono quando utilizzare l’opzione Non pertinente. L’opzione Non pertinente indica in genere che la bozza non è pertinente per il destinatario della bozza e che non è necessario che prenda una decisione approvata o rifiutata. Selezionando Non pertinente, puoi continuare il flusso di lavoro della bozza.<br> <br>L’opzione Non rilevante non è necessaria nella maggior parte dei flussi di lavoro per bozze.<br> <br>Nota: per trovare questa impostazione, vai al menu principale di Workfront > Strumenti di correzione > Impostazioni account > Decisioni. |
| Non riordinare le opzioni di decisione bozza nelle impostazioni bozza. | Ogni impostazione di decisione della bozza contiene un valore/peso specifico che, se riordinato, può generare confusione nelle configurazioni della bozza. L’ordine di decisione e il valore/peso vengono utilizzati come attivatori della fase di bozza e nel reporting.<br> <br>Nota: per trovare questa impostazione, vai al menu principale di Workfront > Strumenti di correzione > Impostazioni account > Decisioni. |
| Impostazione delle impostazioni predefinite per i ruoli delle bozze e gli avvisi e-mail. | Queste impostazioni si popolano automaticamente durante l’assegnazione di un flusso di lavoro della bozza, velocizzando il processo e contribuendo alla coerenza tra i flussi di lavoro della bozza.<br> <br>Nota: per trovare le impostazioni predefinite dell’utente, vai al menu principale di Workfront > Strumenti di correzione > Impostazioni account > Utenti > e seleziona l’utente per il quale impostare le impostazioni predefinite. |
