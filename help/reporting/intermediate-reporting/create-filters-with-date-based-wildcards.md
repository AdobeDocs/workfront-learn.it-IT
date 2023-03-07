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
kt: 9082
exl-id: 0f7db4eb-a062-4eb3-99ca-c40d8e266943
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---

# Creare filtri con caratteri jolly basati sulla data

Questo video illustra come:

* Sapere quando utilizzare i caratteri jolly basati sulla data
* Comprendere la differenza tra i due caratteri jolly basati su date di Workfront
* Aggiungere un carattere jolly basato su data a un filtro
* Creare una data personalizzata utilizzando caratteri jolly, attributi, operatori e modificatori
* Creare un intervallo di date personalizzato utilizzando caratteri jolly

>[!VIDEO](https://video.tv.adobe.com/v/336812/?quality=12)

## Domande sull’attività

1. Come creeresti la regola di filtro se desideri problemi con scadenza ieri o oggi?
1. Come si crea la regola di filtro per trovare i progetti in scadenza la settimana scorsa?
1. Le seguenti regole di filtro fanno parte di un rapporto di attività utilizzato regolarmente. Che tipo di risultati otterresti da questo rapporto?

![Immagine della schermata per creare un filtro attività con un carattere jolly basato sulla data](assets/date-wildcard-answer-1.png)

## Risposte

1. Filtra in base alla data di completamento pianificata del problema tra [!UICONTROL $$OGGI-1g] e [!UICONTROL $$OGGI].
1. Filtra per data di completamento pianificata del progetto tra [!UICONTROL $$OGGIb-1w] e [!UICONTROL $$TODAYe-1w].
1. Questo report individua le attività assegnate all&#39;utente che non sono ancora terminate (in altre parole, hanno una percentuale di completamento inferiore a 100) e che sono scadute o scadute oggi. La regola di filtro per la data di completamento pianificata delle attività indica di esaminare le attività con una data di scadenza uguale o precedente alla data corrente.
