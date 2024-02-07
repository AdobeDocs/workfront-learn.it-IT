---
title: Creare un rapporto di attività
description: 'Scopri come creare un rapporto di attività con un filtro complesso e individuare i rapporti creati in Workfront. Attività: crea un rapporto di nota con indicazioni.'
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335154.png
jira: KT-8859
exl-id: 90bad2e8-9cd2-4ae7-973b-eeab9d615bef
doc-type: video
source-git-commit: 5fa3bbf2fb4763e63beeb7ac640cc93ccf54fed5
workflow-type: tm+mt
source-wordcount: '922'
ht-degree: 40%

---

# Creare un rapporto di attività

In questo video scoprirai:

* Come creare un rapporto di attività con un filtro complesso
* Come trovare i rapporti creati

>[!VIDEO](https://video.tv.adobe.com/v/335154/?quality=12&learn=on)



>[!TIP]
>
>Scoprite le vostre spatole e ciotole per miscelare e preparatevi a provare le &quot;ricette&quot; nel nostro [Manuale di Adobe Workfront per la generazione di rapporti sui clienti](/help/assets/workfront-customer-reporting-cookbook.pdf). All’interno troverai istruzioni dettagliate per 10 rapporti, pronti per essere inseriti nel tuo ambiente attuale.
>Abbiamo raccolto i report preferiti dei clienti e li abbiamo inseriti in un manuale facilmente digeribile e facilmente riconoscibile, da riportare e testare nella vostra cucina Workfront.
>Questi 10 rapporti provengono da clienti che sono proprio come te. Distribuiti in vari settori, reparti, team, posizioni e tutti in diverse aziende, dobbiamo un enorme grazie ai incredibili clienti che hanno condiviso uno dei loro report preferiti. Alcuni rapporti sono semplici (ma incredibilmente utili), mentre altri sono più complessi e possono portare i rapporti a un livello successivo.



## Attività 1: creare un rapporto nota con prompt

Crea un rapporti sulle note che è possibile utilizzare per cercare note utente (ad esempio, commenti o aggiornamenti) o note di sistema in base al contenuto della nota, all’autore, alla data di immissione, al nome del progetto o al tipo di audit. Denomina il rapporto &quot;Ricerca nota&quot;.

Quando si utilizza il prompt Testo nota, questo rapporto esegue la ricerca all’interno dei thread di aggiornamento per estrarre rapidamente quelli che soddisfano i criteri specificati nei prompt. Quando esegui il rapporto, non è necessario compilare ogni prompt, solo quelli a cui tieni. I vuoti vengono automaticamente ignorati.

La visualizzazione deve includere colonne per:

* Testo della Nota
* Testo di controllo
* Data inserimento
* Nome del proprietario
* Tipo di Revisione
* Nome attività
* Nome Issue

Lascia vuota la scheda del filtro.

Raggruppa per nome progetto.

Includi richieste per:

* Testo di controllo
* Testo della Nota
* Nome del proprietario
* Data inserimento
* Nome progetto
* Tipo di Revisione

## Risposta per l’attività 1

1. Seleziona **[!UICONTROL Rapporti]** dal **[!UICONTROL Menu principale]**.
1. Fai clic sul menu **[!UICONTROL Nuovo rapporto]** e seleziona **[!UICONTROL Nota]**.
1. Nella sezione **[!UICONTROL Colonne (visualizzazione)]** imposta le colonne in modo che includano:

   ![Immagine della schermata per la creazione di colonne di rapporti sulle note](assets/note-report-columns.png)

   * [!UICONTROL Nota] > [!UICONTROL Testo nota]
   * [!UICONTROL Nota] > [!UICONTROL Testo di audit]
   * [!UICONTROL Nota] > [!UICONTROL Data di immissione]
   * [!UICONTROL Proprietario] > [!UICONTROL Nome]
   * [!UICONTROL Nota] > [!UICONTROL Tipo di audit]
   * [!UICONTROL Attività] > [!UICONTROL Nome]
   * [!UICONTROL Problema] > [!UICONTROL Nome]

1. Seleziona la colonna **[!UICONTROL Data di immissione]** e modifica l’**[!UICONTROL Ordine decrescente]**.
1. Nella scheda **[!UICONTROL Raggruppamenti]**, imposta il rapporto in base al quale eseguire il raggruppamento [!UICONTROL Progetto] > [!UICONTROL Nome].

   ![Immagine della schermata per creare raggruppamenti di rapporti sulle note](assets/note-report-groupings.png)

1. Lascia vuoto il campo [!UICONTROL Filtri].
1. Apri **[!UICONTROL Impostazioni dei rapporti]** e denomina il rapporto &quot;Ricerca nota&quot;.
1. In [!UICONTROL Descrizione] , inserisci qualcosa come, &quot;Cerca le note sul sistema o sull’utente in base al Tipo di controllo selezionato e ad altri prompt. Le note di sistema vengono visualizzate nella colonna Testo di audit e le note utente nella colonna Testo nota.&quot;

   ![Immagine della schermata per la creazione delle impostazioni per i rapporti sulle note](assets/note-report-report-options.png)

1. Seleziona la **[!UICONTROL Scheda dettagli]** in modo che venga visualizzato il caricamento del rapporto.
1. Imposta il rapporto in modo che mostri 200 elementi quando viene incluso in una dashboard.
1. Fai clic su **[!UICONTROL Prompt dei rapporti]** e aggiungi:

   ![immagine della schermata per la creazione di prompt di rapporti sulle note](assets/note-report-report-prompts.png)

   * [!UICONTROL Nota] > [!UICONTROL Testo di audit]
   * [!UICONTROL Nota] > [!UICONTROL Testo nota]
   * [!UICONTROL Proprietario] > [!UICONTROL Nome]
   * [!UICONTROL Nota] > [!UICONTROL Data immissione]
   * [!UICONTROL Progetto] > [!UICONTROL Nome]
   * [!UICONTROL Nota] > [!UICONTROL Tipo di audit]

1. Seleziona la casella per **[!UICONTROL Mostra i prompt nelle dashboard]**.
1. Salva e chiudi il rapporto.

## Attività 2: creare un rapporto sui feedback del team di amministrazione

Questo è un report di problemi che visualizza tutti i problemi di una coda di richieste di feedback creata per gli amministratori di sistema. Puoi vedere come creare questa coda di richieste nella [Creare una coda di richieste di feedback dell’amministratore di sistema](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/manage-work/request-queues/create-a-system-admin-feedback-request-queue.html) esercitazione.

Questo report utilizza anche un modulo personalizzato. Per informazioni su come creare un modulo personalizzato, vedi [Creare e condividere un modulo personalizzato](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/custom-data/custom-forms/custom-forms-creating-and-sharing-a-custom-form.html) esercitazione.

Il modulo personalizzato deve essere creato come segue:

Nome: feedback del processo di amministrazione

1. Tipo di processo (campo a discesa)
   * livelli di accesso
   * processo di approvazione (solo globale)
   * notifiche e-mail
   * modello di layout
   * percorso milestone
   * modello di progetto
   * notifiche promemoria
   * coda richieste
1. Nome processo (campo di testo a riga singola)
1. Livello processo (campo a discesa)
   * 1 - totalmente inutile
   * 2 - non molto utile
   * 3 - bene ma potrebbe essere meglio
   * 4 - eccellente
1. Problema o buone notizie (campo di testo paragrafo)

Creare un rapporto sui problemi denominato **Rapporto feedback del team di amministrazione**.

La vista deve avere le seguenti colonne:

* Problema: nome
* Contatto principale: nome
* Problema: tipo di processo
* Problema: nome del processo
* Problema: livello processo
* Problema: problema o buone notizie
* Problema: data di ingresso
* Problema: Età
* Problema: assegnazioni
* Problema: stato

Raggruppa in base al tipo di processo.

Puoi filtrare in base all’ID del progetto della coda richieste in cui si trovano i problemi di feedback.


![Schermata del rapporto di feedback del team di amministrazione](assets/create-a-system-admin-feedback-request-queue.png)



## Attività 2 Risposta

1. Seleziona **[!UICONTROL Rapporti]** dal **[!UICONTROL Menu principale]**.
1. Fai clic su **[!UICONTROL Nuovo rapporto]** menu e seleziona **[!UICONTROL Problema]**.
1. Nella sezione **[!UICONTROL Colonne (visualizzazione)]** imposta le colonne in modo che includano:

   ![Immagine della schermata per creare le colonne del report sui problemi](assets/task-report-activity-2-1.png)

   * [!UICONTROL Problema] > [!UICONTROL Nome]
   * [!UICONTROL Contatto principale] > [!UICONTROL Nome]
      * Nota: viene visualizzato con &quot;Proprietario:Nome&quot; come etichetta di colonna. Per cambiare questa impostazione in &quot;Riportato da&quot;, fai clic su Opzioni avanzate e digita &quot;Riportato da&quot; nel **Etichetta colonna personalizzata** campo.
   * [!UICONTROL Problema] > [!UICONTROL Tipo di processo]
   * [!UICONTROL Problema] > [!UICONTROL Nome processo]
   * [!UICONTROL Problema] > [!UICONTROL Livello processo]
   * [!UICONTROL Problema] > [!UICONTROL Problema o buone notizie]
   * [!UICONTROL Problema] > [!UICONTROL Data di ingresso]
   * [!UICONTROL Problema] > [!UICONTROL Età]
   * [!UICONTROL Problema] > [!UICONTROL Assegnazioni]
   * [!UICONTROL Problema] > [!UICONTROL Stato]

1. Seleziona la colonna **[!UICONTROL Data di immissione]** e modifica l’**[!UICONTROL Ordine decrescente]**.
1. In **[!UICONTROL Raggruppamenti]** , impostare il report in base al quale eseguire il raggruppamento **[!UICONTROL Problema] > [!UICONTROL Tipo di processo]**.

   ![Immagine della schermata per creare i raggruppamenti dei report sui problemi](assets/task-report-activity-2-2.png)

1. In **[!UICONTROL Filtri]** , aggiungi un filtro per la scheda **[!UICONTROL Problema] > [!UICONTROL ID Progetto]** per eguagliare il progetto della coda richieste in cui risiedono i problemi di feedback.

   ![Immagine della schermata per creare i filtri per la segnalazione dei problemi](assets/task-report-activity-2-3.png)

1. Salva e chiudi il rapporto.
