---
source-git-commit: b150105844a42e06f5e96f787ad62a1b62185f91
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 18%

---
# Applicare un processo di approvazione del problema in una coda di richieste - CONDIVISO

>[!PREREQUISITES]
>
>* [Crea un flusso di richieste in Workfront](https://experienceleague.adobe.com/it/docs/workfront-learn/tutorials-workfront/manage-work/request-queues/create-a-request-flow)
>* [Creare e gestire i processi di approvazione](https://experienceleague.adobe.com/it/docs/workfront-learn/tutorials-workfront/manage-work/approval-processes-and-milestone-paths/create-a-single-use-approval-process)


Il video illustra il processo di applicazione di un processo di approvazione predefinito durante la creazione di una coda di richieste. &#x200B; Quando viene creata una richiesta, questa inizia con lo stato &quot;Nuovo - In attesa di approvazione&quot; e viene inviata una notifica di approvazione all&#39;approvatore designato. &#x200B; Se approvato, lo stato cambia in &quot;Nuovo&quot;, consentendo alle persone assegnate di iniziare il lavoro. &#x200B; Se viene rifiutato, lo stato potrebbe tornare erroneamente a &quot;Nuovo&quot; a causa di un errore comune nella configurazione del processo di approvazione. &#x200B;
Nel video viene evidenziato che il processo di approvazione viene attivato quando lo stato è impostato su &quot;Nuovo&quot;, che è l’impostazione predefinita per le nuove richieste. &#x200B; Se viene rifiutato, per impostazione predefinita il sistema ripristina lo stato precedente, che non è ideale per le nuove richieste. &#x200B;, invece, deve essere scelto uno stato diverso, ad esempio &quot;Non risolverai&quot;. &#x200B; Nel video viene inoltre indicato che per impostazione predefinita non è stato fornito lo stato &quot;Rifiutato&quot;, ma che un amministratore di sistema può crearne uno in base alle esigenze. &#x200B;

>[!VIDEO](https://video.tv.adobe.com/v/3455032/?captions=ita&quality=12&learn=on&enablevpops=1)

## Concetti chiave

* **Processo di approvazione predefinito:** Durante la creazione di una coda di richieste, è possibile applicare un processo di approvazione predefinito che assegna automaticamente un flusso di lavoro di approvazione a ogni richiesta.
* **Modifiche di stato all&#39;approvazione:** Le richieste approvate cambiano lo stato da &quot;Nuovo - In attesa di approvazione&quot; a &quot;Nuovo&quot;, consentendo alle persone assegnate di iniziare a lavorarci.
* **Errore comune nella gestione dei rifiuti:** Se una richiesta viene rifiutata, lo stato verrà ripristinato a &quot;Nuovo&quot; a causa di un&#39;impostazione di sistema predefinita nel processo di approvazione.
* **Stato consigliato per richieste rifiutate:** Anziché ripristinare lo stato precedente (&quot;Nuovo&quot;), è preferibile scegliere uno stato diverso, ad esempio &quot;Non risolverlo&quot;, per evitare confusione.
* **Opzioni di stato personalizzate:** Per impostazione predefinita non è stato fornito lo stato &quot;Rifiutato&quot;, ma un amministratore di sistema può crearne uno se necessario per una maggiore chiarezza nel processo di approvazione.


## Tutorial consigliati su questo argomento

* [Delega in modo efficace attività, problemi e approvazioni](/help/manage-work/approval-processes-and-milestone-paths/delegate-approvals.md)
* [Comprendere i processi di approvazione specifici del gruppo](/help/administration-and-setup/approval-processes-and-milestone-paths/group-specific-approval-processes.md)
* [Creare un flusso di richieste in Workfront](/help/manage-work/request-queues/create-a-request-flow.md)
* [Creare e gestire i processi di approvazione](https://experienceleague.adobe.com/it/docs/workfront-learn/tutorials-workfront/manage-work/approval-processes-and-milestone-paths/create-a-single-use-approval-process)

