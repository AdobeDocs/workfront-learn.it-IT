---
title: Ruoli bozza e avvisi e-mail
description: Scopri come abilitare i ruoli di bozza e gli avvisi e-mail appropriati in modo che i destinatari delle bozze possano accedere alle bozze e avere visibilità sul lavoro che viene eseguito in [!DNL  Workfront].
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Beginner
thumbnail: proof-roles-and-email-alerts.png
kt: 10177
exl-id: 15bfb18a-5392-4a91-a6a2-223f7ac30dc5
source-git-commit: 65bd26fefb280d12ec44a4923f6d96ac8d88d6fb
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 0%

---

# Ruoli bozza e avvisi e-mail

I ruoli delle bozze e gli avvisi e-mail aiutano a indirizzare il flusso di lavoro della bozza, garantendo ai destinatari il diritto di accesso alle bozze e la visibilità del lavoro svolto.

Esaminiamo alcuni termini di base relativi alle bozze:

* **Ruolo bozza —** Definisce cosa può fare un utente con una bozza (ad esempio, commento, markup, approvazione, ecc.).
* **Avviso e-mail —** E-mail inviate a persone nel flusso di lavoro della bozza quando è presente un’attività sulla bozza.

![Un&#39;immagine del [!UICONTROL Nuova bozza] finestra con [!UICONTROL Ruolo bozza] e [!UICONTROL Avvisi e-mail] colonne evidenziate.](assets/proof-roles-and-email-alerts.png)

L’amministratore del sistema di bozze può impostare i ruoli di bozza predefiniti e gli avvisi e-mail per gli utenti delle bozze della tua organizzazione. Inoltre, queste informazioni possono essere incorporate nei modelli di flusso di lavoro della bozza (noti anche come modelli di flusso di lavoro automatizzati).

Tuttavia, in alcuni casi può essere necessario impostare queste informazioni manualmente durante il caricamento di una bozza.

[!DNL Workfront] offre le seguenti raccomandazioni generali quando si assegnano ruoli bozza a destinatari bozza:

* **Revisore e approvatore —** Questi utenti possono sia fare commenti sulle bozze che prendere una decisione (ad esempio approvata o rifiutata) su una bozza. Utilizza questo ruolo di bozza per le principali parti interessate interne ed esterne nel processo di revisione.
* **Revisore —** Alcuni utenti nel flusso di lavoro della bozza devono solo aggiungere commenti; questo ruolo è ideale per loro. È inoltre possibile assegnare il ruolo di revisore a [!DNL Workfront] utenti che caricano principalmente bozze o fungono da proprietari della bozza, ma che non fanno parte del processo di bozza.
* **Sola lettura —** Ideale per i destinatari che devono solo visualizzare la bozza. [!UICONTROL Sola lettura] consente l&#39;accesso in visualizzazione e non consente commenti.

[!DNL Workfront] offre le seguenti raccomandazioni generali quando si assegnano avvisi e-mail ai destinatari delle bozze:

* **Decisione finale —** Questo invia un’e-mail quando l’ultima persona prende una decisione sulla bozza. Assegna questa opzione alla persona che monitora il flusso di lavoro della bozza. Può trattarsi di un responsabile bozza, del proprietario della bozza, del creatore della bozza, del project manager o di altro [!DNL Workfront] utente. [!DNL Workfront] consiglia questo avviso quando si utilizza un flusso di lavoro di base, in modo che la persona che monitora la bozza sappia che tutte le decisioni sono state prese.
* **Decisioni —** Questo invia avvisi man mano che ogni parte interessata del flusso di lavoro di verifica prende una decisione sulla bozza. Questa opzione è consigliata quando si utilizza un flusso di lavoro automatizzato, con diverse decisioni. Assegna alla persona che monitora il flusso di lavoro della bozza. Può trattarsi di un responsabile bozza, del proprietario della bozza, del creatore della bozza, del project manager o di altro [!DNL Workfront] utente.
* **Disabilitato —** Utilizzalo per limitare il numero di e-mail che gli utenti guest possono ricevere sulla bozza. I destinatari ricevono comunque notifiche su nuove bozze, nuove versioni e bozze in ritardo, oltre a [!DNL Workfront] gli utenti ricevono messaggi diretti inseriti in un commento della bozza utilizzando @username e i destinatari ospiti con @emailaddress.

## Tocca a te

1. Accedi a Workfront e crea utenti che utilizzeranno gli strumenti di verifica non creati in precedenza. Nelle impostazioni utente, imposta il profilo delle autorizzazioni di bozza in base al ruolo che la persona svolgerà nei flussi di lavoro delle bozze.
1. Se necessario, modifica le impostazioni degli utenti già creati per regolare la selezione del profilo delle autorizzazioni della bozza.
1. Accedere all&#39;area delle impostazioni di correzione e passare alla scheda Utenti. Controlla le impostazioni personali degli utenti: lingua, fuso orario, formato della data, ruolo bozza predefinito e avviso e-mail predefinito. Questo è importante se questi utenti sono stati creati prima che fossero stabiliti i valori predefiniti del sistema globale.

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
