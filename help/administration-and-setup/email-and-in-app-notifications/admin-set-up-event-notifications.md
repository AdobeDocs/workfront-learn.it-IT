---
title: Impostare le notifiche degli eventi
description: Scopri come gestire le notifiche degli eventi per determinare quali notifiche e-mail e in-app inviare agli utenti.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate
thumbnail: 10093.jpeg
jira: KT-10093
exl-id: 6bd3a777-0ed8-4383-ad8e-f1238e334e78
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: ht
source-wordcount: '621'
ht-degree: 100%

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
>A causa di un rollout graduale, la funzionalità che consente agli amministratori di sistema e dei gruppi di gestire le notifiche degli eventi non è al momento disponibile per alcuni clienti di [!DNL Workfront]. Per aggiornamenti sul rilascio di questa funzione, segui questo articolo: Sbloccare la configurazione delle notifiche degli eventi per i gruppi.

Gli amministratori di sistema determinano quali notifiche potranno essere ricevute dagli utenti tramite [!DNL Workfront].

![[!UICONTROL Finestra Notifiche e-mail] nell’area [!UICONTROL Configurazione]](assets/admin-fund-notifications-1.png)

L’elenco [!UICONTROL Notifiche eventi] è raggruppato per tipo. Per ogni notifica evento elencata, sono disponibili cinque informazioni:

* **[!UICONTROL Attivo]:** la colonna [!UICONTROL Attivo] consente di attivare o disattivare una notifica a livello di sistema.
* **[!UICONTROL Nome]:** è il nome della notifica all’interno di [!DNL Workfront].
* **[!UICONTROL Descrizione]:** fornisce una breve spiegazione di quale azione è stata eseguita per attivare una notifica o deve essere intrapresa in risposta alla ricezione della notifica.
* **[!UICONTROL Oggetto e-mail]:** testo da inserire nella riga dell’oggetto quando l’e-mail viene inviata agli utenti.
* **[!UICONTROL Accesso ai gruppi]:** sblocca le notifiche in modo che possano essere gestite dagli amministratori dei gruppi.

## Attiva le notifiche

Per gestire le notifiche a livello di sistema globale, assicurati che la barra di ricerca indichi [!UICONTROL Notifiche eventi di sistema].

Per attivare una notifica specifica e renderla disponibile per tutti gli utenti, fai clic sull’interruttore in modo che diventi blu. Se il blu è nascosto, la notifica è disattivata.

![[!UICONTROL Colonna Attivo] sulla pagina [!UICONTROL Notifiche e-mail]](assets/admin-fund-notifications-2.png)

Una volta attivata una notifica evento, i messaggi saranno inviati non appena si verifica l’evento.

## Consenti il controllo Amministratore gruppo

Gli amministratori di sistema possono concedere agli amministratori dei gruppi l’autorizzazione necessaria per personalizzare ulteriormente l’elenco delle notifiche, in base al ruolo dei rispettivi gruppi e sottogruppi, e in base ai loro loro flussi di lavoro.

![[!UICONTROL Colonna Accesso ai gruppi] sulla pagina [!UICONTROL Notifiche e-mail]](assets/ganotifications_01.png)

Per consentire agli amministratori dei gruppi di gestire le notifiche per i propri gruppi e sottogruppi, è necessario sbloccare le notifiche a livello di sistema.

* Passa alla scheda Notifica evento della pagina Notifiche e-mail.

* Assicurati che la barra di ricerca indichi Notifiche eventi di sistema.

* Per sbloccar una singola notifica per tutti gli amministratori dei gruppi, fai clic sull’interruttore nella colonna Accesso ai gruppi, in modo che diventi blu.

* Per sbloccare più notifiche contemporaneamente, seleziona la casella a sinistra di ciascuna notifica e fai clic sull’icona di sblocco nella barra degli strumenti sopra l’elenco.

![[!UICONTROL Colonna Accesso ai gruppi] sulla pagina [!UICONTROL Notifiche e-mail]](assets/ganotifications_02.png)

Per bloccare una notifica sbloccata, fai clic sull’interruttore in modo che diventi grigio. Per bloccare più notifiche contemporaneamente, selezionane le caselle di controllo e fai clic sull’icona Sblocca nella barra degli strumenti.

![[!UICONTROL Colonna Accesso ai gruppi] sulla pagina [!UICONTROL Notifiche e-mail]](assets/ganotifications_03.png)

Le notifiche sbloccate vengono visualizzate dagli amministratori dei gruppi di livello superiore per determinare se tale notifica è necessaria per i loro gruppi e sottogruppi. I sottogruppi ereditano le configurazioni di notifica dal primo gruppo principale. ﻿


## Gestire le notifiche dei gruppi

Dopo che l’amministratore di sistema ha sbloccato le opzioni di notifica, gli amministratori dei gruppi possono gestire le notifiche di un gruppo dalla pagina di un gruppo, facendo clic su Notifiche eventi nel menu del pannello a sinistra. Quindi puoi attivare o disattivare le opzioni di notifica.

![[!UICONTROL Colonna Accesso ai gruppi] sulla pagina [!UICONTROL Notifiche e-mail]](assets/managegroupnotifications_01.png)

Se necessario, gli amministratori di sistema possono gestire le notifiche dei gruppi dalla pagina Notifiche immettendo il nome del gruppo nella barra di ricerca, nella parte superiore della finestra.

![[!UICONTROL Colonna Accesso gruppo] sulla pagina [!UICONTROL Notifiche e-mail]](assets/managegroupnotifications_02.png)

## Suggerimenti professionali

Ci sono alcune notifiche che [!DNL Workfront] consiglia di mettere a disposizione degli utenti.

Per la maggior parte degli utenti:

* [!UICONTROL Il predecessore di una delle mie attività è stato completato]
* [!UICONTROL Qualcuno mi include in un aggiornamento diretto]
* [!UICONTROL Qualcuno ha commentato il mio elemento di lavoro]
* [!UICONTROL La data di scadenza cambia per un’attività che mi è stata assegnata]


In particolare, per i project manager:

* [!UICONTROL Un progetto a cui partecipo venta attivo]
* [!UICONTROL Un progettodi mia proprietà è in ritardo]
* [!UICONTROL Viene aggiunto un problema a un progetto di cui sono proprietario]
* [!UICONTROL L’attività milestone è completata in un progetto di cui sono proprietario]

<!---
learn more URLs
--->
