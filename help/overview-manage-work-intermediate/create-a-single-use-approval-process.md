---
title: Creare un processo di approvazione globale e monouso
description: Scopri come creare un processo di approvazione globale e a utente singolo per un progetto, un’attività o un problema.
activity: use
feature: Approvals
thumbnail: 335225.jpeg
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-8962
hide: true
doc-type: video
exl-id: e80dd36f-7aab-4cf1-873c-92dba684c13c
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-05T19:20:03.459Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 448
ht-degree: 95%

---

# Creare un processo di approvazione globale e monouso

I processi di approvazione su progetti, attività e problemi consentono a un project manager di ottenere la conferma da parte di esperti che il lavoro è stato svolto prima di procedere. Il project manager può creare un processo di approvazione per ogni situazione (noto come processo di approvazione monouso) o scegliere da un elenco di molti processi di approvazione creati in precedenza per soddisfare esigenze comuni (noti come processi di approvazione globali o esistenti).

In entrambi i casi, quando lo stato dell’oggetto cambia in quello specificato nel processo di approvazione, l’approvatore viene informato in vari modi per rivedere il lavoro e approvarlo o rifiutarlo. Dato che l’intero progetto può essere messo in pausa in attesa dell’approvazione, gli approvatori dovrebbero essere consapevoli in anticipo che potrebbero essere chiamati per un’approvazione. Se un approvatore è assente dall’incarico per qualsiasi motivo, può delegare le proprie approvazioni a un sostituto qualificato. Per maggiori informazioni, consulta [Delegare attività, problemi e approvazioni](/help/manage-work/approval-processes-and-milestone-paths/delegate-approvals.md).

Questo video illustra come creare un processo di approvazione globale e un processo di approvazione monouso per un progetto, un’attività o un problema.

>[!VIDEO](https://video.tv.adobe.com/v/335225/?quality=12&learn=on&enablevpops=1)

>[!TIP]
>
>È possibile aggiungere un processo di approvazione per singolo utilizzo per un progetto o un’attività a un modello di progetto.

>[!NOTE]
>
>Puoi impostare un’approvazione per singolo utilizzo su progetti e problemi nello stesso modo descritto per le attività nel video.

## Applicare le approvazioni automatiche dei problemi in una coda di richieste

Se desideri impostare approvazioni automatiche dei problemi in una coda richieste, queste possono essere eseguite solo utilizzando un processo di approvazione dei problemi globale e applicate in un [!UICONTROL argomento coda].

Durante la creazione o la modifica di un [!UICONTROL argomento coda], seleziona il processo di approvazione globale nel campo **[!UICONTROL Approvazione predefinita]**.

![Immagine che mostra come selezionare un processo di approvazione predefinito in un argomento coda](assets/automatic-issue-approval-1.png)

Potrebbe essere necessario modificare il processo di approvazione del problema per assicurarsi che lo **[!UICONTROL stato Precedente]** non sia quello impostato per il rifiuto dell’approvazione. Questo perché lo stato precedente è **[!UICONTROL Nuovo]** e questo è anche lo stato che attiva il processo di approvazione, quindi è lo stato in cui verrà impostato quando approvato. Per evitare confusione quando l’approvazione del problema viene rifiutata, è meglio impostare lo stato su qualcosa come **[!UICONTROL Impossibile risolvere]** o uno stato personalizzato creato a questo scopo.

![Immagine che mostra la modifica dello stato da utilizzare quando il problema viene rifiutato](assets/automatic-issue-approval-2.png)


## Tutorial consigliati su questo argomento

* [Delegare attività, problemi e approvazioni](/help/manage-work/approval-processes-and-milestone-paths/delegate-approvals.md)
* [Comprendere i processi di approvazione specifici del gruppo](/help/administration-and-setup/approval-processes-and-milestone-paths/group-specific-approval-processes.md)
* [Creare un flusso di richieste](/help/manage-work/request-queues/create-a-request-flow.md)

