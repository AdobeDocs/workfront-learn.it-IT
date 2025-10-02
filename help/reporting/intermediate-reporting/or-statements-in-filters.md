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
last-substantial-update: 2025-08-11T00:00:00Z
doc-type: video
source-git-commit: bbdf99c6bc1be714077fd94fc3f8325394de36b3
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 31%

---

# Creare istruzioni OR nei filtri

Il video spiega come creare e utilizzare i filtri con più regole in Workfront. &#x200B; Per impostazione predefinita, Workfront utilizza &quot;AND&quot; tra le regole del filtro, il che significa che tutte le condizioni devono essere true affinché un elemento venga visualizzato nell’elenco.
In alternativa, è possibile modificare la logica del filtro in &quot;OR&quot;, che visualizza gli elementi che soddisfano una qualsiasi delle condizioni.
Il video illustra anche come creare filtri per le attività utilizzando i gruppi di filtri. &#x200B; Ad esempio, puoi creare due gruppi: uno per le attività incomplete assegnate al team creativo in ritardo e un altro per le attività incomplete assegnate al team creativo non assegnate. &#x200B; All&#39;interno di ogni gruppo, si applica la logica &quot;AND&quot;, il che significa che tutte le condizioni del gruppo devono essere soddisfatte. &#x200B; La logica &quot;OR&quot; tra i gruppi consente di visualizzare le attività che soddisfano le condizioni di uno dei due gruppi.

>[!VIDEO] (https://video.tv.adobe.com/v/3470701/?quality=12&learn=on&enablevpops=0&captions=ita

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
