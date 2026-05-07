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
last-substantial-update: '2025-06-26T00:00:00.000Z'
jira: KT-9081
exl-id: 46c83acd-6e43-42aa-875f-ae24b09a7fee
doc-type: video
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: c6dd2ac5-f5bd-4e59-9101-25b156918623
subfeature_v2: id: ceb4d94a-32ed-4fea-9724-1339d684b0bc
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-06T13:58:26.659Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 362
ht-degree: 46%

---

# Creare filtri con caratteri jolly basati sull’utente

In questo video scoprirai come:

* comprendere a cosa servono i caratteri jolly
* Creare un filtro con un carattere jolly basato sull’utente

>[!VIDEO](https://video.tv.adobe.com/v/336810/?quality=12&learn=on&enablevpops=0)

>[!TIP]
>
>Utilizza il nome e l’origine del campo Utenti dell’assegnazione >> ID durante la creazione di filtri che esaminano le informazioni sulle assegnazioni di attività o problemi.  Questa opzione esamina tutti gli utenti assegnati all’attività o al problema, non solo il &quot;proprietario&quot; o l’assegnatario principale.

>[!TIP]
>
>Utilizza $$USER.ID (invece del tuo nome) anche quando crei filtri per te stesso. In questo modo, se qualcuno vede un filtro che stai utilizzando e dice &quot;condividi con me&quot;, il filtro è già configurato in modo che ogni persona che lo utilizza possa visualizzare le proprie informazioni.

>[!TIP]
>
>È sempre necessario utilizzare il qualificatore del filtro Uguale quando si utilizzano caratteri jolly basati sull’utente.


## Attività &quot;Creare filtri con caratteri jolly basati sugli utenti&quot;

### Attività 1

Questa settimana hai un po&#39; di tempo in più, quindi vuoi vedere se c&#39;è qualcuno nel tuo team che potrebbe usare un po&#39; di assistenza per le sue assegnazioni. Crea un filtro attività per trovare le attività assegnate al team principale in scadenza questa settimana e non ancora completate.

### Risposta 1

Sei fantastico per aiutare i tuoi compagni di squadra! Con il filtro impostato come nell’immagine seguente, troverai le attività:

* Che non sono stati completati (ovvero non hanno uno stato [!UICONTROL Complete] che equivale a [!UICONTROL Complete]);
* che si trovano in progetti con uno stato [!UICONTROL Attuale] (dopo tutto, non desideri trovare attività per progetti che non sono ancora stati avviati);
* che vengono assegnate a qualcuno del team predefinito, come definito dalle impostazioni del team di Workfront;
* E che hanno una data di completamento di questa settimana (questa regola utilizzava il filtro data predefinito per definire &quot;questa settimana&quot;).

![Immagine della schermata per creare un filtro attività con un carattere jolly basato sull’utente](assets/user-wildcard-exercise-answer.png)

Potrebbe essere necessario aggiungere alcuni filtri aggiuntivi desideri limitare ulteriormente l’elenco. Ad esempio, potresti voler aggiungere una regola di filtro che esamini un programma o un portfolio specifico su cui lavora il team.
