---
title: Creare filtri con caratteri jolly basati sull'utente
description: Scopri come utilizzare i caratteri jolly basati sugli utenti e come creare un filtro basato sull’utente connesso.
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
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 0%

---

# Creare filtri con caratteri jolly basati sull&#39;utente

Questo video illustra come:

* Perché utilizzare i caratteri jolly
* Creare un filtro con un carattere jolly basato sull&#39;utente

>[!VIDEO](https://video.tv.adobe.com/v/336810/?quality=12&learn=on)

>[!TIP]
>
>Utilizza l’origine e il nome del campo Utenti assegnazione >> ID quando crei filtri che esaminano le informazioni sull’assegnazione di un’attività o di un problema.  Questa opzione esamina tutti gli utenti assegnati all’attività o al problema, non solo il &quot;proprietario&quot; o l’assegnatario principale.

>[!TIP]
>
>Usa $$USER.ID (invece del tuo nome) anche quando crei dei filtri per te stesso. In questo modo, se qualcuno visualizza un filtro che stai utilizzando e dice &quot;condividi con me&quot;, il filtro è già configurato in modo che ogni persona che lo utilizza visualizzi le proprie informazioni.

>[!TIP]
>
>Quando si utilizzano caratteri jolly basati sull&#39;utente, è sempre necessario utilizzare il qualificatore di filtro Equal.

## Attività

Questa settimana hai un po’ di tempo in più, quindi vuoi vedere se c’è qualcuno nel tuo team che potrebbe usare un po’ di assistenza per le sue assegnazioni. Crea un filtro attività per trovare le attività in scadenza questa settimana che non sono state completate.

## Risposta

Sei fantastico per aiutare i tuoi compagni di squadra! Con il filtro impostato come nell’immagine seguente, troverai le attività:

* Che non sono stati completati (il che significa che non hanno un [!UICONTROL Completa] stato o stato che equivale a [!UICONTROL Completa]);
* che si trovano in progetti con [!UICONTROL Corrente] stato (dopo tutto, non desideri trovare attività per progetti che non sono ancora stati avviati);
* Assegnate a un utente del team principale, come definito dalle impostazioni del team Workfront;
* E che hanno una data di completamento di questa settimana (questa regola utilizzava il filtro data predefinito per definire &quot;questa settimana&quot;).

![Immagine della schermata per creare un filtro attività con un carattere jolly basato sull&#39;utente](assets/user-wildcard-exercise-answer.png)

Per limitare ulteriormente l’elenco, potrebbe essere necessario aggiungere altri filtri. Ad esempio, potrebbe essere utile aggiungere una regola di filtro che analizzi un programma o un portfolio specifico da cui lavora il team.
