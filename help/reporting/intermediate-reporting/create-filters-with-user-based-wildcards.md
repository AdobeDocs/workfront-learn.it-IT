---
title: Creare filtri con caratteri jolly basati sull’utente
description: Scopri come utilizzare i caratteri jolly basati sull’utente e come creare un filtro basato sull’utente che ha effettuato l’accesso.
activity: use
feature: Reports and Dashboards
thumbnail: 336810.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-9081
exl-id: 46c83acd-6e43-42aa-875f-ae24b09a7fee
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: ht
source-wordcount: '340'
ht-degree: 100%

---

# Creare filtri con caratteri jolly basati sull’utente

In questo video scoprirai come:

* comprendere a cosa servono i caratteri jolly
* Creare un filtro con un carattere jolly basato sull’utente

>[!VIDEO](https://video.tv.adobe.com/v/336810/?quality=12&learn=on)

>[!TIP]
>
>Utilizza il nome e l’origine del campo Utenti dell’assegnazione >> ID durante la creazione di filtri che esaminano le informazioni sulle assegnazioni di attività o problemi.  Questa opzione esamina tutti gli utenti a cui è stata assegnata l’attività o il problema, non solo il “proprietario” o l’assegnatario principale.

>[!TIP]
>
>Utilizza $$USER.ID (invece del tuo nome) anche quando crei filtri per te stesso. In questo modo, se qualcuno visualizza un filtro che stai utilizzando e chiede di condividerlo, il filtro è già configurato in modo che ogni persona che lo utilizza visualizzi le proprie informazioni.

>[!TIP]
>
>È sempre necessario utilizzare il qualificatore del filtro Uguale quando si utilizzano caratteri jolly basati sull’utente.

## Attività

Questa settimana, disponi di più tempo, quindi desideri vedere se c’è qualcuno nel tuo team a cui potrebbe servire aiuto nelle assegnazioni. Crea un filtro attività per trovare le attività in scadenza questa settimana che non sono state completate.

## Risposta

Complimenti per l’aiuto che vuoi offrire agli altri membri del team! Con il filtro impostato come nell’immagine seguente, troverai le attività:

* che non sono state completate (il che significa che non hanno uno stato [!UICONTROL Completato] o uno stato che equivale a [!UICONTROL Completato]);
* che fanno parte di progetti con stato [!UICONTROL Attuale] (dopo tutto, non vuoi trovare attività per progetti che non sono ancora stati avviati);
* che vengono assegnate a qualcuno del team predefinito, come definito dalle impostazioni del team di Workfront;
* e che hanno una data di completamento di questa settimana (questa regola utilizzava il filtro della data predefinito per definire “questa settimana”).

![Immagine della schermata per creare un filtro attività con un carattere jolly basato sull’utente](assets/user-wildcard-exercise-answer.png)

Potrebbe essere necessario aggiungere alcuni filtri aggiuntivi desideri limitare ulteriormente l’elenco. Ad esempio, potresti voler aggiungere una regola di filtro che esamini un programma o un portfolio specifico su cui lavora il team.
