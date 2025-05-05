---
title: Comprendere i dettagli della bozza
description: Approfondisci i dettagli di una bozza in  [!DNL &#x200B; Workfront]  tramite il pannello di riepilogo e la pagina [!UICONTROL Dettagli documento].
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Beginner
thumbnail: understand-proof-details.png
jira: KT-10110
exl-id: 196f9318-eced-4825-b0fd-8592b6cb3403
source-git-commit: cb72c429f0ef4cd9945282876aa49189dab1bd96
workflow-type: tm+mt
source-wordcount: '1038'
ht-degree: 57%

---

# Comprendere i dettagli della bozza

## Visualizzare i dettagli della bozza

In qualità di manager o proprietario di una bozza, puoi approfondirne i dettagli attraverso il pannello di riepilogo e la pagina [!UICONTROL Dettagli documento]. Per prima cosa, cerca la bozza nella sezione [!UICONTROL Documenti] di un progetto, attività o problema.

### Pannello di Riepilogo

Seleziona una bozza dall’elenco dei documenti, quindi fai clic sull’icona Riepilogo in alto a destra dello schermo.

![Immagine della sezione [!UICONTROL Documenti] di un progetto con una bozza selezionata.](assets/document-summary-1.png)

Fai clic su Panoramica per espandere la sezione panoramica.

![Immagine della sezione [!UICONTROL Documenti] di un progetto con una bozza selezionata e il pannello di riepilogo espanso. Vengono evidenziate sia l’icona che il pannello di riepilogo.](assets/document-summary-2.png)

Quindi scorri verso il basso fino alla sezione Bozza. Qui puoi vedere il proprietario della bozza, l’avanzamento, il numero di commenti, lo stato e la data di scadenza.

![Immagine della sezione [!UICONTROL Documenti] di un progetto con una bozza selezionata e il pannello di riepilogo espanso. Vengono evidenziate sia l’icona che il pannello di riepilogo.](assets/document-summary-3.png)

Nota: la sezione [!UICONTROL Approvazioni] nel pannello di riepilogo è per le approvazioni **document** e **non è** associata al processo di revisione e approvazione della bozza. In [!DNL Workfront], i due processi sono distinti.

### [!UICONTROL Dettagli Documento]

Per ulteriori informazioni sulla bozza, fare clic su [!UICONTROL Dettagli documento].

![Immagine della sezione [!UICONTROL Documenti] di un progetto con una bozza selezionata e [!UICONTROL Dettagli documento] evidenziati.](assets/document-summary-4.png)

Viene visualizzata la pagina [!UICONTROL Dettagli documento] e diverse opzioni aggiuntive nel pannello a sinistra.

![Immagine della pagina della bozza in [!DNL &#x200B; Workfront].](assets/document-details.png)

È importante notare che la possibilità di visualizzare informazioni relative al processo di verifica dipende dalle autorizzazioni di verifica in [!DNL Workfront].

Dalla pagina della bozza, puoi accedere alle sezioni seguenti dal menu del pannello a sinistra:

* **Aggiornamenti —** I commenti aggiunti nel visualizzatore bozze vengono visualizzati qui, con il tag &quot;proof comment&quot; (commento bozza). È inoltre possibile aggiungere commenti al file, proprio come si fa per un’attività o un progetto (questi commenti non vengono visualizzati nel Proofing Viewer).
* **Approvazioni:** questa sezione riguarda le approvazioni dei documenti, non le approvazioni della bozza. I due tipi di approvazioni sono processi separati in [!DNL Workfront] e non sono collegati. Se utilizzi flussi di lavoro di bozza per le revisioni e le approvazioni, non utilizzerai questa sezione.
* **Tutte le versioni:** per tenere traccia e gestirei la cronologia delle versioni della bozza. Per accedere più facilmente a queste informazioni, consulta il pannello di riepilogo nell’elenco [!UICONTROL Documenti].
* **Moduli personalizzati:** i moduli personalizzati vengono utilizzati sulle bozze per acquisire informazioni specifiche dell’organizzazione. Queste informazioni possono essere trasmesse con il file ai sistemi di archiviazione dei documenti integrati, ad esempio [!DNL Workfront] DAM o Adobe Experience Manager. I moduli personalizzati sono impostati dal tuo amministratore di sistema o amministratore di gruppo di [!DNL Workfront]. Parla con il tuo team o con gli amministratori per sapere se utilizzerai moduli personalizzati sulle bozze.
* **Flusso di lavoro di bozza:** per gestire o modificare il flusso di lavoro assegnato alla bozza. Puoi aprire questa finestra utilizzando il collegamento [!UICONTROL Flusso di lavoro bozza] nella bozza dell&#39;elenco [!UICONTROL Documenti].

Esaminiamo più da vicino due sezioni: [!UICONTROL Impostazioni visualizzatore bozze] e [!UICONTROL Attività bozza].

### [!UICONTROL Impostazioni visualizzatore bozza]

Queste impostazioni consentono di controllare l’accesso alla bozza stessa.

![Immagine delle [!UICONTROL Impostazioni Proofing Viewer] dalla pagina della bozza con l’opzione [!UICONTROL Impostazioni Proofing Viewer] evidenziata nel menu del pannello a sinistra.](assets/proofing-settings-on-details-page.png)

* **[!UICONTROL Accesso obbligatorio. Questa bozza non può essere condivisa con utenti guest].** La bozza può essere condivisa solo con persone che hanno una licenza per le bozze di [!DNL Workfront].
* **[!UICONTROL Richiede che le decisioni siano firmate elettronicamente] —** Quando si condivide una bozza, è necessario che il destinatario disponga delle autorizzazioni di verifica in [!DNL Workfront] e che &quot;firmi elettronicamente&quot; la bozza immettendo la password di verifica quando prende una decisione in merito alla bozza. (Nota: la password per la bozza è diversa dalla tua password di [!DNL Workfront]. La password di verifica non è facilmente accessibile, pertanto la maggior parte dei destinatari non la conosce.) Adobe consiglia di contattare il consulente [!DNL Workfront] prima di utilizzare questa funzione.
* **[!UICONTROL Blocca la bozza quando vengono prese tutte le decisioni necessarie]:** questa opzione blocca la bozza per qualsiasi ulteriore commento, risposta, decisione, ecc., una volta che le decisioni sono state prese. Questa opzione blocca l’intera versione della bozza, non solo una fase specifica del flusso di lavoro.
* **[!UICONTROL Consenti il download del file originale] —** I destinatari della bozza possono scaricare il file di origine originale della bozza dal visualizzatore di bozze.
* **[!UICONTROL Consenti condivisione bozze tramite URL pubblico o codice di incorporamento]:** i destinatari della bozza possono condividere con chiunque un collegamento alla bozza accessibile al pubblico.
* **[!UICONTROL Consenti la sottoscrizione alla bozza tramite URL pubblico o codice di incorporamento]:** chiunque riceve l’URL pubblico può aggiungersi alla bozza con il proprio indirizzo e-mail e nome (se non è un utente della bozza) o il proprio indirizzo e-mail e password della bozza (se è un utente della bozza). (Nota: la password della bozza non uguale a una password di [!DNL Workfront].)


### [!UICONTROL Attività bozza]

Questa pagina tiene traccia di tutte le attività che si sono verificate sulla bozza, oltre ai messaggi e-mail inviati relativi alla bozza.

![Immagine della sezione [!UICONTROL Attività bozza] nella pagina della stessa con l’opzione [!UICONTROL Attività bozza] evidenziata nel menu del pannello a sinistra.](assets/proofing-activity-in-details.png)

Timestamp della sezione **[!UICONTROL Attività]** in cui sono presenti i commenti e le decisioni effettuati, oltre a chi li ha realizzati. Inoltre, tiene traccia dell’inizio delle fasi relative al flusso di lavoro di bozza, quando un destinatario ha aperto per la prima volta una bozza e altre informazioni utili per un responsabile o proprietario di bozza. Questi dettagli possono essere utili quando si cerca di capire cose come, perché una fase del flusso di lavoro di bozza non è mai iniziata, ad esempio.

Timestamp della sezione **[!UICONTROL Messaggi]** in cui sono presenti avvisi e messaggi e-mail inviati ai destinatari, i mittenti e il contenuto del messaggio. Questo può essere utile durante la risoluzione dei problemi se qualcuno dice di non aver ricevuto un’e-mail relativa a una bozza. Puoi verificare se e quando è stato inviato un messaggio e-mail.

Adobe consiglia al gestore delle bozze e al proprietario della bozza di acquisire familiarità con le informazioni contenute in queste due sezioni. La combinazione di queste informazioni con le istruzioni su come leggere la barra di avanzamento [!UICONTROL SOCD], ti consente di comprendere e gestire le bozze in modo efficace, indipendentemente dalla posizione che occupano all’interno del flusso di lavoro di bozza.

Dopo aver terminato di lavorare nella sezione [!UICONTROL Dettagli documento], utilizza la traccia delle breadcrumb per tornare alla sezione [!UICONTROL Documenti] del progetto, dell&#39;attività o del problema a cui è allegata la bozza.

![Immagine del percorso breadcrumb nell’intestazione.](assets/proof-breadcrumb.png)

<!--
#### Learn more
* [!UICONTROL Document details] overview
* Add a custom form to a document
* Request document approvals
* Summary for documents overview
* View activity on a proof within [!DNL Workfront]
-->
