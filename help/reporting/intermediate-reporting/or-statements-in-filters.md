---
title: Creare istruzioni OR nei filtri
description: La logica di filtro flessibile di Workfront consente agli utenti di perfezionare le visualizzazioni di reporting utilizzando le regole "E" predefinite, le condizioni "O" facoltative e i gruppi di filtri organizzati per criteri complessi.
activity: use
team: Technical Marketing
feature: Reports and Dashboards
thumbnail: create-or-statements-in-filters.png
type: Tutorial
role: User
level: Intermediate
jira: KT-9987
exl-id: 1a56f2f6-12df-43a5-943c-986a85661efa
last-substantial-update: '2025-08-11T00:00:00.000Z'
doc-type: video
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: c6dd2ac5-f5bd-4e59-9101-25b156918623
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-06T02:11:54.379Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 318
ht-degree: 31%

---

# Creare istruzioni OR nei filtri

Il video spiega come creare e utilizzare i filtri con più regole in Workfront. &#x200B; Per impostazione predefinita, Workfront utilizza &quot;AND&quot; tra le regole del filtro, il che significa che tutte le condizioni devono essere true affinché un elemento venga visualizzato nell’elenco.
In alternativa, è possibile modificare la logica del filtro in &quot;OR&quot;, che visualizza gli elementi che soddisfano una qualsiasi delle condizioni.
Il video illustra anche come creare filtri per le attività utilizzando i gruppi di filtri. &#x200B; Ad esempio, puoi creare due gruppi: uno per le attività incomplete assegnate al team creativo in ritardo e un altro per le attività incomplete assegnate al team creativo non assegnate. &#x200B; All’interno di ciascun gruppo, si applica la logica &quot;AND&quot;, il che significa che tutte le condizioni del gruppo devono essere soddisfatte. &#x200B; La logica &quot;OR&quot; tra i gruppi garantisce la visualizzazione delle attività che soddisfano le condizioni di uno dei due gruppi.

>[!VIDEO](https://video.tv.adobe.com/v/3470692/?quality=12&learn=on&enablevpops=0)

## Attività filtro OR

Desideri trovare attività incomplete che ti sono state assegnate o che non sono state assegnate a nessuno. Hai impostato un filtro simile a quello riportato di seguito. Questo filtro ti darà i risultati desiderati? Perché sì o perché no?

![Immagine di un’istruzione OR creata in modo non corretto in [!DNL Workfront]](assets/or-statement-your-turn-1.png)

### Risposte

No, questo filtro non fornirà i risultati desiderati, ovvero le attività che non sono state completate e che sono state assegnate a te o a nessuno, perché la regola del filtro per la completezza dell&#39;attività si trova solo su un lato dell&#39;operatore OR.

Al contrario, questo filtro genera un elenco che mostra:

* Attività assegnate non completate.
* **PIÙ (OR)**
* Tutte le attività non assegnate, indipendentemente dallo stato.

Il filtro deve essere simile a quello riportato di seguito. Nota che questo filtro ha la regola di filtro per la completezza dell’attività su entrambi i lati dell’operatore OR.

![Immagine di un’istruzione OR creata correttamente in [!DNL Workfront]](assets/or-statement-your-turn-2.png)
