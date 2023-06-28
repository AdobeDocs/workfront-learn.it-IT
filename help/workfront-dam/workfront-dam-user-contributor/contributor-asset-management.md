---
title: Scopri come gestire le risorse in [!UICONTROL DAM WORKFRONT]
description: Scopri come gestire le risorse in [!UICONTROL DAM WORKFRONT] per migliorare il workflow.
activity: use
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8996
exl-id: a09d0b0e-2631-414e-87e6-385ddbeb5cd2
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# Collaboratore: gestione risorse

Questo video illustra come:

* Utilizzare il menu Modifica su una risorsa
* Impostare una data di scadenza
* Visualizza notifiche
* Definire le singole impostazioni di notifica
* Caricare una versione della risorsa
* Crea una nuova cartella
* Applicare un modello di metadati a una cartella
* Stabilire le autorizzazioni per la cartella

>[!VIDEO](https://video.tv.adobe.com/v/335256/?quality=12&learn=on)

## Funzionamento delle versioni delle risorse

Una parte del flusso di lavoro può includere la gestione di più versioni (o arrotondamenti, bozze, iterazioni, o qualsiasi altro termine) di una risorsa. Puoi gestire tutte le versioni tramite [!UICONTROL DAM WORKFRONT].

Il sistema consente il controllo automatico della versione delle risorse quando un file con lo stesso nome di un file esistente viene caricato nella stessa cartella. Rivolgiti all’amministratore di sistema per verificare se questa funzionalità è stata attivata.

Se è attivato il controllo automatico della versione, la versione di una risorsa viene eseguita solo se viene caricata nella cartella che contiene la risorsa originale. Entrambe le risorse devono avere lo stesso nome file. Se la risorsa viene caricata in un’altra cartella, viene inserita come nuovo file.
Se il controllo della versione non è attivato, un file con lo stesso nome di un file esistente viene caricato come nuovo file, indipendentemente dalla cartella in cui è inserito. Questo poteva comportare la presenza di due risorse con lo stesso nome nella stessa cartella.

Puoi anche caricare manualmente le versioni di una risorsa specifica. Fai clic sull’icona di modifica della risorsa, quindi seleziona **[!UICONTROL Carica nuova versione]**.

Se pubblichi una risorsa con le versioni di Brand Connect, l’utente di Brand Connect visualizza solo la versione più recente della risorsa.

## Stato e scadenza della cartella e della risorsa

Gli stati sono un altro modo per gestire l’accesso a cartelle e risorse in [!UICONTROL DAM WORKFRONT]. Gli stati possono essere utilizzati per nascondere determinate risorse o cartelle da [!UICONTROL Brand Connect] utenti o di far scadere una risorsa o una cartella in modo che solo l’amministratore di sistema possa accedervi.

* **[!UICONTROL Attivo]**- Utilizzato per risorse e cartelle. Risorse e cartelle con [!UICONTROL Attivo] sono visibili a tutti gli utenti con autorizzazioni e possono essere pubblicati in [!UICONTROL Brand Connect]. [!UICONTROL Attivo] è indicato da un punto verde su una risorsa o cartella.
* **[!UICONTROL Inattivo]**- Utilizzato per risorse e cartelle. Risorse e cartelle con [!UICONTROL Inattivo] lo stato è visibile a [!UICONTROL DAM WORKFRONT] utenti ma non sono visibili nel [!UICONTROL Brand Connect]. [!UICONTROL Inattivo] è indicato da un punto rosso su una risorsa o cartella.
* **[!UICONTROL Non scaduto]**- Utilizzato solo per le risorse. Questo è lo stato predefinito di tutte le risorse. Risorse non scadute che sono anche [!UICONTROL Attivo] sono visibili in [!UICONTROL Brand Connect].
* **[!UICONTROL Scaduto]**- Utilizzato solo per le risorse. Risorse con [!UICONTROL Scaduto] lo stato non può essere scaricato da alcun utente ad eccezione dell&#39;amministratore di sistema. Le risorse scadute sono visibili o non visibili nel [!UICONTROL Brand Connect], a seconda delle configurazioni del sistema.
