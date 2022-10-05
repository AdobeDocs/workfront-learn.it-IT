---
title: Creare uno stato del problema
description: Scopri come creare uno stato di problema per soddisfare le esigenze dei flussi di lavoro della tua organizzazione.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
kt: 10019
exl-id: 1689080d-1d3c-4fad-a353-64fb3b0d5851
source-git-commit: 1f7a4da813805691fc0e52d3ad1ea708f9e07a9a
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 0%

---

# Creare uno stato di problema

[!DNL Workfront] consiglia di modificare le statue di problemi esistenti nel sistema prima di iniziare a creare nuovi stati. Questo consente di limitare il numero di stati da mantenere.

1. Fai clic su **[!UICONTROL Configurazione]** in **[!UICONTROL Menu principale]**.
1. Espandi la **[!UICONTROL Preferenze del progetto]** nel pannello del menu a sinistra.
1. Seleziona **[!UICONTROL Stati]**.
1. Seleziona la **[!UICONTROL Problemi]** scheda .
1. Assicurati che il campo in alto a destra sia impostato su [!UICONTROL Stati del sistema]. In questo modo, il nuovo stato sarà disponibile a livello globale nell’intera sezione [!DNL Workfront] istanza.
1. Seleziona **[!UICONTROL Elenco principale ]**per visualizzare tutti gli stati dei problemi. In questo punto puoi creare o modificare uno stato.
1. Fai clic su **[!UICONTROL Aggiungi un nuovo stato]**.
1. Compila i campi necessari per la tua organizzazione: nome, descrizione, colore, equazioni con, chiave, ecc.
1. Seleziona le caselle per il tipo di problema con cui questo stato può essere utilizzato.
1. Fai clic su **[!UICONTROL Salva]**.

![Nuova finestra di stato su [!UICONTROL Stati] page](assets/admin-fund-create-issue-status.png)

## Stato dei problemi e amministratori dei gruppi

Gli amministratori dei gruppi possono creare e personalizzare gli stati dei problemi per i gruppi gestiti. Questo offre una certa autonomia al loro gruppo, fornendo loro gli stati di cui hanno bisogno per continuare a lavorare. Elimina inoltre la necessità di un lungo elenco di stati a livello di sistema.

Gli amministratori di gruppo possono modificare gli stati esistenti se sono stati configurati dall’amministratore di sistema per consentire la personalizzazione.

Gli amministratori di sistema possono gestire gli stati dei gruppi selezionando il nome del gruppo nell’angolo in alto a destra del gruppo [!UICONTROL Stati] finestra.

![Menu elenco gruppi in [!UICONTROL Stati] page](assets/admin-fund-change-group-master-list.png)

Gli amministratori dei gruppi possono fare clic su [!UICONTROL Gruppi] nella sezione [!UICONTROL Configurazione] , apri il gruppo facendo clic sul nome e quindi seleziona [!UICONTROL Stati] nel menu del pannello a sinistra. Assicurati di selezionare la scheda Problemi .

![[!UICONTROL Stati] sezione [!UICONTROL Gruppo] page](assets/admin-fund-group-issue-statuses.png)

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
