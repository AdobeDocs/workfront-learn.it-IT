---
title: Creare filtri con caratteri jolly basati sulla data
description: Scopri come e quando utilizzare i caratteri jolly basati sulla data e come creare un filtro basato sulla data corrente.
activity: use
feature: Reports and Dashboards
thumbnail: 336812.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-9082
exl-id: 0f7db4eb-a062-4eb3-99ca-c40d8e266943
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: ht
source-wordcount: '231'
ht-degree: 100%

---

# Creare filtri con caratteri jolly basati sulla data

In questo video scoprirai come:

* Scopri quando utilizzare i caratteri jolly basati sulla data
* Informazioni sulla differenza tra i due caratteri jolly basati su date di Workfront
* Aggiungere un carattere jolly basato su data a un filtro
* Creare una data personalizzata utilizzando caratteri jolly, attributi, operatori e modificatori
* Creare un intervallo di date personalizzato utilizzando caratteri jolly

>[!VIDEO](https://video.tv.adobe.com/v/336812/?quality=12&learn=on)

## Domande sull’attività

1. Come creeresti la regola di filtro se volessi ottenere problemi con una data di scadenza di ieri o oggi?
1. Come creeresti la regola di filtro per trovare i progetti che erano in scadenza la settimana scorsa?
1. Le regole di filtro seguenti fanno parte di un rapporto sulle attività da utilizzare regolarmente. Che tipo di risultati otterresti da questo rapporto?

![Immagine della schermata per creare un filtro attività con un carattere jolly basato sulla data](assets/date-wildcard-answer-1.png)

## Risposte

1. Filtra in base alla data di completamento pianificata del problema tra [!UICONTROL $$TODAY-1d] e [!UICONTROL $$TODAY].
1. Filtra per data di completamento pianificata del progetto tra [!UICONTROL $$TODAYb-1w] e [!UICONTROL $$TODAYe-1w].
1. Questo rapporto trova le attività assegnate all’utente che non sono ancora state completate (in altre parole, hanno una percentuale di completamento inferiore a 100) e che sono in ritardo o in scadenza oggi. La regola di filtro per la data di completamento pianificata delle attività indica di esaminare le attività con una data di scadenza uguale o precedente al giorno attuale.
