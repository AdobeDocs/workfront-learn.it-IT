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
exl-id: 138989b2-32d7-43e5-9660-d7b4172f232a
TQID: https://experienceleague.adobe.com/PcQL0NTo4cz4jEOXcQ-48tXu8Zr5U-BsbAx9hKn20Tk
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 36674ed53c8645f556862bb2d99f3bfd6c993c1e
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

