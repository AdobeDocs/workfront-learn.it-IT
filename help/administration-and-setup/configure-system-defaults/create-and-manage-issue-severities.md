---
title: Creare e gestire la gravità dei problemi
description: Scopri come impostare e gestire la gravità dei problemi.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
jira: KT-10020
exl-id: a5a9280b-0d48-413d-92de-f6a949e6b210
source-git-commit: 4568e4e47b719e2dee35357d42674613112a9c43
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Creare e gestire la gravità dei problemi

## Introduzione alle gravità dei problemi

Il livello di gravità può essere utilizzato per indicare la criticità di un problema o come potrebbe influire sullo svolgimento del lavoro.

Menu ![[!UICONTROL Gravità] nella finestra [!UICONTROL Dettagli problema]](assets/admin-fund-severity-issue-details.png)

Si può accedere al campo [!UICONTROL Gravità] in [!UICONTROL Dettagli problema]. Il campo può essere incluso anche nelle visualizzazioni a colonne negli elenchi e nei rapporti personalizzati.

[!DNL Workfront] ha cinque livelli di gravità predefiniti:

* [!UICONTROL Cosmetico]
* [!UICONTROL Causa Confusione]
* [!UICONTROL Bug con workaround]
* [!UICONTROL Bug senza workaround]
* [!UICONTROL Errore Fatale]

Se necessario, gli amministratori di sistema possono rinominare le gravità predefinite o crearne di nuove.

Le gravità sono disponibili solo per i problemi in [!DNL Workfront].

## Creare e gestire la gravità dei problemi

In qualità di amministratore di sistema, puoi creare nuove gravità, se necessario, per completare il flusso di lavoro del problema.

Pagina ![[!UICONTROL Gravità] in [!UICONTROL Configurazione]](assets/admin-fund-severity-section.png)

1. Fai clic **[!UICONTROL Configurazione]** nel **[!UICONTROL Menu principale]**.
1. Espandi la sezione **[!UICONTROL Preferenze progetto]** nel pannello del menu a sinistra.
1. Seleziona **[!UICONTROL Gravità]**.
1. Fai clic su **[!UICONTROL Aggiungi nuova gravità]**.
1. Assegna alla gravità un nome corrispondente all’uso previsto.
1. l numero di **[!UICONTROL Importanza]** indica la criticità del problema. Il numero più alto corrisponde alla gravità più alta. Il numero di [!UICONTROL Importanza] deve essere univoco.
1. Seleziona un colore per la priorità. Il colore viene utilizzato nei rapporti grafici e in altre posizioni in [!DNL Workfront].
1. Designa una delle opzioni di gravità come **[!UICONTROL Gravità predefinita]**. Questo valore verrà applicato automaticamente a tutti i nuovi problemi in Workfront.
1. Includi una descrizione della gravità, ad esempio la modalità di utilizzo.
1. Fai clic all’esterno dei campi da salvare.

Elenco ![[!UICONTROL Gravità]](assets/admin-fund-severity-new.png)

### Modifica delle gravità

Se una gravità non diventa più rilevante per i flussi di lavoro relativi ai problemi, può essere rinominata, nascosta o eliminata.

Se una gravità non è più necessaria, [!DNL Workfront] consiglia di nasconderla (facendo clic sulla casella [!UICONTROL Nascondi] accanto ad essa nell’area di configurazione). In questo modo l’opzione gravità viene rimossa dal menu a discesa del problema, ma viene mantenuta nei dati storici in modo che sia ancora disponibile a scopo di reporting.

Colonna ![[!UICONTROL Nascondi] evidenziata sulla pagina [!UICONTROL Gravità] in [!UICONTROL Configurazione]](assets/admin-fund-severity-hide.png)

[!DNL Workfront] consiglia di **non** eliminare una gravità che è stata utilizzata in problemi precedenti. Quando elimini una gravità, ti viene chiesto di sostituirla con un’altra. Questo potrebbe modificare i dati storici e influire sul reporting.

![Finestra Elimina gravità](assets/admin-fund-severity-delete.png)

<!--
learn more URLs
Create and customize issue severities
Update issue severity
-->
