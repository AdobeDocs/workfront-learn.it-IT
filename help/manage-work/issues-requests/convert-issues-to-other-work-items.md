---
title: Convertire un problema/richiesta in un’attività
description: Scopri come convertire i problemi in altri elementi di lavoro .
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: convert-issues-to-other-work-items.jpeg
type: Tutorial
role: User
level: Intermediate
jira: KT-10069
exl-id: 1fd4d862-e44b-4c50-9663-70e727f6e9b7
source-git-commit: 060ceb14d274e8b2ad080c1f58290a2c5769e007
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# Convertire un problema/richiesta in un’attività

Un problema può essere abbastanza significativo da richiedere che il tempo e lo sforzo necessari per risolverlo siano contabilizzati nella tempistica del progetto e che vengano assegnate le risorse appropriate. In questo caso, il problema può essere convertito in un’attività.

![Un&#39;immagine del [!UICONTROL Converti in attività] opzione di un problema in [!UICONTROL Workfront].](assets/15-convert-issue-to-task-menu-option.png)

1. Accedi a [!UICONTROL Problemi] sezione del progetto o dell’attività a cui è connesso il problema. In alternativa, puoi individuare il problema in un rapporto a cui hai accesso.
1. Fai clic sul nome del problema per aprirlo.
1. Dal menu a 3 punti a destra del nome del problema, seleziona **[!UICONTROL Converti in attività]**.
1. Compila il [!UICONTROL Converti in attività] modulo. Per iniziare, assegnare un nome e una descrizione alla nuova attività.
1. Se la nuova attività deve far parte di un progetto diverso, modificare la [!UICONTROL Progetto di destinazione] nome.
1. In [!UICONTROL Opzioni] , seleziona le caselle per mantenere il problema originale, consentire l’accesso alla nuova attività e mantenere la data di completamento. Segui il flusso di lavoro della tua organizzazione quando effettui queste selezioni.
1. Allega un modulo personalizzato se desideri trasferire i dati del modulo personalizzato dal problema all’attività. (Tutti i campi presenti sia nel modulo del problema che nel modulo delle attività verranno trasferiti automaticamente al modulo delle attività.)
1. Clic **[!UICONTROL Converti in attività]** per terminare.

![Un&#39;immagine del [!UICONTROL Converti in attività] forma di un problema in [!UICONTROL Workfront].](assets/16-convert-to-task-options.png)

A seconda dell’ [!DNL Workfront] impostazioni di sistema, è possibile modificare le impostazioni nella sezione Opzioni durante la conversione dell&#39;attività. Queste opzioni hanno effetto sia sul problema originale che sulla nuova attività.

* **Mantieni il problema originale e collegane la risoluzione a questa attività** mantiene il problema originale e le relative informazioni (ore, documenti, ecc.). Quando questa opzione è selezionata, al termine dell’attività il problema verrà contrassegnato come risolto. Se questa opzione è **non** Selezionando questa opzione, il problema originale verrà eliminato durante la creazione dell’attività. Questo può influenzare il modo in cui la tua organizzazione tiene traccia e segnala i problemi.
* Il **Consenti a (nome utente) di accedere a questa attività** consente alla persona che ha creato il problema di accedere a questa nuova attività.
* Il **Mantieni la data di completamento pianificata del problema** consente di mantenere la data di completamento pianificata già impostata sul problema. In questo modo il vincolo attività viene impostato su [!UICONTROL Finire non Dopo di]. Se la casella è deselezionata, le date dell&#39;attività verranno impostate come se fosse stata creata una nuova attività all&#39;interno del progetto.

La nuova attività viene posizionata in fondo all&#39;elenco delle attività del progetto. Spostare l&#39;attività nella posizione desiderata, assegnare un utente o un team al lavoro, aggiungere ore e durata pianificate e così via.

>[!NOTE]
>
>Non è possibile aggiungere problemi alla sequenza temporale del progetto, poiché rappresentano &quot;lavoro non pianificato&quot;. La timeline del progetto è per &quot;lavoro pianificato&quot;, ovvero attività.


