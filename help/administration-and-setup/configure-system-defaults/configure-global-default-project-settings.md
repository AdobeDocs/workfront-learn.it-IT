---
title: Configurare le impostazioni di progetto predefinite globali
description: Scopri come modificare uno stato personalizzato, impostare le preferenze del progetto globale e creare pianificazioni predefinite globali.
feature: System Setup and Administration
role: Admin
level: Intermediate
activity: deploy
type: Tutorial
team: Technical Marketing
thumbnail: 335065.png
kt: 8753
exl-id: b961ba8c-9597-4ed4-a6d7-79689c8e290d
source-git-commit: adf12d7846d2a1b4c32513a3955c080905044576
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 0%

---

# Configurare le impostazioni di progetto predefinite globali

<!---
21.4 updates have been made
--->

Questo video illustra come:

* Modificare uno stato personalizzato
* Impostare le preferenze globali del progetto
* Creare e utilizzare pianificazioni

>[!VIDEO](https://video.tv.adobe.com/v/335065/?quality=12)

## Impostazioni globali e di gruppo per progetti, attività e problemi

Quando apri la [!UICONTROL Progetti] impostazioni in [!DNL Workfront], noterai che dice &quot;[!UICONTROL Preferenze del progetto di sistema]&quot; nella barra di ricerca nella parte superiore della finestra. Questo consente di sapere che queste impostazioni influiscono su tutti gli utenti [!DNL Workfront] è una configurazione globale.

![[!UICONTROL Preferenze del progetto] in [!UICONTROL Configurazione]](assets/admin-fund-system-project-preferences-1.png)

Vedrai qualcosa di simile all’apertura della [!UICONTROL Attività e problemi] impostazioni.

![[!UICONTROL Preferenze attività e problemi] in [!UICONTROL Configurazione]](assets/admin-fund-task-issue-preferences-2.png)

Tuttavia, è possibile che non tutti i gruppi in [!DNL Workfront] richiede le stesse preferenze per progetti, attività e problemi. Ad esempio, il gruppo di marketing desidera che lo stato di un nuovo progetto sia Planning, mentre il gruppo di project manager preferisce lo stato Request.

[!DNL Workfront] consente agli amministratori dei gruppi di modificare determinati progetti, attività e preferenze di problema per i propri gruppi. Quali preferenze possono essere regolate in base alla [!DNL Workfront] amministratore di sistema che utilizza i pulsanti di blocco/sblocco.

Per iniziare, vai alla pagina [!UICONTROL Configurazione] area:

1. Seleziona **[!UICONTROL Configurazione]** in **[!UICONTROL Menu principale]**.
1. Espandi **[!UICONTROL Preferenze del progetto]** nel menu a sinistra.
1. Seleziona **[!UICONTROL Progetti]** o **[!UICONTROL Attività e problemi]**, a seconda delle impostazioni da modificare.

Blocca una preferenza per impedire agli amministratori di gruppo di regolare tale impostazione per il proprio gruppo.

![Messaggio preferenza bloccato](assets/admin-fund-preferences-locked-3.png)

Sblocca la preferenza per renderla disponibile agli amministratori di gruppo da personalizzare.

![Messaggio di preferenza sbloccato](assets/admin-fund-preferences-unlocked-4.png)

Alcune impostazioni non possono essere sbloccate e rimangono impostazioni di sistema globali.

![Messaggio preferenza bloccato](assets/admin-fund-preferences-always-locked-5.png)

### Impostare le preferenze di gruppo e sottogruppo

Per tutte le impostazioni sbloccate dall’amministratore di sistema, gli amministratori di gruppo possono apportare modifiche ai gruppi che gestiscono e a tutti i sottogruppi nidificati in tali gruppi. Inoltre, gli amministratori dei gruppi possono controllare le impostazioni che possono essere modificate dagli amministratori dei sottogruppi.

1. Seleziona **[!UICONTROL Configurazione]** in **[!UICONTROL Menu principale]**.
1. Fai clic su **[!DNL Groups]** nel menu a sinistra.
1. Fare clic sul nome del gruppo o del sottogruppo per aprirlo.
1. Seleziona **[!UICONTROL Preferenze del progetto]** o **[!UICONTROL Preferenze relative a operazioni e problemi]** nel menu a sinistra.
1. Apporta le modifiche necessarie per ciascuna delle preferenze sbloccate.
1. Seleziona **[!UICONTROL Salva]**.

![[!UICONTROL Stato del progetto] sezione [!UICONTROL Gruppo] page](assets/admin-fund-group-preferences.png)

Se l’organizzazione non utilizza gli amministratori di gruppo, l’amministratore di sistema può gestire le impostazioni delle preferenze per i diversi gruppi.

<!---
learn more URLs and guides
Create or edit a group status 
Group administrators 
Configure system-wide project preferences 
Configure project preferences for a group 
Configure task and issue preferences for a group 
Create and modify a group’s schedule 
--->
