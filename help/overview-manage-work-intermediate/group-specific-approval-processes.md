---
title: Comprendere i processi di approvazione specifici del gruppo
description: Scopri come gli amministratori di gruppo possono creare o modificare i processi di approvazione per i gruppi che gestiscono.
feature: Approvals
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate
jira: KT-10017
hide: true
exl-id: 9986469c-b02f-48ac-b71e-055473a2855b
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bdid: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-05T19:17:51.764Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 214
ht-degree: 100%

---

# Comprendere i processi di approvazione specifici del gruppo

Sia gli amministratori di sistema che quelli di gruppo possono creare processi di approvazione in [!DNL Workfront]. Gli amministratori di sistema possono creare processi da utilizzare in tutto il sistema di [!DNL Workfront] o solo per un gruppo specifico. Gli amministratori di gruppo possono creare o modificare i processi solo per il gruppo che gestiscono.

Per un processo di approvazione che può essere utilizzato da tutti gli utenti in [!DNL Workfront], assicurati che il campo [!UICONTROL “Questa approvazione è utilizzabile da”] sia impostato su [!UICONTROL Tutti i gruppi].

Finestra ![[!UICONTROL Modifica processo di approvazione] con campo gruppo evidenziato](assets/admin-fund-approval-processes-1.png)

Gli stati disponibili nel menu [!UICONTROL “Avvia il processo di approvazione quando lo stato è impostato su”] dipendono dalla selezione nel campo “utilizzato da”. Se il campo [!UICONTROL Tutti i gruppi] è selezionato, sono disponibili solo gli stati di blocco a livello di sistema.

Per limitare un processo di approvazione per un gruppo specifico, seleziona il nome del gruppo dall’elenco per il campo [!UICONTROL “Questa approvazione è utilizzabile da”].

Finestra ![[!UICONTROL Modifica processo di approvazione] con campo gruppo espanso](assets/admin-fund-approval-processes-2.png)

L’opzione [!UICONTROL Tutti i gruppi] non è disponibile per gli amministratori di gruppo.

Quando viene selezionato un gruppo specifico, nel menu [!UICONTROL “Avvia il processo di approvazione quando lo stato è impostato su”] vengono visualizzati solo gli stati disponibili per tale gruppo.

Finestra ![[!UICONTROL Modifica processo di approvazione] con campo di stato evidenziato](assets/admin-fund-approval-processes-3.png)
