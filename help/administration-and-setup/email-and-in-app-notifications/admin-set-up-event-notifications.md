---
title: Impostare le notifiche degli eventi
description: Scopri come controllare quali notifiche e-mail e in-app vengono ricevute dagli utenti gestendo le notifiche degli eventi.
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

![[!UICONTROL Notifiche e-mail] finestra in [!UICONTROL Configurazione] area](assets/admin-fund-notifications-1.png)

Il [!UICONTROL Notifiche evento] L&#39;elenco è raggruppato per tipo. Per ogni notifica di evento elencata, visualizzerai cinque informazioni:

* **[!UICONTROL Attivo] —** Il [!UICONTROL Attivo] consente di attivare o disattivare una notifica a livello di sistema.
* **[!UICONTROL Nome] —** Nome della notifica in [!DNL Workfront].
* **[!UICONTROL Descrizione] —** La descrizione fornisce una breve spiegazione dell’azione intrapresa per attivare una notifica o che deve essere intrapresa in risposta alla ricezione della notifica.
* **[!UICONTROL Oggetto e-mail] —** Cosa verrà visualizzato all’utente nella riga dell’oggetto quando l’e-mail viene inviata agli utenti.
* **[!UICONTROL Accesso gruppo] —** Sblocca le notifiche in modo che possano essere gestite dagli amministratori di gruppi.

## Attiva notifiche

Per gestire le notifiche a livello di sistema globale, assicurati che la barra di ricerca indichi [!UICONTROL Notifiche eventi di sistema].

Attiva una notifica specifica per renderla disponibile per tutti gli utenti facendo clic sul pulsante di attivazione in modo che venga visualizzata la schermata blu. Se il blu è nascosto, la notifica è disattivata.

![[!UICONTROL Attivo] colonna su [!UICONTROL Notifiche e-mail] pagina](assets/admin-fund-notifications-2.png)

Quando la notifica di un evento è attivata, i messaggi vengono inviati immediatamente quando si verifica l’evento.

## Consenti controllo amministratore gruppo

Gli amministratori di gruppo possono essere autorizzati a personalizzare ulteriormente l’elenco delle notifiche in base al funzionamento dei gruppi e dei sottogruppi e ai flussi di lavoro.

![[!UICONTROL Accesso gruppo] colonna su [!UICONTROL Notifiche e-mail] pagina](assets/ganotifications_01.png)

Per consentire agli amministratori di gruppi di gestire le notifiche per i loro gruppi e sottogruppi, è necessario sbloccare le notifiche a livello di sistema.

* Passa alla scheda Notifica eventi della pagina Notifiche e-mail.

* Assicurarsi che la barra di ricerca indichi Notifiche eventi di sistema.

* Per sbloccare una singola notifica per tutti gli amministratori di gruppi, fai clic sull’interruttore nella colonna Accesso ai gruppi in modo che venga visualizzato il blu.

* Per sbloccare più notifiche contemporaneamente, seleziona la casella a sinistra di ciascuna notifica e fai clic sull’icona di sblocco nella barra degli strumenti sopra l’elenco.

![[!UICONTROL Accesso gruppo] colonna su [!UICONTROL Notifiche e-mail] pagina](assets/ganotifications_02.png)

Blocca una notifica sbloccata facendo clic sull’interruttore in modo che venga visualizzato il grigio. Blocca più notifiche contemporaneamente selezionando le caselle di controllo e facendo clic sull’icona Sblocca nella barra degli strumenti.

![[!UICONTROL Accesso gruppo] colonna su [!UICONTROL Notifiche e-mail] pagina](assets/ganotifications_03.png)

Vengono visualizzate notifiche sbloccate per gli amministratori di gruppi di livello superiore per determinare se tale notifica è necessaria per i loro gruppi e sottogruppi. I sottogruppi ereditano le configurazioni di notifica dal gruppo padre principale. ﻿


## Gestire le notifiche dei gruppi

Dopo che l’amministratore di sistema ha sbloccato le opzioni di notifica, gli amministratori dei gruppi possono gestire le notifiche di un gruppo dalla pagina Gruppo individuale, facendo clic su Notifiche evento nel menu del pannello a sinistra. Quindi puoi attivare o disattivare le opzioni di notifica.

![[!UICONTROL Accesso gruppo] colonna su [!UICONTROL Notifiche e-mail] pagina](assets/managegroupnotifications_01.png)

Se necessario, gli amministratori di sistema possono gestire le notifiche di un gruppo dalla pagina Notifiche immettendo il nome del gruppo nella barra di ricerca nella parte superiore della finestra.

![[!UICONTROL Accesso gruppo] colonna su [!UICONTROL Notifiche e-mail] pagina](assets/managegroupnotifications_02.png)

## Suggerimenti pro

Sono presenti alcune notifiche [!DNL Workfront] consiglia di metterlo a disposizione degli utenti.

Per la maggior parte degli utenti:

* [!UICONTROL Quando si completa un&#39;attività, invia una Email a tutti gli incaricati di attività dipendenti]
* [!UICONTROL Qualcuno mi include in un aggiornamento diretto]
* [!UICONTROL Qualcuno ha commentato il mio elemento di lavoro]
* [!UICONTROL Le modifiche della data di scadenza su un’attività a cui sono assegnato]


In particolare per i project manager:

* [!UICONTROL Quando si attiva un progetto, invia una Email alla squadra]
* [!UICONTROL Quando si cambia lo stato di avanzamento di un progetto da positivo (Nei Tempi) a negativo (In Ritardo), invia una Email al Proprietario del progetto.]
* [!UICONTROL Quando si aggiunge una Issue, invia email al Proprietario del progetto]
* [!UICONTROL L&#39;attività principale è completata su un mio progetto]

<!---
learn more URLs
--->
