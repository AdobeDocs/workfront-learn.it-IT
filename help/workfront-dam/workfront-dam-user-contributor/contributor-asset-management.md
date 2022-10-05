---
title: Come gestire le risorse in [!UICONTROL Workfront DAM]
description: Scopri come gestire le risorse in [!UICONTROL Workfront DAM] per migliorare il flusso di lavoro.
activity: use
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
kt: 8996
exl-id: a09d0b0e-2631-414e-87e6-385ddbeb5cd2
source-git-commit: d1f5c4a558f737cb8188e209a16b91b67d32285c
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 0%

---

# Collaboratore: gestione risorse

Questo video illustra come:

* Utilizzare il menu Modifica di una risorsa
* Imposta una data di scadenza
* Visualizza notifiche
* Stabilire impostazioni di notifica individuali
* Caricare una versione di una risorsa
* Crea una nuova cartella
* Applicare un modello di metadati a una cartella
* Stabilire le autorizzazioni della cartella

>[!VIDEO](https://video.tv.adobe.com/v/335256/?quality=12)

## Funzionamento delle versioni delle risorse

Parte del flusso di lavoro può includere la gestione di più versioni di una risorsa, o arrotondamenti, bozze, iterazioni, come le chiamate. Puoi gestire tutte le versioni attraverso [!UICONTROL Workfront DAM].

Il sistema consente il controllo automatico della versione delle risorse quando un file con lo stesso nome di un file esistente viene caricato nella stessa cartella. Verifica con l’amministratore di sistema se questa funzionalità è stata attivata.

Se il controllo automatico della versione è attivato, la versione di una risorsa verrà eseguita solo se è caricata nella cartella che contiene la risorsa originale. Entrambe le risorse devono avere lo stesso nome file. Se la risorsa viene caricata in un’altra cartella, la risorsa viene inserita come nuovo file.
Se il controllo della versione non è attivato, un file con lo stesso nome di un file esistente viene caricato come nuovo file, indipendentemente dalla cartella in cui è stato inserito. Questo potrebbe comportare l’inserimento nella stessa cartella di due risorse con lo stesso nome.

Puoi anche caricare manualmente le versioni di una risorsa specifica. Fai clic sull’icona di modifica della risorsa, quindi seleziona **[!UICONTROL Carica nuova versione]**.

Se pubblichi una risorsa con versioni su Brand Connect, l’utente di Brand Connect visualizza solo la versione più recente della risorsa.

## Stato e scadenza della cartella e della risorsa

Gli stati sono un altro modo per gestire l’accesso a cartelle e risorse in [!UICONTROL Workfront DAM]. Gli stati possono essere utilizzati per nascondere determinate risorse o cartelle da [!UICONTROL Brand Connect] gli utenti o la scadenza di una risorsa o di una cartella in modo che nessun altro amministratore di sistema possa accedervi.

* **[!UICONTROL Attivo]**- Utilizzato per risorse e cartelle. Risorse e cartelle con [!UICONTROL Attivo] lo stato è visibile a tutti gli utenti con autorizzazioni e può essere pubblicato in [!UICONTROL Brand Connect]. [!UICONTROL Attivo] è indicato con un punto verde su una risorsa o una cartella.
* **[!UICONTROL Inattivo]**- Utilizzato per risorse e cartelle. Risorse e cartelle con [!UICONTROL Inattivo] lo stato è visibile per [!UICONTROL Workfront DAM] ma non sono visibili nel [!UICONTROL Brand Connect]. [!UICONTROL Inattivo] è indicato con un punto rosso su una risorsa o una cartella.
* **[!UICONTROL Imprevedibile]**- Utilizzato solo per le risorse. Questo è lo stato predefinito di tutte le risorse. Risorse impreviste che sono anche [!UICONTROL Attivo] sono visibili nella [!UICONTROL Brand Connect].
* **[!UICONTROL Scaduto]**- Utilizzato solo per le risorse. Risorse con [!UICONTROL Scaduto] lo stato non può essere scaricato da alcun utente, ad eccezione dell&#39;amministratore di sistema. Le risorse scadute sono visibili o non sono visibili nel [!UICONTROL Brand Connect], a seconda delle configurazioni di sistema.
