---
title: Creare un rapporto attività
description: Questo video illustra come creare un rapporto attività con un filtro complesso e individuare i rapporti creati in [!DNL  Workfront].
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335154.png
kt: 8859
exl-id: 90bad2e8-9cd2-4ae7-973b-eeab9d615bef
source-git-commit: f4000878d453c58fabf34308a8e3ab31d9667a1f
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 5%

---

# Creare un rapporto attività

In questo video imparerai:

* Come creare un rapporto attività con un filtro complesso
* Come trovare i rapporti creati

>[!VIDEO](https://video.tv.adobe.com/v/335154/?quality=12)

## Attività: Creare un rapporto di nota con prompt

Crea un rapporto di nota che puoi utilizzare per cercare le note utente (ad esempio, commenti o aggiornamenti) o le note di sistema in base al contenuto della nota, all’autore, alla data di ingresso, al nome del progetto o al tipo di controllo. Denomina il report &quot;Ricerca note&quot;.

Quando si utilizza il prompt Testo nota , questo rapporto eseguirà una ricerca all’interno dei thread di aggiornamento per estrarre rapidamente tutti i criteri che soddisfano i criteri specificati nei prompt. Quando esegui il rapporto, non devi compilare tutti i prompt, solo quelli che ti interessano. Quelli vuoti vengono automaticamente ignorati.

La visualizzazione deve includere colonne per:

* Testo della Nota
* Testo di controllo
* Data inserimento
* Proprietario: Nome
* Tipo di Revisione
* Nome attività
* Nome Issue

Lascia vuota la scheda del filtro.

Raggruppa in nome progetto.

Includi prompt per i seguenti elementi:

* Testo di controllo
* Testo della Nota
* Nome proprietario
* Data inserimento
* Nome progetto
* Tipo di Revisione

## Risposta

1. Seleziona **[!UICONTROL Rapporti]** dal **[!UICONTROL Menu principale]**.
1. Fai clic sul pulsante **[!UICONTROL Nuovo rapporto]** menu e seleziona **[!UICONTROL Nota]**.
1. In **[!UICONTROL Colonne (visualizzazione)]** imposta le colonne in modo da includere:

   ![Immagine della schermata per creare colonne di report note](assets/note-report-columns.png)

   * [!UICONTROL Nota] > [!UICONTROL Testo nota]
   * [!UICONTROL Nota] > [!UICONTROL Testo di controllo]
   * [!UICONTROL Nota] > [!UICONTROL Data di ingresso]
   * [!UICONTROL Proprietario] > [!UICONTROL Nome]
   * [!UICONTROL Nota] > [!UICONTROL Tipo di audit]
   * [!UICONTROL Attività] > [!UICONTROL Nome]
   * [!UICONTROL Problema] > [!UICONTROL Nome]

1. Seleziona la **[!UICONTROL Data di ingresso]** e modifica la **[!UICONTROL Ordina per decrescente]**.
1. In **[!UICONTROL Raggruppamenti]** imposta il rapporto su raggruppa per [!UICONTROL Progetto] > [!UICONTROL Nome].

   ![Immagine della schermata per creare raggruppamenti di rapporti per note](assets/note-report-groupings.png)

1. Esci [!UICONTROL Filtri] vuoto.
1. Apri **[!UICONTROL Impostazioni dei rapporti]** e denomina il rapporto &quot;Ricerca note&quot;.
1. In [!UICONTROL Descrizione] Inserisci un esempio di tipo &quot;Cerca note di sistema o utente in base al tipo di controllo selezionato e ad altri prompt. Le note di sistema vengono visualizzate nella colonna Testo di controllo e le note utente vengono visualizzate nella colonna Testo nota .&quot;

   ![Immagine della schermata per creare le impostazioni dei rapporti sulle note](assets/note-report-report-options.png)

1. Seleziona **[!UICONTROL Scheda Dettagli]** in modo che venga visualizzato quando il report viene caricato.
1. Imposta il rapporto in modo da visualizzare 200 elementi quando il rapporto viene incluso in un dashboard.
1. Fai clic su **[!UICONTROL Richieste di rapporto]** e aggiungi:

   ![Immagine della schermata per creare i prompt dei report di note](assets/note-report-report-prompts.png)

   * [!UICONTROL Nota] > [!UICONTROL Testo di controllo]
   * [!UICONTROL Nota] > [!UICONTROL Testo nota]
   * [!UICONTROL Proprietario] > [!UICONTROL Nome]
   * [!UICONTROL Nota] > [!UICONTROL Data di ingresso]
   * [!UICONTROL Progetto] > [!UICONTROL Nome]
   * [!UICONTROL Nota] > [!UICONTROL Tipo di audit]

1. Seleziona la casella per **[!UICONTROL Mostra prompt nelle dashboard]**.
1. Salva e chiudi il rapporto.
