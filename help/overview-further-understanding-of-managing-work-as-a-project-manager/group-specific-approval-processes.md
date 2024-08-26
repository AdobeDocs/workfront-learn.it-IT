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
source-git-commit: 2351b6ff9977fd8a81289ab2fad28e21322d347e
workflow-type: tm+mt
source-wordcount: '212'
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

