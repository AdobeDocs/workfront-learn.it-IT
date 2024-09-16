---
title: Risposte alle domande più comuni sulle code di richieste
description: Ottieni risposte alle domande più comuni sulle code di richieste in [!DNL  Workfront].
feature: Work Management
type: Tutorial
role: Admin, User
level: Beginner
last-substantial-update: 2024-09-16T00:00:00Z
recommendations: noDisplay,noCatalog
jira: KT-10101
exl-id: bfa3ae5f-9618-444c-9eb8-5d82db9a77c7
source-git-commit: e9a4f2bcd39e2598ff540bb4f300e891e817e939
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 50%

---

# Risposte alle domande più comuni sulle code di richieste

**Perché vedo una coda di richieste, ma il mio utente non la vede?**

Nella scheda [!UICONTROL Dettagli coda] della tua coda di richieste o nel tuo progetto, assicurati che l’utente soddisfi i criteri del campo “Chi può aggiungere richieste a questa coda?” .

Per ulteriori informazioni, guarda questo video:

>[!VIDEO](https://video.tv.adobe.com/v/3434156/?quality=12&learn=on)

**Ho concesso agli utenti l’accesso alla coda, ma ora possono vedere anche il progetto della coda delle richieste. Perché?**

Nella sezione &quot;Chi può aggiungere richieste a questa coda?&quot; Se scegli &quot;Persone con accesso di visualizzazione a questo progetto&quot;, chiunque tu dia i diritti di visualizzazione a per poter utilizzare la coda di richieste sarà anche in grado di visualizzare la coda di richieste in un elenco di progetti. Per evitare questo problema, utilizza l’opzione &quot;Persone nell’azienda di questo progetto&quot; o &quot;Persone nel gruppo di questo progetto&quot;.

**Posso trasformare una richiesta in un progetto?**

Sì. Puoi convertire i problemi in attività o progetti in base alle necessità.

Queste esercitazioni ti mostreranno come:

* [Convertire un problema o una richiesta in un progetto](/help/manage-work/issues-requests/create-a-project-from-a-request.md)

* [Convertire un problema/richiesta in un’attività](/help/manage-work/issues-requests/convert-issues-to-other-work-items.md)

**Dove trovo una coda di richieste per apportarvi modifiche?**

Puoi usare il campo [!UICONTROL Ricerca] nella barra di navigazione opure puoi trovarla elencata nell’area [!UICONTROL Progetti].

Se apri una richiesta dalla coda di richieste, puoi fare clic sul nome del progetto nell’area delle breadcrumb.

**Posso trasferire le informazioni da un modulo personalizzato di una richiesta a un modulo personalizzato di un progetto?**

Sì. Quando crei un modulo personalizzato, seleziona [!UICONTROL Progetto] e [!UICONTROL Problema] come tipi di oggetto. È inoltre possibile modificare un modulo personalizzato del progetto per includere il tipo di oggetto problema e viceversa.

Allega il modulo personalizzato alla richiesta. Quando converti la richiesta in un progetto, il modulo personalizzato verrà automaticamente allegato al nuovo progetto e i valori contenuti in tutti i campi verranno visualizzati sia nella richiesta che nei moduli personalizzati del progetto.

**Sto guardando un progetto o un rapporto di attività. Come posso capire da quale richiesta proviene questo oggetto?**

Per aggiungere tali informazioni ai rapporti di progetto e attività, puoi accedere ai campi nelle origini campo **[!UICONTROL Problema convertito]** e il **[!UICONTROL Referente problema convertito]**.

Per ulteriori informazioni, guarda questo video:

>[!VIDEO](https://video.tv.adobe.com/v/3434176/?quality=12&learn=on)


**Qual è il modo migliore per filtrare le code di richieste in un rapporto?**

Se il filtro del progetto include **Coda>>È pubblico>>Uguale a>>Nessuno** il rapporto mostrerà solo i progetti che **NON** sono code di richieste.

Se il filtro del progetto include **Coda>>È pubblico>>Non uguale a>>Nessuno** il rapporto mostrerà solo i progetti che **SONO** code di richieste.

Per ulteriori informazioni, guarda questo video:

>[!VIDEO](https://video.tv.adobe.com/v/3434329/?quality=12&learn=on)

**Creare uno stato personalizzato della coda richieste?**

Alcuni clienti creano uno stato personalizzato di Coda richieste che è uguale a Corrente. Possono quindi eseguire un rapporto che mostra tutte le code di richieste o escludere facilmente le code di richieste da un rapporto. Anche se questo ha il vantaggio di essere più semplice da usare rispetto all&#39;uso di **Coda>>È pubblico>>Non uguale a>>Nessuno**, ha lo svantaggio che le persone che creano code di richieste potrebbero dimenticarsi di usarlo, dal momento che lo stato Attuale funziona allo stesso modo ed è quello che vedranno nella maggior parte del materiale di formazione. Per questo motivo, molti clienti scelgono di non utilizzare uno stato personalizzato Coda richieste.

Tuttavia, se utilizzi già lo stato Coda richieste nell&#39;organizzazione e vuoi solo essere sicuro che venga utilizzato correttamente (o correggere i casi in cui non lo è), puoi creare il rapporto **Code di richieste attive** descritto nel video precedente e modificare il filtro per **Progetto>>Stato è uguale a>>Uguale a>>Corrente** in **Progetto>>Stato>>Uguale a> Corrente**. Verranno visualizzate tutte le code di richieste attive che utilizzano lo stato Corrente anziché lo stato della coda di richieste che si desidera utilizzare. Seleziona tutti i progetti visualizzati ed esegui una modifica in blocco per modificare gli stati in Coda richieste.

## Tutorial consigliati su questo argomento

* [Comprendere le code di richieste](/help/manage-work/request-queues/understand-request-queues.md)
* [Creare una coda di richieste](/help/manage-work/request-queues/create-a-request-queue.md)
* [Comprendere le impostazioni per un flusso di richieste](/help/manage-work/request-queues/understand-settings-for-a-flow-request.md)
* [Creare un flusso di richieste](/help/manage-work/request-queues/create-a-request-flow.md)
* [Creare una coda richieste di feedback dell’amministratore di sistema](/help/manage-work/request-queues/create-a-system-admin-feedback-request-queue.md)
