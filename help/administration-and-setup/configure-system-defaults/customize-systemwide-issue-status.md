---
title: Personalizzare gli stati dei problemi a livello di sistema
description: Scopri come modificare i nomi degli stati dei problemi, controllare i tipi di problemi per i quali viene utilizzato uno stato e bloccare/sbloccare gli stati per la personalizzazione a livello di gruppo.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
jira: KT-10030
exl-id: c8f5677f-8d9d-4d1a-a1e3-d1a438878213
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 0%

---

# Personalizzare gli stati a livello di sistema

[!DNL Workfront] fornisce una serie di stati predefiniti per adattarsi ai flussi di lavoro di gestione dei problemi della tua organizzazione. Questi stati possono essere rinominati in base alla terminologia della tua organizzazione. Gli stati AND possono essere assegnati a tipi di problemi specifici.

Se necessario, è possibile creare stati aggiuntivi. Solo gli amministratori di sistema possono creare stati a livello di sistema. Inoltre, gli amministratori di sistema controllano quali stati possono essere modificati dagli amministratori di gruppi.

![[!UICONTROL Problemi] scheda su [!UICONTROL Statue] pagina in [!UICONTROL Configurazione]](assets/admin-fund-all-issue-statuses.png)

## Modificare gli stati esistenti

[!DNL Workfront] consiglia un numero minimo di stati. In questo modo la scelta dello stato corretto è più semplice per gli utenti e si ottiene un elenco più breve di stati da mantenere.

È possibile modificare uno stato esistente per cambiare il nome, i tipi di problema a cui è assegnato, il colore correlato e così via.

![Elenco stato problema con [!UICONTROL Modifica] opzione evidenziata](assets/admin-fund-edit-issue-status.png)

1. Clic **[!UICONTROL Configurazione]** nel **[!UICONTROL Menu principale]**.
1. Espandi **[!UICONTROL Preferenze progetto]** nel pannello del menu a sinistra.
1. Seleziona **[!UICONTROL Stati]**.
1. Seleziona la **[!UICONTROL Problemi]** e assicurati che [!UICONTROL Stati del sistema] viene visualizzato nell&#39;angolo superiore destro.
1. Seleziona **[!UICONTROL Elenco principale]** per visualizzare gli stati di tutti i tipi di problemi. In questa fase è possibile creare o modificare lo stato di un problema.
1. Passa il puntatore del mouse sul lato destro dello stato che desideri rinominare e fai clic su **[!UICONTROL Modifica]**.
1. Assegna un nuovo nome allo stato o modifica eventuali altre informazioni, a seconda delle esigenze.
1. Se queste impostazioni devono essere applicate a tutti gli utenti nel tuo [!DNL Workfront] dell&#39;istanza.
1. Sblocca lo stato per consentire agli amministratori di gruppi di modificare lo stato solo per i loro gruppi.
1. Seleziona le caselle per il tipo di problema a cui si applica lo stato.
1. Fai clic su **[!UICONTROL Salva]**.

![Finestra per creare un nuovo stato](assets/admin-fund-edit-issue-status-2.png)

### Assegnazioni di stato

È possibile che non tutti gli stati vengano assegnati a tutti i tipi di problemi. Il [!UICONTROL Stati] La pagina include colonne che mostrano per quale tipo di problema è possibile utilizzare ogni stato.

![Ordine di modifica evidenziato nella scheda Problemi della pagina Stati](assets/admin-fund-issue-type-statuses.png)


Per visualizzare solo gli stati assegnati a un tipo di problema specifico, fai clic sul nome del tipo di problema nella parte superiore della finestra.

![[!UICONTROL Problema] scheda di [!UICONTROL Stato] pagina con colonne evidenziate](assets/admin-fund-statuses-issue-type.png)

Da qui, puoi trascinare e rilasciare i problemi nell’ordine in cui desideri che vengano visualizzati nel [!UICONTROL Stato] menu a discesa.

Per modificare gli stati, devi tornare al [!UICONTROL Elenco principale].
