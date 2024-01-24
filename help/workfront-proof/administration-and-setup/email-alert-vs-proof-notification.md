---
title: Comprendere gli avvisi e-mail e le notifiche delle bozze
description: Comprendere la differenza tra gli avvisi e-mail e le notifiche delle bozze in [!DNL  Workfront].
feature: Workfront Proof
type: Tutorial
role: User
level: Beginner
thumbnail: email-alert-vs-proof-notifications.png
jira: KT-10174
last-substantial-update: 2024-01-24T00:00:00Z
exl-id: 51423110-960c-46ed-8b4e-6e73c67c42e0
source-git-commit: 30748311c14fb8aa6b10c03a74e83f46bdb5dfbf
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 0%

---

# Comprendere gli avvisi e-mail e le notifiche delle bozze

Gli avvisi e-mail sono diversi dalle e-mail di notifica delle bozze. Riceverai un’e-mail di notifica della bozza quando ti viene assegnata una nuova bozza da rivedere, quando una bozza è in ritardo o quando è presente una nuova versione della bozza da esaminare.

![Immagine di un’e-mail di notifica della bozza che indica che è presente una nuova bozza da rivedere.](assets/email-alert-1.png)

Se disattivi l’opzione di notifica durante il caricamento di una bozza, nessuno riceve alcuna comunicazione da [!DNL Workfront] sull’esistenza di una nuova bozza da rivedere.

Gli avvisi e-mail vengono impostati per revisore/approvatore, il più delle volte quando viene caricata la bozza. È possibile che ai destinatari della bozza venga assegnato un tipo di avviso e-mail predefinito, in modo da non doverlo impostare ogni volta che si carica una bozza. Rivolgersi all&#39;amministratore di sistema per l&#39;impostazione di queste impostazioni predefinite.

![Immagine di un avviso e-mail che indica che è stata presa una decisione sulla bozza ed è presente un commento da rivedere.](assets/email-alert-2.png)

Anche se gli avvisi e-mail sono impostati su [!UICONTROL Disabilitato], ai destinatari della bozza viene comunque notificata una nuova bozza o versione.

## Best practice

| Best practice | Ecco perché |
|---|---|
| Nelle impostazioni di Workfront, disabilita l’impostazione &quot;Send emails from Workfront when a comment is made on a proof&quot; (Invia e-mail da quando viene inserito un commento su una bozza) | Quando questa impostazione è abilitata (che è per impostazione predefinita), gli utenti possono ricevere più notifiche e-mail per ogni commento su una bozza, una dalla funzionalità di correzione e una da Workfront stessa. Tali notifiche duplicate causano confusione e interruzioni delle notifiche e-mail, nonché una casella in entrata e-mail completa, che può in ultima analisi causare l’ignoramento delle notifiche delle bozze ricevute dagli utenti. Il che, a sua volta, potrebbe significare scadenze non rispettate. <br> <br>Nota: questa impostazione si trova nel menu principale di Workfront > Configurazione > E-mail > Revisione e approvazione. |


