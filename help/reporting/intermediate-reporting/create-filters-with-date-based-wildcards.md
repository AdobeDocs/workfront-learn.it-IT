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
last-substantial-update: '2025-06-27T00:00:00.000Z'
jira: KT-9082
exl-id: 0f7db4eb-a062-4eb3-99ca-c40d8e266943
doc-type: video
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: c6dd2ac5-f5bd-4e59-9101-25b156918623
subfeature_v2:
  - id: ceb4d94a-32ed-4fea-9724-1339d684b0bc
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-06T13:57:08.996Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 246
ht-degree: 70%

---

# Creare filtri con caratteri jolly basati sulla data

In questo video scoprirai come:

* Scopri quando utilizzare i caratteri jolly basati sulla data
* Comprendere la differenza tra i due caratteri jolly basati su date di Workfront
* Aggiungere un carattere jolly basato su data a un filtro
* Creare una data personalizzata utilizzando caratteri jolly, attributi, operatori e modificatori
* Creare un intervallo di date personalizzato utilizzando caratteri jolly

>[!VIDEO](https://video.tv.adobe.com/v/3412661/?captions=ita&quality=12&learn=on&enablevpops=0)


## Attività &quot;Creare filtri con caratteri jolly basati su date&quot;


### Domande sull’attività

1. Come creeresti la regola di filtro se volessi ottenere problemi con una data di scadenza di ieri o oggi?
1. Come creeresti la regola di filtro per trovare i progetti che erano in scadenza la settimana scorsa?
1. Le regole di filtro seguenti fanno parte di un rapporto sulle attività da utilizzare regolarmente. Che tipo di risultati otterresti da questo rapporto?

![Immagine della schermata per creare un filtro attività con un carattere jolly basato sulla data](assets/date-wildcard-answer-1.png)

### Risposte

1. Filtra in base alla data di completamento pianificata del problema tra [!UICONTROL $$TODAY-1d] e [!UICONTROL $$TODAY].
1. Filtra per data di completamento pianificata del progetto tra [!UICONTROL $$TODAYb-1w] e [!UICONTROL $$TODAYe-1w].
1. Questo report individua le attività assegnate all&#39;utente che non sono ancora terminate (in altre parole, hanno una percentuale di completamento inferiore a 100) e che sono scadute o scadute oggi. La regola di filtro per la data di completamento pianificata delle attività indica di esaminare le attività con una data di scadenza uguale o precedente alla data corrente.
