---
title: Convertire i problemi in altri elementi di lavoro
description: Scopri come convertire i problemi in altri elementi di lavoro .
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: convert-issues-to-other-work-items.jpeg
type: Tutorial
role: User
level: Intermediate
kt: 10069
exl-id: 1fd4d862-e44b-4c50-9663-70e727f6e9b7
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '1098'
ht-degree: 0%

---

# Conversione di problemi in altri elementi di lavoro

## Convertire un problema in un’attività

Un problema può essere abbastanza significativo che il tempo e lo sforzo per risolverlo devono essere contabilizzati nella tempistica del progetto e allocare le risorse appropriate. In questo caso, il problema può essere convertito in un’attività.

![Un&#39;immagine del [!UICONTROL Converti in attività] opzione di un problema in [!UICONTROL Workfront].](assets/15-convert-issue-to-task-menu-option.png)

1. Passa a [!UICONTROL Problemi] sezione del progetto o dell&#39;attività su cui il problema è connesso. Oppure trova il problema in un report a cui hai accesso.
1. Fai clic sul nome del problema per aprirlo.
1. Dal menu a 3 punti a destra del nome del problema, seleziona **[!UICONTROL Converti in attività]**.
1. Compila il [!UICONTROL Converti in attività] modulo. Iniziare assegnando un nome e una descrizione alla nuova attività.
1. Se la nuova attività deve far parte di un progetto diverso, immettere il nome del progetto.
1. In [!UICONTROL Opzioni] selezionare le caselle per mantenere il problema originale, consentire l&#39;accesso alla nuova attività e mantenere la data di completamento. Quando effettui queste selezioni, segui il flusso di lavoro della tua organizzazione. Allegare un modulo personalizzato se si desidera trasferire i dati del modulo personalizzato dal problema all’attività. (Tutti i campi presenti sia nel modulo del problema che nel modulo attività verranno automaticamente trasferiti al modulo.)
1. Compilare il modulo personalizzato, se allegato.
1. Fai clic su **[!UICONTROL Converti in attività]** per finire.

![Un&#39;immagine del [!UICONTROL Converti in attività] forma di un problema in [!UICONTROL Workfront].](assets/16-convert-to-task-options.png)

A seconda del [!DNL Workfront] impostazioni di sistema, è possibile modificare o meno le impostazioni nella sezione Opzioni durante la conversione dell&#39;attività. Queste opzioni influiscono sia sul problema originale che sulla nuova attività.

* **&quot;Mantenere il problema originale e legarne la risoluzione a questo compito&quot;** conserva il problema originale e le relative informazioni (ore, documenti, ecc.). Con questa opzione selezionata, al termine dell’attività il problema verrà contrassegnato come risolto. Se questa opzione non è selezionata, il problema originale verrà eliminato al completamento dell&#39;attività. Questo può influenzare il modo in cui l&#39;organizzazione tiene traccia e genera rapporti sui problemi.
* La **&quot;Consenti accesso a questa attività a (nome utente)&quot;** consentirà alla persona che ha creato il problema di accedere a questa nuova attività.
* La **&quot;Conserva la data di completamento pianificata del problema&quot;** consente di mantenere la data di completamento pianificata già impostata sul problema. Imposta il vincolo dell&#39;attività su [!UICONTROL Fine entro]. Se la casella è deselezionata, le date dell’attività verranno impostate come se all’interno del progetto venisse creata una nuova attività.

La nuova attività viene posizionata in fondo all’elenco delle attività del progetto. Sposta l’attività nella posizione desiderata, assegna un utente o un team al lavoro, aggiungi ore e durata pianificate, ecc.

>[!NOTE]
>
>Non puoi aggiungere problemi alla timeline del progetto, poiché rappresentano un &quot;lavoro non pianificato&quot;. La tempistica del progetto è &quot;lavoro pianificato&quot;, ovvero attività.

## Convertire un problema in un progetto

Ci sono casi in cui un problema non può essere risolto affrontando il problema stesso o convertendolo in un&#39;attività, perché il processo di risoluzione del problema deve essere coordinato più accuratamente. In questo caso, puoi convertire il problema in un progetto.

1. Passa alla sezione Problemi del progetto o dell&#39;attività su cui il problema è connesso. Oppure trova il problema in un report a cui hai accesso.
1. Fai clic sul nome del problema per aprirlo.
1. Fai clic sul menu a 3 punti a destra del nome del problema per visualizzare il menu Altro .
1. Quindi seleziona se desideri creare un nuovo progetto completamente vuoto o utilizza un modello di progetto, che precompila le informazioni sull’attività e sulla timeline.
1. Compila le informazioni nella finestra Converti in progetto, a partire dal nome del progetto.
1. Compila gli altri dettagli del progetto richiesti dal team o dall’organizzazione.
1. Nella sezione Opzioni , seleziona le caselle per mantenere il problema originale e consentire l’accesso al nuovo progetto. Quando effettui queste selezioni, segui il flusso di lavoro della tua organizzazione.
1. Compilare il modulo personalizzato, se allegato. Allega un modulo personalizzato se desideri trasferire i dati del modulo personalizzato dal problema al progetto. (Tutti i campi presenti sia nel modulo per il problema che nel modulo per il progetto verranno automaticamente trasferiti al modulo per il progetto.)
1. Fai clic su **Converti in progetto** per finire.

I campi dei dettagli del progetto visualizzati nella finestra Converti in progetto dipendono dal metodo utilizzato per creare il progetto. Nel menu a sinistra sono disponibili ulteriori informazioni se è stata utilizzata l’opzione Converti in progetto da modello.

>[!NOTE]
>
>Alcune sezioni, come la sezione Opzioni, anche se visibili, potrebbero essere inaccessibili a seconda delle impostazioni di sistema Workfront della tua organizzazione.

![Immagine di una schermata di un progetto che mostra le opzioni di conversione](assets/conversion-options.png)

* Fai clic su &quot;**Mantenere il problema originale e legarne la risoluzione a questo progetto**&quot; opzione. Questa opzione conserva il problema originale e le relative informazioni (ore, documenti, ecc.). Al termine del nuovo progetto, il problema viene contrassegnato come risolto. Se questa opzione non è selezionata, il problema originale verrà eliminato al completamento del progetto. Questo può influenzare il modo in cui l&#39;organizzazione tiene traccia e genera rapporti sui problemi.
* &quot;**Consenti accesso al progetto (nome utente)**&quot; consente alla persona che ha creato il problema di accedere al progetto in fase di creazione.

## Gestisci informazioni durante il processo di conversione

<!-- Need link to wf one doc article below 

To learn about what information transfers when you convert an issue to a task or project, we recommend you read through the conversion considerations in the article, Convert issues. This lists what information is kept when converting issues and what isn’t. Workfront recommends you become familiar with these considerations so you don’t lose important information when converting issues to tasks or projects.

-->

Il trasferimento dei dati del modulo personalizzato richiede:

* Più copie dello stesso modulo personalizzato, una per il problema e una per l’attività o il progetto. I campi di questi moduli personalizzati devono corrispondere esattamente, in modo che le informazioni possano essere trasferite da un modulo personalizzato all’altro.

* Oppure un singolo modulo personalizzato in cui vengono selezionati il problema, l’attività e/o gli oggetti del progetto. Questo metodo consente di creare e gestire campi personalizzati in un solo modulo personalizzato. Si tratta di un miglioramento recente ed è molto più facile che avere più copie dello stesso modulo, ma entrambi i metodi funzioneranno.



<!-- Need link to wf one doc article below

Learn more in the article, Transfer custom form data to a larger work item.

-->

<!-- Pro tips graphic -->

Se si inserisce un modulo personalizzato in un modello di progetto, questo verrà assegnato automaticamente quando il modello viene selezionato nel processo di conversione.

<!-- Learn more graphic and documentation article links 

* Convert issues
* Transfer custom form data to a larger work item
* Overview of resolving and resolvable objects
* Understanding resolving and resolvable objects
* Unlink issues from their resolvable objects

-->

## Convertire un problema in un&#39;attività o un progetto da qualsiasi elenco di problemi

Per aumentare l&#39;efficienza del lavoro e semplificare la conversione dei problemi in un ambiente veloce, puoi convertire un problema in un&#39;attività o in un progetto da qualsiasi elenco di problemi in un progetto, report o dashboard. Seleziona un problema e fai clic sul menu a 3 punti visualizzato.

![Immagine di una schermata di un progetto che mostra le opzioni di conversione dei problemi](assets/convert-from-a-list.png)

