---
title: Applicare un processo di approvazione del problema in una coda di richieste
description: Implementa un processo di approvazione predefinito per semplificare i flussi di lavoro delle richieste, garantendo che le richieste approvate cambino il loro stato in modo appropriato a "Nuovo". Risolvi eventuali problemi relativi alle richieste rifiutate selezionando una modifica di stato in "Non risolvibile".
activity: use
feature: Approvals
thumbnail: 335225.jpeg
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-17578
last-substantial-update: '2025-03-26T00:00:00.000Z'
recommendations: noDisplay,catalog
doc-type: video
exl-id: 9200eeb4-db5d-45c1-9b17-28c6ca04de2d
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: c10f2e93-7a58-4212-aa24-684c265ebe76
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-06T15:58:59.618Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 426
ht-degree: 23%

---

# Applicare un processo di approvazione del problema in una coda di richieste

>[!PREREQUISITES]
>
>* [Creare un flusso di richieste](https://experienceleague.adobe.com/it/docs/workfront-learn/tutorials-workfront/manage-work/request-queues/create-a-request-flow)
>* [Creare un processo di approvazione globale e monouso](https://experienceleague.adobe.com/it/docs/workfront-learn/tutorials-workfront/manage-work/approval-processes-and-milestone-paths/create-a-single-use-approval-process)


Il video illustra il processo di applicazione di un processo di approvazione predefinito durante la creazione di una coda di richieste. &#x200B; Quando viene creata una richiesta, questa inizia con lo stato &quot;Nuovo - In attesa di approvazione&quot; e viene inviata una notifica di approvazione all&#39;approvatore designato. &#x200B; Se approvato, lo stato cambia in &quot;Nuovo&quot;, consentendo alle persone assegnate di iniziare il lavoro. &#x200B; Se viene rifiutato, lo stato potrebbe tornare erroneamente a &quot;Nuovo&quot; a causa di un errore comune nella configurazione del processo di approvazione. &#x200B;
Nel video viene evidenziato che il processo di approvazione viene attivato quando lo stato è impostato su &quot;Nuovo&quot;, che è l’impostazione predefinita per le nuove richieste. &#x200B; Se viene rifiutato, per impostazione predefinita il sistema ripristina lo stato precedente, che non è ideale per le nuove richieste. &#x200B;, invece, deve essere scelto uno stato diverso, ad esempio &quot;Non risolverai&quot;. &#x200B; Nel video viene inoltre indicato che per impostazione predefinita non è stato fornito lo stato &quot;Rifiutato&quot;, ma che un amministratore di sistema può crearne uno in base alle esigenze. &#x200B;

>[!VIDEO](https://video.tv.adobe.com/v/3455013/?quality=12&learn=on&enablevpops=1)

## Concetti chiave

* **Processo di approvazione predefinito:** Durante la creazione di una coda di richieste, è possibile applicare un processo di approvazione predefinito che assegna automaticamente un flusso di lavoro di approvazione a ogni richiesta.
* **Modifiche di stato all&#39;approvazione:** Le richieste approvate cambiano lo stato da &quot;Nuovo - In attesa di approvazione&quot; a &quot;Nuovo&quot;, consentendo alle persone assegnate di iniziare a lavorarci.
* **Errore comune nella gestione dei rifiuti:** Se una richiesta viene rifiutata, lo stato verrà ripristinato a &quot;Nuovo&quot; a causa di un&#39;impostazione di sistema predefinita nel processo di approvazione.
* **Stato consigliato per richieste rifiutate:** Anziché ripristinare lo stato precedente (&quot;Nuovo&quot;), è preferibile scegliere uno stato diverso, ad esempio &quot;Non risolverlo&quot;, per evitare confusione.
* **Opzioni di stato personalizzate:** Per impostazione predefinita non è stato fornito lo stato &quot;Rifiutato&quot;, ma un amministratore di sistema può crearne uno se necessario per una maggiore chiarezza nel processo di approvazione.


## Tutorial consigliati su questo argomento

* [Delegare attività, problemi e approvazioni](/help/manage-work/approval-processes-and-milestone-paths/delegate-approvals.md)
* [Comprendere i processi di approvazione specifici del gruppo](/help/administration-and-setup/approval-processes-and-milestone-paths/group-specific-approval-processes.md)
* [Creare un flusso di richieste](/help/manage-work/request-queues/create-a-request-flow.md)
* [Creare un processo di approvazione globale e monouso](https://experienceleague.adobe.com/it/docs/workfront-learn/tutorials-workfront/manage-work/approval-processes-and-milestone-paths/create-a-single-use-approval-process)
