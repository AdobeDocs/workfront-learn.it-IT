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
kt: 8859
exl-id: 90bad2e8-9cd2-4ae7-973b-eeab9d615bef
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 11%

---

# Creare un rapporto di attività

Questo video illustra:

* Come creare un rapporto di attività con un filtro complesso
* Come trovare i rapporti creati

>[!VIDEO](https://video.tv.adobe.com/v/335154/?quality=12)

## Attività: crea un rapporto di nota con le richieste

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

## Risposta

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
