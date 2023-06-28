---
title: Imposta gli Avvisi di Promemoria
description: Scopri come impostare notifiche di promemoria specifiche per oggetto per informare gli utenti della scadenza o dell’imminente scadenza del lavoro.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Beginner
thumbnail: setupremindnote.png
jira: KT-10091
exl-id: f1ba58d7-3226-4c62-8aa4-40f88495b833
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 0%

---

<!---
this has the same content as the system administrator notification setup and mangement section of the email and inapp notificiations learning path
--->

# Configurare le notifiche di promemoria

Le notifiche di promemoria vengono create dagli amministratori di sistema in [!UICONTROL Configurazione] area. Possono quindi essere allegati e utilizzati dai proprietari di progetti, attività e problemi come promemoria per quando il lavoro è in scadenza o in ritardo.

I promemoria sono specifici dell’oggetto e devono essere allegati manualmente all’elemento di lavoro corrispondente in modo che la notifica possa essere inviata.

**Creare una notifica di promemoria**

1. Clic **[!UICONTROL Configurazione]** nel **[!UICONTROL Menu principale]**.
1. Fai clic su **[!UICONTROL E-mail]** sezione.
1. Fai clic su **[!UICONTROL Notifiche]** sezione.
1. Fai clic su **[!UICONTROL Nuovo promemoria]** scheda.
1. Fai clic su **[!UICONTROL +Nuova notifica promemoria]** pulsante.
1. Seleziona l’oggetto desiderato per il menu a discesa.
1. Compila le informazioni richieste.
1. Fai clic su **[!UICONTROL Salva]**.

![[!UICONTROL Nuovo Avviso di Promemoria] finestra](assets/admin-fund-reminder-notification-1.png)

Quando si imposta il promemoria, è necessario considerare alcuni aspetti:

* **[!UICONTROL Nome notifica promemoria] —** Questo è il nome visualizzato dai project manager quando allegano un promemoria a un oggetto. Assicurati che il nome sia sintetico ma descrittivo.
* **[!UICONTROL Periodo idoneo] —** Il numero di ore, giorni, settimane o mesi prima/dopo la data selezionata nella sezione Intervallo.
* **[!UICONTROL Tempistica] —** Seleziona se inviare il promemoria prima o dopo le date di inizio/completamento pianificate, previste o effettive dell&#39;oggetto. Le opzioni per le schede orario sono correlate alla data di inizio, alla data di fine o alla data dell’ultimo aggiornamento.
* **[!UICONTROL Criteri] —** Specifica i criteri per qualificare il promemoria da inviare. Le opzioni variano a seconda del promemoria specifico dell&#39;oggetto.
* **[!UICONTROL Destinatari] —** Selezionare a chi inviare il promemoria. Le opzioni delle parti interessate variano a seconda del tipo di oggetto selezionato per il promemoria.

Una volta stabilite e salvate le impostazioni del promemoria, questa notifica è disponibile per i proprietari di oggetti in [!DNL Workfront].

## Personalizzazione e-mail

Le notifiche di promemoria utilizzano un formato e un messaggio e-mail predefiniti. Se desideri personalizzare l’e-mail, puoi creare un modello.

<!---
paragraph above needs a hyperlink to an article
--->

![Finestra Nuovo modello e-mail](assets/admin-fund-email-customization.png)

<!---
learn more URLs
--->
