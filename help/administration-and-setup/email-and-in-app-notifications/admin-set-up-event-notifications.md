---
title: Impostare le notifiche degli eventi
description: Scopri come controllare le notifiche e-mail e in-app ricevute dagli utenti gestendo le notifiche degli eventi.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate
thumbnail: 10093.jpeg
kt: 10093
exl-id: 6bd3a777-0ed8-4383-ad8e-f1238e334e78
source-git-commit: 1f7a4da813805691fc0e52d3ad1ea708f9e07a9a
workflow-type: tm+mt
source-wordcount: '621'
ht-degree: 4%

---

<!---
this has the same content as the system administrator notification setup and mangement section of the email and inapp notificiations learning path
--->

<!---
add URL link in the note at the top of the LP
--->

# Impostare le notifiche degli eventi

>[!NOTE]
>
>A causa di un rollout graduale, la funzionalità che consente agli amministratori di sistema e di gruppo di gestire le notifiche degli eventi non è temporaneamente disponibile per alcuni [!DNL Workfront] clienti. Per aggiornamenti sulla versione, segui questo articolo: Sblocca la configurazione delle notifiche degli eventi per i gruppi.

Gli amministratori di sistema determinano le notifiche che gli utenti devono ricevere tramite [!DNL Workfront].

![[!UICONTROL Notifiche e-mail] nella finestra [!UICONTROL Configurazione] area](assets/admin-fund-notifications-1.png)

La [!UICONTROL Notifiche degli eventi] elenco è raggruppato per tipo. Per ogni notifica di evento elencata, vedrai cinque informazioni:

* **[!UICONTROL Attivo] —** La [!UICONTROL Attivo] consente di attivare o disattivare una notifica a livello di sistema.
* **[!UICONTROL Nome] —** Questo è il nome della notifica all&#39;interno di [!DNL Workfront].
* **[!UICONTROL Descrizione] —** La descrizione fornisce una breve spiegazione delle azioni intraprese per attivare una notifica o che devono essere intraprese in risposta alla ricezione della notifica.
* **[!UICONTROL Oggetto e-mail] —** Cosa verrà visualizzato all’utente nella riga dell’oggetto quando l’e-mail viene inviata agli utenti.
* **[!UICONTROL Accesso al gruppo] —** Sblocca le notifiche in modo che possano essere gestite dagli amministratori del gruppo.

## Attiva notifiche

Per gestire le notifiche a livello di sistema globale, assicurati che la barra di ricerca indichi [!UICONTROL Notifiche degli eventi di sistema].

Attiva una notifica specifica per renderla disponibile a tutti gli utenti facendo clic sul pulsante di attivazione/disattivazione , in modo che venga visualizzato il blu. Se il blu è nascosto, la notifica è disattivata.

![[!UICONTROL Attivo] colonna [!UICONTROL Notifiche e-mail] page](assets/admin-fund-notifications-2.png)

Una volta attivata la notifica di un evento, i messaggi vengono inviati immediatamente quando si verifica l’evento.

## Consenti controllo amministratore gruppo

Gli amministratori di gruppo possono ricevere l’autorizzazione, da parte degli amministratori di sistema, di personalizzare ulteriormente l’elenco delle notifiche in base al funzionamento dei gruppi e dei sottogruppi e ai relativi flussi di lavoro.

![[!UICONTROL Accesso al gruppo] colonna [!UICONTROL Notifiche e-mail] page](assets/ganotifications_01.png)

Per consentire agli amministratori dei gruppi di gestire le notifiche per i gruppi e i sottogruppi, è necessario sbloccare le notifiche a livello di sistema.

* Passa alla scheda Notifica eventi della pagina Notifiche e-mail.

* Assicurati che la barra di ricerca indichi Notifiche degli eventi di sistema.

* Sblocca una singola notifica per tutti gli amministratori del gruppo facendo clic sull&#39;interruttore nella colonna Accesso al gruppo in modo che venga visualizzato il blu.

* Sblocca più notifiche contemporaneamente selezionando la casella a sinistra di ciascuna notifica e facendo clic sull’icona sblocca nella barra degli strumenti sopra l’elenco.

![[!UICONTROL Accesso al gruppo] colonna [!UICONTROL Notifiche e-mail] page](assets/ganotifications_02.png)

Blocca una notifica sbloccata facendo clic sull’interruttore in modo che venga visualizzato il grigio. Per bloccare più notifiche contemporaneamente, seleziona le caselle di controllo e fai clic sull’icona Sblocca nella barra degli strumenti.

![[!UICONTROL Accesso al gruppo] colonna [!UICONTROL Notifiche e-mail] page](assets/ganotifications_03.png)

Le notifiche sbloccate vengono visualizzate per gli amministratori di gruppo di primo livello per determinare se tale notifica è necessaria per i loro gruppi e sottogruppi. I sottogruppi ereditano le configurazioni di notifica dal gruppo principale. ﻿


## Gestione delle notifiche dei gruppi

Una volta che l’amministratore di sistema ha sbloccato le opzioni di notifica, gli amministratori del gruppo possono gestire le notifiche di un gruppo dalla singola pagina Gruppo, facendo clic su Notifiche evento nel menu del pannello a sinistra. Puoi quindi attivare o disattivare le opzioni di notifica.

![[!UICONTROL Accesso al gruppo] colonna [!UICONTROL Notifiche e-mail] page](assets/managegroupnotifications_01.png)

Se necessario, gli amministratori di sistema possono gestire le notifiche di un gruppo dalla pagina Notifiche immettendo il nome del gruppo nella barra di ricerca nella parte superiore della finestra.

![[!UICONTROL Accesso al gruppo] colonna [!UICONTROL Notifiche e-mail] page](assets/managegroupnotifications_02.png)

## Suggerimenti per i professionisti

Alcune notifiche [!DNL Workfront] consiglia di rendere disponibile agli utenti.

Per la maggior parte degli utenti:

* [!UICONTROL Quando si completa un&#39;attività, invia una Email a tutti gli incaricati di attività dipendenti]
* [!UICONTROL Qualcuno mi include in un aggiornamento diretto]
* [!UICONTROL Qualcuno commenta il mio elemento di lavoro]
* [!UICONTROL La data di scadenza cambia in un&#39;attività a cui sono assegnato]


In particolare per i project manager:

* [!UICONTROL Un progetto su cui sto lavorando diventa attivo]
* [!UICONTROL Quando si cambia lo stato di avanzamento di un progetto da positivo (Nei Tempi) a negativo (In Ritardo), invia una Email al Proprietario del progetto.]
* [!UICONTROL Quando si aggiunge una Issue, invia email al Proprietario del progetto]
* [!UICONTROL Attività Milestone completata su un progetto di cui sono proprietario]

<!---
learn more URLs
--->
