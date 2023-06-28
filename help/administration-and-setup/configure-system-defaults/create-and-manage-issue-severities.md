---
title: Creare e gestire le gravità dei problemi
description: Scopri come impostare e gestire la gravità dei problemi.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
jira: KT-10020
exl-id: a5a9280b-0d48-413d-92de-f6a949e6b210
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '368'
ht-degree: 3%

---

# Creare e gestire le gravità dei problemi

## Introduzione alle gravità dei problemi

Una gravità può essere utilizzata per indicare la gravità di un problema o come potrebbe influire sul lavoro svolto.

![[!UICONTROL Gravità] menu in [!UICONTROL Dettagli problema] finestra](assets/admin-fund-severity-issue-details.png)

Il [!UICONTROL Gravità] è accessibile nel [!UICONTROL Dettagli problema]. Può essere incluso anche nelle viste a colonne negli elenchi e nei rapporti personalizzati.

[!DNL Workfront] ha cinque gravità predefinite:

* [!UICONTROL Cosmetico]
* [!UICONTROL Causa Confusione]
* [!UICONTROL Bug con workaround]
* [!UICONTROL Bug senza workaround]
* [!UICONTROL Errore Fatale]

Se necessario, gli amministratori di sistema possono rinominare le gravità predefinite o crearne di nuove.

Le gravità sono disponibili solo per i problemi in [!DNL Workfront].

## Creare e gestire le gravità dei problemi

In qualità di amministratore di sistema, puoi creare nuove gravità, se necessario, per completare il flusso di lavoro del problema.

![[!UICONTROL Gravità] pagina in [!UICONTROL Configurazione]](assets/admin-fund-severity-section.png)

1. Clic **[!UICONTROL Configurazione]** nel **[!UICONTROL Menu principale]**.
1. Espandi **[!UICONTROL Preferenze progetto]** nel pannello del menu a sinistra.
1. Seleziona **[!UICONTROL Gravità]**.
1. Clic **[!UICONTROL Aggiungi nuova gravità]**.
1. Assegnare alla gravità un nome corrispondente all&#39;uso previsto.
1. Il **[!UICONTROL Importanza]** number corrisponde alla gravità del problema. Il numero più alto corrisponde alla gravità più elevata. Il [!UICONTROL Importanza] il numero deve essere univoco.
1. Seleziona un colore per la tua priorità. Viene utilizzato nei rapporti grafico e in altre posizioni in [!DNL Workfront].
1. Designare una delle opzioni di gravità come **[!UICONTROL Gravità predefinita]**. Questo viene applicato automaticamente a tutti i nuovi problemi in Workfront.
1. Includere una descrizione della gravità, ad esempio la modalità di utilizzo.
1. Fai clic all’esterno dei campi da salvare.

![[!UICONTROL Gravità] list](assets/admin-fund-severity-new.png)

### Modifica delle gravità

Se una gravità non diventa più rilevante per i flussi di lavoro relativi ai problemi, può essere rinominata, nascosta o eliminata.

Se una gravità non è più necessaria, [!DNL Workfront] consiglia di nascondere la gravità (fare clic sul pulsante [!UICONTROL Nascondi] nell&#39;area di configurazione). In questo modo l’opzione gravità viene rimossa dal menu a discesa del problema, ma viene mantenuta nei dati storici in modo che sia ancora disponibile a scopo di reporting.

![[!UICONTROL Nascondi] colonna evidenziata su [!UICONTROL Gravità] pagina in [!UICONTROL Configurazione]](assets/admin-fund-severity-hide.png)

[!DNL Workfront] consiglia di **non** elimina una gravità utilizzata per i problemi passati. Quando si elimina una gravità, viene richiesto di sostituirne un&#39;altra. Questo può modificare i dati storici e influire sul reporting.

![Finestra Elimina gravità](assets/admin-fund-severity-delete.png)

<!---
learn more URLs
Create and customize issue severities
Update issue severity
--->
