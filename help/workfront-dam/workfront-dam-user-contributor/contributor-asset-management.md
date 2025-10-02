---
title: Comprendere la gestione risorse come collaboratore
description: Scopri come gestire le risorse in [!UICONTROL Workfront DAM] per migliorare il flusso di lavoro.
activity: use
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8996
exl-id: a09d0b0e-2631-414e-87e6-385ddbeb5cd2
doc-type: video
source-git-commit: bbdf99c6bc1be714077fd94fc3f8325394de36b3
workflow-type: tm+mt
source-wordcount: '460'
ht-degree: 100%

---

# Comprendere la gestione risorse come collaboratore

In questo video scoprirai come:

* Utilizzare il menu Modifica per una risorsa
* Impostare una data di scadenza
* Visualizzare le notifiche
* Definire le impostazioni di notifica per singoli elementi
* Caricare una versione di una risorsa
* Creare una nuova cartella
* Applicare un modello di metadati a una cartella
* Stabilire le autorizzazioni per una cartella

>[!VIDEO](https://video.tv.adobe.com/v/335256/?quality=12&learn=on&enablevpops=1)

## Funzionamento delle versioni delle risorse

Un flusso di lavoro può includere la gestione di più versioni (o passate, bozze, iterazioni, o qualsiasi altro termine) di una risorsa. Puoi gestire tutte le versioni tramite [!UICONTROL Workfront DAM].

Il sistema consente il controllo automatico delle versioni delle risorse quando un file con lo stesso nome di un file esistente viene caricato nella stessa cartella. Per verificare se questa funzionalità è stata attivata, rivolgiti all’amministratore di sistema.

Se è stato attivato il controllo automatico delle versioni, la versione di una risorsa viene eseguita solo se viene caricata nella cartella che contiene la risorsa originale. Entrambe le risorse devono avere lo stesso nome file. Se la risorsa viene caricata in un’altra cartella, viene inserita come nuovo file.
Se il controllo della versione non è stato attivato, un file con lo stesso nome di un file esistente viene caricato come nuovo file, indipendentemente dalla cartella in cui è inserito. Questo può comportare la presenza di due risorse con lo stesso nome nella stessa cartella.

Puoi anche caricare manualmente le versioni di una risorsa specifica. Fai clic sull’icona di modifica della risorsa, quindi seleziona **[!UICONTROL Carica nuova versione]**.

Se pubblichi in Brand Connect una risorsa con più versioni, l’utente di Brand Connect vede solo la versione più recente della risorsa.

## Stato e scadenza delle cartelle e delle risorse

Gli stati sono un altro modo per gestire l’accesso a cartelle e risorse in [!UICONTROL Workfront DAM]. Gli stati possono essere utilizzati per nascondere determinate risorse o cartelle agli utenti di [!UICONTROL Brand Connect] oppure per far scadere una risorsa o una cartella in modo che solo l’amministratore di sistema possa accedervi.

* **[!UICONTROL Attivo:]** utilizzato per risorse e cartelle. Le risorse e le cartelle con stato [!UICONTROL Attivo] sono visibili a tutti gli utenti con autorizzazioni e possono essere pubblicate in [!UICONTROL Brand Connect]. [!UICONTROL Attivo] è indicato da un punto verde su una risorsa o cartella.
* **[!UICONTROL Inattivo:]** utilizzato per risorse e cartelle. Le risorse e le cartelle con stato [!UICONTROL Inattivo] sono visibili agli utenti [!UICONTROL Workfront DAM] ma non sono visibili in [!UICONTROL Brand Connect]. [!UICONTROL Inattivo] è indicato da un punto rosso su una risorsa o cartella.
* **[!UICONTROL Non scaduto:]** utilizzato solo per le risorse. Questo è lo stato predefinito di tutte le risorse. Le risorse non scadute che sono anche in stato [!UICONTROL Attivo] sono visibili in [!UICONTROL Brand Connect].
* **[!UICONTROL Scaduto:]** utilizzato solo per le risorse. Le risorse con stato [!UICONTROL Scaduto] non possono essere scaricate da alcun utente, ad eccezione dell’amministratore di sistema. Le risorse scadute sono visibili o non visibili in [!UICONTROL Brand Connect], a seconda delle configurazioni del sistema.
