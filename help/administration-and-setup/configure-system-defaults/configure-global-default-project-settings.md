---
title: Configurare le impostazioni globali predefinite del progetto
description: Scopri come modificare uno stato personalizzato, impostare le preferenze globali del progetto e creare pianificazioni che sono impostazioni globali predefinite.
feature: System Setup and Administration
role: Admin
level: Intermediate
activity: deploy
type: Tutorial
team: Technical Marketing
thumbnail: 335065.png
jira: KT-8753
exl-id: b961ba8c-9597-4ed4-a6d7-79689c8e290d
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 0%

---

# Configurare le impostazioni globali predefinite del progetto

<!---
21.4 updates have been made
--->

Questo video illustra come:

* Modificare uno stato personalizzato
* Impostare le preferenze globali del progetto
* Creare e utilizzare pianificazioni

>[!VIDEO](https://video.tv.adobe.com/v/335065/?quality=12&learn=on)

## Impostazioni globali e di gruppo per progetti, attività e problemi

All&#39;apertura di [!UICONTROL Progetti] impostazioni in [!DNL Workfront], noterai che dice &quot;[!UICONTROL Preferenze progetto di sistema]&quot; nella barra di ricerca nella parte superiore della finestra. Questo consente di sapere che queste impostazioni interessano tutti gli utenti [!DNL Workfront] sistema: è una configurazione globale.

![[!UICONTROL Preferenze progetto] pagina in [!UICONTROL Configurazione]](assets/admin-fund-system-project-preferences-1.png)

Quando apri il modulo potrai vedere qualcosa di simile. [!UICONTROL Attività e problemi] impostazioni.

![[!UICONTROL Preferenze attività e problemi] in [!UICONTROL Configurazione]](assets/admin-fund-task-issue-preferences-2.png)

Tuttavia, è possibile che non tutti [!DNL Workfront] ha bisogno delle stesse preferenze per progetto, attività e problema. Ad esempio, il gruppo marketing desidera che lo stato di un nuovo progetto sia Pianificazione, mentre il gruppo project manager preferisce lo stato Richiesta.

[!DNL Workfront] consente agli amministratori di gruppi di regolare alcune preferenze di progetto, attività e problema per i loro gruppi. Quali preferenze possono essere modificate sono determinate dal [!DNL Workfront] dell&#39;amministratore di sistema utilizzando le opzioni di blocco/sblocco.

Per iniziare, accedi al [!UICONTROL Configurazione] area:

1. Seleziona **[!UICONTROL Configurazione]** nel **[!UICONTROL Menu principale]**.
1. Espandi **[!UICONTROL Preferenze progetto]** nel menu a sinistra.
1. Seleziona **[!UICONTROL Progetti]** o **[!UICONTROL Attività e problemi]**, a seconda delle impostazioni da modificare.

Bloccare una preferenza per impedire agli amministratori di gruppi di modificare tale impostazione per il proprio gruppo.

![Messaggio di preferenza Bloccato](assets/admin-fund-preferences-locked-3.png)

Sblocca la preferenza per renderla disponibile agli amministratori di gruppi per la personalizzazione.

![Messaggio di preferenza sbloccato](assets/admin-fund-preferences-unlocked-4.png)

Alcune impostazioni non possono essere sbloccate e rimangono impostazioni di sistema globali.

![Messaggio di preferenza Bloccato](assets/admin-fund-preferences-always-locked-5.png)

### Impostare le preferenze di gruppo e sottogruppo

Per qualsiasi impostazione sbloccata dall’amministratore di sistema, gli amministratori dei gruppi possono apportare modifiche ai gruppi da loro gestiti ed ai sottogruppi nidificati in tali gruppi. Inoltre, gli amministratori dei gruppi possono controllare le impostazioni che i loro amministratori dei sottogruppi possono modificare.

1. Seleziona **[!UICONTROL Configurazione]** nel **[!UICONTROL Menu principale]**.
1. Clic **[!DNL Groups]** nel menu a sinistra.
1. Fare clic sul nome del gruppo o del sottogruppo per aprirlo.
1. Seleziona **[!UICONTROL Preferenze progetto]** o **[!UICONTROL Preferenze attività e problemi]** nel menu a sinistra.
1. Apporta le modifiche necessarie per ciascuna delle preferenze sbloccate.
1. Seleziona **[!UICONTROL Salva]**.

![[!UICONTROL Stato progetto] sezione su [!UICONTROL Gruppo] pagina](assets/admin-fund-group-preferences.png)

Se l’organizzazione non utilizza gli amministratori di gruppi, l’amministratore di sistema può gestire le impostazioni delle preferenze per i diversi gruppi.

<!---
learn more URLs and guides
Create or edit a group status 
Group administrators 
Configure system-wide project preferences 
Configure project preferences for a group 
Configure task and issue preferences for a group 
Create and modify a group’s schedule 
--->
