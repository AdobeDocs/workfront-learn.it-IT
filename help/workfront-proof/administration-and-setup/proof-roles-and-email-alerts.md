---
title: Ruoli di prova e avvisi e-mail
description: Scopri come abilitare ruoli di bozza e avvisi e-mail appropriati in modo che i destinatari delle prove abbiano accesso alle bozze e alla visibilità del lavoro in corso [!DNL  Workfront].
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Beginner
thumbnail: proof-roles-and-email-alerts.png
kt: 10177
exl-id: 15bfb18a-5392-4a91-a6a2-223f7ac30dc5
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '562'
ht-degree: 0%

---

# Ruoli di prova e avvisi e-mail

I ruoli di prova e gli avvisi e-mail consentono di gestire il flusso di lavoro della bozza, garantendo ai destinatari il diritto di accesso alle bozze e la visibilità del lavoro in corso.

Rivediamo alcuni termini di prova di base:

* **Ruolo di prova —** Definisce le operazioni che un utente può eseguire con una bozza (ad esempio, commento, markup, approvazione, ecc.).
* **Avviso e-mail —** Invia e-mail alle persone nel flusso di lavoro della bozza quando c’è attività sulla bozza.

![Un&#39;immagine del [!UICONTROL Nuova bozza] finestra con [!UICONTROL Ruolo di prova] e [!UICONTROL Avvisi e-mail] colonne evidenziate.](assets/proof-roles-and-email-alerts.png)

L’amministratore di sistema della bozza può impostare ruoli di bozza predefiniti e avvisi e-mail per gli utenti della bozza dell’organizzazione. Inoltre, queste informazioni possono essere incorporate in modelli di flusso di lavoro di prova (noti anche come modelli di flusso di lavoro automatizzati).

Tuttavia, in alcuni casi può essere necessario impostare manualmente queste informazioni durante il caricamento di una bozza.

[!DNL Workfront] offre le seguenti raccomandazioni generali quando si assegnano ruoli di bozza ai destinatari della bozza:

* **Revisore e approvatore —** Questi utenti possono formulare osservazioni sulle bozze e prendere una decisione (come quella approvata o rifiutata) su una prova. Utilizza questo ruolo di prova per le principali parti interessate interne ed esterne nel processo di revisione.
* **Revisore —** Alcuni utenti del flusso di lavoro di prova devono solo fare commenti, questo ruolo è ideale per loro. Il ruolo di revisore può essere assegnato anche a [!DNL Workfront] gli utenti che caricano principalmente le bozze o fungono da proprietario della bozza ma che altrimenti non fanno parte del processo di correzione.
* **Sola lettura —** Ideale per i destinatari che devono solo vedere la bozza. [!UICONTROL Sola lettura] consente l’accesso alla visualizzazione e non consente l’inserimento di commenti.

[!DNL Workfront] offre le seguenti raccomandazioni generali quando si assegnano avvisi e-mail ai destinatari della bozza:

* **Decisione finale —** Questo invia un’e-mail quando l’ultima persona prende una decisione sulla bozza. Assegna questa proprietà alla persona che monitora il flusso di lavoro della bozza. Può trattarsi di un responsabile della bozza, di un proprietario della bozza, di un creatore della bozza, di un project manager o di un altro [!DNL Workfront] utente. [!DNL Workfront] consiglia questo avviso quando si utilizza un flusso di lavoro di base, in modo che l’utente che esegue il monitoraggio della bozza sappia che sono state prese tutte le decisioni necessarie.
* **Decisioni —** Questo invia gli avvisi mentre ogni stakeholder del flusso di lavoro di correzione prende una decisione sulla bozza. Questa opzione è ideale quando si utilizza un flusso di lavoro automatizzato, con diverse decisioni. Assegna alla persona che monitora il flusso di lavoro della bozza. Può trattarsi di un responsabile della bozza, di un proprietario della bozza, di un creatore della bozza, di un project manager o di un altro [!DNL Workfront] utente.
* **Disattivato —** Utilizza questa opzione per gli utenti a prova di ospite per limitare il numero di e-mail ricevute sulla bozza. I destinatari ricevono ancora le notifiche relative a nuove bozze, nuove versioni e prove in ritardo, più [!DNL Workfront] gli utenti ricevono messaggi diretti inseriti in un commento di bozza utilizzando @username e destinatari guest con @emailaddress.

## Il tuo turno

1. Accedi a Workfront e crea utenti che utilizzeranno le bozze che non hai creato in precedenza. Imposta il profilo delle autorizzazioni di bozza nelle impostazioni utente in base al ruolo che la persona svolgerà nei flussi di lavoro di prova.
1. Per gli utenti che sono già stati creati, modifica le loro impostazioni per regolare la selezione dei profili di autorizzazioni di prova e , se necessario.
1. Accedi all’area delle impostazioni di correzione e passa alla scheda Utenti . Controlla le impostazioni personali dei tuoi utenti: lingua, fuso orario, formato data, ruolo di bozza predefinito e avviso e-mail predefinito. Ciò è importante se questi utenti sono stati creati prima che siano state stabilite le impostazioni predefinite del sistema globale (queste impostazioni sono descritte nella sezione 1 di questo percorso di apprendimento).

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
