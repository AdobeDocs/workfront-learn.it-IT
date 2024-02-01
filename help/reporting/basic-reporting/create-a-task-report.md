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
source-git-commit: 8cd01b3dca3a62c1d8699d7d076dccddf2010907
workflow-type: tm+mt
source-wordcount: '794'
ht-degree: 6%

---

# Creare un rapporto di attività

Questo video illustra:

* Come creare un rapporto di attività con un filtro complesso
* Come trovare i rapporti creati

>[!VIDEO](https://video.tv.adobe.com/v/335154/?quality=12&learn=on)

## Attività 1: creare un rapporto nota con prompt

Creare un report di note che è possibile utilizzare per cercare note utente (ad esempio, commenti o aggiornamenti) o note di sistema in base al contenuto della nota, all&#39;autore, alla data di immissione, al nome del progetto o al tipo di controllo. Denomina il rapporto &quot;Ricerca nota&quot;.

Quando si utilizza il prompt Testo nota, questo report esegue la ricerca all&#39;interno dei thread di aggiornamento per estrarre rapidamente quelli che soddisfano i criteri specificati nei prompt. Quando esegui il rapporto, non è necessario compilare ogni prompt, solo quelli a cui tieni. I vuoti vengono automaticamente ignorati.

La visualizzazione deve includere colonne per:

* Testo della Nota
* Testo di controllo
* Data inserimento
* Proprietario: Name
* Tipo di Revisione
* Nome attività
* Nome Issue

Lascia vuota la scheda del filtro.

Raggruppa per nome progetto.

Includi richieste per:

* Testo di controllo
* Testo della Nota
* Nome proprietario
* Data inserimento
* Nome progetto
* Tipo di Revisione

## Risposta attività 1

1. Seleziona **[!UICONTROL Rapporti]** dal **[!UICONTROL Menu principale]**.
1. Fai clic su **[!UICONTROL Nuovo rapporto]** menu e seleziona **[!UICONTROL Nota]**.
1. In entrata **[!UICONTROL Colonne (visualizzazione)]** imposta le colonne in modo che includano:

   ![Immagine della schermata per la creazione di colonne di report note](assets/note-report-columns.png)

   * [!UICONTROL Nota] > [!UICONTROL Testo nota]
   * [!UICONTROL Nota] > [!UICONTROL Testo di controllo]
   * [!UICONTROL Nota] > [!UICONTROL Data immissione]
   * [!UICONTROL Proprietario] > [!UICONTROL Nome]
   * [!UICONTROL Nota] > [!UICONTROL Tipo di controllo]
   * [!UICONTROL Attività] > [!UICONTROL Nome]
   * [!UICONTROL Problema] > [!UICONTROL Nome]

1. Seleziona la **[!UICONTROL Data immissione]** e modificare la **[!UICONTROL Ordine decrescente]**.
1. In **[!UICONTROL Raggruppamenti]** , impostare il report in base al quale eseguire il raggruppamento [!UICONTROL Progetto] > [!UICONTROL Nome].

   ![Immagine della schermata per creare raggruppamenti di report note](assets/note-report-groupings.png)

1. Esci [!UICONTROL Filtri] vuoto.
1. Apri **[!UICONTROL Impostazioni dei rapporti]** e denomina il rapporto &quot;Ricerca nota&quot;.
1. In [!UICONTROL Descrizione] , inserisci qualcosa come, &quot;Cerca le note sul sistema o sull’utente in base al Tipo di controllo selezionato e ad altri prompt. Le note di sistema vengono visualizzate nella colonna Testo di audit e le note utente nella colonna Testo nota.&quot;

   ![Immagine della schermata per la creazione delle impostazioni per i rapporti sulle note](assets/note-report-report-options.png)

1. Seleziona **[!UICONTROL Scheda Dettagli]** in modo che venga visualizzato quando viene caricato il rapporto.
1. Imposta il rapporto in modo che mostri 200 elementi quando il rapporto viene incluso in un dashboard.
1. Clic **[!UICONTROL Prompt dei report]** e aggiungi:

   ![Immagine della schermata per la creazione di richieste di report note](assets/note-report-report-prompts.png)

   * [!UICONTROL Nota] > [!UICONTROL Testo di controllo]
   * [!UICONTROL Nota] > [!UICONTROL Testo nota]
   * [!UICONTROL Proprietario] > [!UICONTROL Nome]
   * [!UICONTROL Nota] > [!UICONTROL Data immissione]
   * [!UICONTROL Progetto] > [!UICONTROL Nome]
   * [!UICONTROL Nota] > [!UICONTROL Tipo di controllo]

1. Seleziona la casella per **[!UICONTROL Mostra i prompt nei dashboard]**.
1. Salva e chiudi il report.

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



## Risposta attività 2

1. Seleziona **[!UICONTROL Rapporti]** dal **[!UICONTROL Menu principale]**.
1. Fai clic su **[!UICONTROL Nuovo rapporto]** menu e seleziona **[!UICONTROL Problema]**.
1. In entrata **[!UICONTROL Colonne (visualizzazione)]** imposta le colonne in modo che includano:

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

1. Seleziona la **[!UICONTROL Data immissione]** e modificare la **[!UICONTROL Ordine decrescente]**.
1. In **[!UICONTROL Raggruppamenti]** , impostare il report in base al quale eseguire il raggruppamento **[!UICONTROL Problema] > [!UICONTROL Tipo di processo]**.

   ![Immagine della schermata per creare i raggruppamenti dei report sui problemi](assets/task-report-activity-2-2.png)

1. In **[!UICONTROL Filtri]** , aggiungi un filtro per la scheda **[!UICONTROL Problema] > [!UICONTROL ID Progetto]** per eguagliare il progetto della coda richieste in cui risiedono i problemi di feedback.

   ![Immagine della schermata per creare i filtri per la segnalazione dei problemi](assets/task-report-activity-2-3.png)

1. Salva e chiudi il report.
