---
title: Creazione di uno stato problema
description: Scopri come creare uno stato del problema per soddisfare le esigenze dei flussi di lavoro della tua organizzazione.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
jira: KT-10019
exl-id: 1689080d-1d3c-4fad-a353-64fb3b0d5851
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 0%

---

# Creare uno stato di problema

[!DNL Workfront] consiglia di modificare gli stati dei problemi esistenti nel sistema prima di iniziare a creare nuovi stati. Questo consente di limitare il numero di stati che devono essere mantenuti.

1. Clic **[!UICONTROL Configurazione]** nel **[!UICONTROL Menu principale]**.
1. Espandi **[!UICONTROL Preferenze progetto]** nel pannello del menu a sinistra.
1. Seleziona **[!UICONTROL Stati]**.
1. Seleziona la **[!UICONTROL Problemi]** scheda.
1. Assicurati che il campo in alto a destra sia impostato su [!UICONTROL Stati del sistema]. In questo modo il nuovo stato sarà disponibile a livello globale in tutte le [!DNL Workfront] dell&#39;istanza.
1. Seleziona **[!UICONTROL Elenco principale]** per visualizzare tutti gli stati dei problemi. In questo punto è possibile creare o modificare uno stato.
1. Clic **[!UICONTROL Aggiungi un nuovo stato]**.
1. Compila i campi necessari per la tua organizzazione: nome, descrizione, colore, equivale a, chiave, ecc.
1. Seleziona le caselle per il tipo di problema con cui questo stato può essere utilizzato.
1. Fai clic su **[!UICONTROL Salva]**.

![Nuova finestra di stato il [!UICONTROL Stati] pagina](assets/admin-fund-create-issue-status.png)

## Stati dei problemi e amministratori dei gruppi

Gli amministratori dei gruppi possono creare e personalizzare gli stati dei problemi per i gruppi che gestiscono. Questo garantisce una certa autonomia al loro gruppo, fornendo loro gli stati necessari per continuare a lavorare. Elimina inoltre la necessità di un lungo elenco di stati a livello di sistema.

Gli amministratori di gruppi possono modificare gli stati esistenti se l’amministratore di sistema li ha configurati per consentire la personalizzazione.

Gli amministratori di sistema possono gestire gli stati dei gruppi selezionando il nome del gruppo nell&#39;angolo superiore destro della [!UICONTROL Stati] finestra.

![Raggruppa menu elenco su [!UICONTROL Stati] pagina](assets/admin-fund-change-group-master-list.png)

Gli amministratori di gruppi possono fare clic su nella [!UICONTROL Gruppi] sezione nella sezione [!UICONTROL Configurazione] aprire il gruppo facendo clic sul nome e quindi selezionando [!UICONTROL Stati] nel menu del pannello sinistro. Assicurarsi di selezionare la scheda Issues (Problemi).

![[!UICONTROL Stati] sezione di [!UICONTROL Gruppo] pagina](assets/admin-fund-group-issue-statuses.png)

<!---
For detailed information on how managing statuses can be done by group administrators, see these articles:
Create and customize group statuses
Group administrators
--->

<!---
learn more URLs
Issue statuses
Create and customize system-wide statuses
--->
