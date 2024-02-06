---
title: Ruoli bozza e avvisi e-mail
description: Scopri come abilitare i ruoli bozza e gli avvisi e-mail appropriati in modo che i destinatari della bozza possano accedervi e avere visibilità sul lavoro che viene eseguito in  [!DNL  Workfront].
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Beginner
thumbnail: proof-roles-and-email-alerts.png
jira: KT-10177
exl-id: 15bfb18a-5392-4a91-a6a2-223f7ac30dc5
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: ht
source-wordcount: '551'
ht-degree: 100%

---

# Ruoli bozza e avvisi e-mail

I ruoli bozza e gli avvisi e-mail aiutano a indirizzare il flusso di lavoro di bozza, garantendo ai destinatari il diritto di accesso alle bozze e la visibilità del lavoro svolto.

Esaminiamo alcuni termini di base relativi alle bozze:

* **Ruolo bozza:** definisce le operazioni che un utente può eseguire con una bozza (ad esempio, commentare, aggiungere markup, approvare, ecc.).
* **Avviso e-mail:** e-mail inviate a persone nel flusso di lavoro di bozza quando è presente un’attività sulla bozza.

![Un’immagine della finestra [!UICONTROL Nuova bozza] con [!UICONTROL Ruolo bozza] e le colonne [!UICONTROL Avvisi e-mail] evidenziate.](assets/proof-roles-and-email-alerts.png)

L’amministratore del sistema di bozza può impostare i ruoli di bozza predefiniti e gli avvisi e-mail per gli utenti delle bozze della tua organizzazione. Inoltre, queste informazioni possono essere incorporate nei modelli di flusso di lavoro di bozza (noti anche come modelli di flusso di lavoro automatizzati).

Tuttavia, in alcuni casi può essere necessario impostare queste informazioni manualmente durante il caricamento di una bozza.

[!DNL Workfront] offre i seguenti consigli generali quando si assegnano ruoli bozza ai destinatari della bozza:

* **Revisore e approvatore:** questi utenti possono sia creare commenti sulle bozze sia prendere una decisione (come approvare o rifiutare) riguardo una bozza. Utilizza questo ruolo bozza per gli stakeholder interni ed esterni al processo di revisione.
* **Revisore:** ruolo ideale per quelle persone che nel flusso di lavoro di bozza devono solo creare commenti. È inoltre possibile assegnare il ruolo di revisore a utenti di [!DNL Workfront] che caricano principalmente bozze o fungono da proprietari di bozza, ma che non fanno parte del processo di bozza.
* **Sola lettura:** ideale per i destinatari che necessitano solo di visualizzare la bozza. [!UICONTROL Sola lettura] consente l’accesso tramite visualizzazione e non consente di creare commenti.

[!DNL Workfront] offre i seguenti consigli generali quando si assegnano avvisi e-mail ai destinatari della bozza:

* **Decisione finale:** viene inviata un’e-mail quando l’ultima persona prende una decisione sulla bozza. Assegna questo ruolo alla persona che monitora il flusso di lavoro di bozza. Potrebbe trattarsi di un manager della bozza, del proprietario della bozza, del creatore della bozza, del project manager o altro utente di [!DNL Workfront]. [!DNL Workfront] consiglia questo avviso quando si utilizza un flusso di lavoro di base, in modo che la persona che monitora la bozza sappia che tutte le decisioni sono state prese.
* **Decisioni:** invia avvisi mentre ogni stakeholder del flusso di lavoro di bozza prende una decisione sulla bozza. Questa opzione è la migliore quando si utilizza un flusso di lavoro automatizzato, con diverse decisioni. Assegnare alla persona che monitora il flusso di lavoro di bozza. Può trattarsi di un manager della bozza, di un proprietario della bozza, di un creatore della bozza, del project manager o altro utente di [!DNL Workfront].
* **Disabilitato:** da utilizzare per gli utenti guest della bozza per limitare il numero di e-mail che ricevono sulla bozza. I destinatari ricevono comunque informazioni su nuove bozze, nuove versioni e bozze in ritardo; inoltre gli utenti di [!DNL Workfront] ricevono messaggi diretti inseriti in un commento della bozza utilizzando @username e i destinatari guest con @emailaddress.

## Tocca a te

1. Accedi a Workfront e crea utenti che utilizzeranno la bozza che non hai creato in precedenza. Nelle impostazioni utente, imposta il profilo delle autorizzazioni di bozza in base al ruolo che la persona svolgerà nei flussi di lavoro di bozza.
1. Se necessario, modifica le impostazioni degli utenti già creati per regolare la selezione del profilo delle autorizzazioni di bozza.
1. Accedi all’area delle impostazioni di bozza e passa alla scheda Utenti. Verifica le impostazioni personali per i tuoi utenti: lingua, fuso orario, formato data, ruolo di bozza predefinito e avviso e-mail predefinito. Questo è importante se gli utenti sono stati creati prima che fossero stabiliti i valori predefiniti del sistema globale.

<!--
Download the proof role and email alert guides to have on hand as you start uploading proofs and assigning proof recipients.
-->

<!--
## Learn more
* Notifications for proof comments and decisions
-->

<!--
## Guides
* Proof roles
* Email alerts
-->
