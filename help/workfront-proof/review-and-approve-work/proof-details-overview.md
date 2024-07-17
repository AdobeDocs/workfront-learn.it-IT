---
title: Comprendere i dettagli della bozza
description: Approfondisci i dettagli di una bozza in  [!DNL  Workfront]  tramite il pannello di riepilogo e la pagina [!UICONTROL Dettagli documento].
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Beginner
thumbnail: understand-proof-details.png
jira: KT-10110
exl-id: 196f9318-eced-4825-b0fd-8592b6cb3403
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '1029'
ht-degree: 100%

---

# Comprendere i dettagli della bozza

## Visualizzare i dettagli della bozza

In qualità di manager o proprietario di una bozza, puoi approfondirne i dettagli attraverso il pannello di riepilogo e la pagina [!UICONTROL Dettagli documento]. Per prima cosa, cerca la bozza nella sezione [!UICONTROL Documenti] di un progetto, attività o problema.

### Pannello di Riepilogo

Il pannello di riepilogo fornisce una panoramica di alto livello dei dettagli di base della bozza. Utilizza l’icona per espandere il pannello quando necessario e comprimerlo quando non lo desideri. Puoi anche passare il cursore sulla miniatura della bozza per aprirla o scaricarla.

![Immagine della sezione [!UICONTROL Documenti] di un progetto con una bozza selezionata e il pannello di riepilogo espanso. Vengono evidenziate sia l’icona che il pannello di riepilogo.](assets/document-summary.png)

Nota: la sezione [!UICONTROL Approvazioni] nel pannello di riepilogo è per le approvazioni del **documento** e **non è** legata al processo di revisione e approvazione delle bozze che stai imparando in questo corso. In [!DNL Workfront], i due processi sono distinti.

### [!UICONTROL Dettagli Documento]

Per ulteriori informazioni sulla bozza, consulta il link [!UICONTROL Dettagli documento] per accedere alla “pagina“ della bozza in [!DNL Workfront].

![Immagine della pagina della bozza in [!DNL  Workfront].](assets/document-details.png)

È importante tenere presente che la possibilità di visualizzare informazioni relative al processo relativo alla bozza dipende dalle autorizzazioni della bozza in [!DNL Workfront].

Dalla pagina della bozza, puoi accedere alle sezioni seguenti dal menu del pannello a sinistra:

* **Aggiornamenti:** i commenti fatti nel Proofing Viewer vengono visualizzati qui, con un tag “commento bozza“. È inoltre possibile aggiungere commenti al file, proprio come si fa per un’attività o un progetto (questi commenti non vengono visualizzati nel Proofing Viewer).
* **Approvazioni:** questa sezione riguarda le approvazioni dei documenti, non le approvazioni della bozza. I due tipi di approvazioni sono processi separati in [!DNL Workfront] e non sono collegati. Se utilizzi flussi di lavoro di bozza per le revisioni e le approvazioni, non utilizzerai questa sezione.
* **Tutte le versioni:** per tenere traccia e gestirei la cronologia delle versioni della bozza. Per accedere più facilmente a queste informazioni, consulta il pannello di riepilogo nell’elenco [!UICONTROL Documenti].
* **Moduli personalizzati:** i moduli personalizzati vengono utilizzati sulle bozze per acquisire informazioni specifiche dell’organizzazione. Queste informazioni possono essere trasferite insieme al file a sistemi di archiviazione documenti integrati, come [!DNL Workfront]DAM o [!DNL Adobe’s]AEM. I moduli personalizzati sono impostati dal tuo amministratore di sistema o amministratore di gruppo di [!DNL Workfront]. Parla con il tuo team o con gli amministratori per sapere se utilizzerai moduli personalizzati sulle bozze.
* **Flusso di lavoro di bozza:** per gestire o modificare il flusso di lavoro assegnato alla bozza. È possibile aprire questa finestra anche utilizzando il link [!UICONTROL Flusso di lavoro di bozza] sulla bozza nell’elenco [!UICONTROL Documenti]. Scopri come apportare modifiche al flusso di lavoro con il video Modificare un flusso di lavoro di bozza.

Esaminiamo più da vicino due sezioni: [!UICONTROL Impostazioni Proofing Viewer] e [!UICONTROL Attività bozza].

### [!UICONTROL Impostazioni visualizzatore bozza]

Queste impostazioni consentono di controllare l’accesso alla bozza stessa.

![Immagine delle [!UICONTROL Impostazioni Proofing Viewer] dalla pagina della bozza con l’opzione [!UICONTROL Impostazioni Proofing Viewer] evidenziata nel menu del pannello a sinistra.](assets/proofing-settings-on-details-page.png)

* **[!UICONTROL Accesso obbligatorio. Questa bozza non può essere condivisa con utenti guest].** La bozza può essere condivisa solo con persone che hanno una licenza per le bozze di [!DNL Workfront].
* **[!UICONTROL Richiedi che le decisioni siano firmate elettronicamente]:** quando si condivide una bozza, è necessario che il destinatario disponga delle autorizzazioni per la bozza in [!DNL Workfront] e consente di &quot;firmare elettronicamente&quot; la bozza inserendo la relativa password quando prendono una Decisione bozza. (Nota: la password per la bozza è diversa dalla tua password di [!DNL Workfront]. La password per la bozza non è facilmente accessibile, quindi la maggior parte dei destinatari non la conosce.) [!DNL Workfront] consiglia di parlare con il proprio consulente di [!DNL Workfront] prima di utilizzare questa funzione.
* **[!UICONTROL Blocca la bozza quando vengono prese tutte le decisioni necessarie]:** questa opzione blocca la bozza per qualsiasi ulteriore commento, risposta, decisione, ecc., una volta che le decisioni sono state prese. Questa opzione blocca l’intera versione della bozza, non solo una fase specifica del flusso di lavoro.
* **[!UICONTROL Consenti il download del file originale]:** i destinatari della bozza possono scaricare il file sorgente originale della bozza dal Proofing Viewer (l’opzione si trova nel menu del pannello di destra).
* **[!UICONTROL Consenti condivisione bozze tramite URL pubblico o codice di incorporamento]:** i destinatari della bozza possono condividere con chiunque un collegamento alla bozza accessibile al pubblico.
* **[!UICONTROL Consenti la sottoscrizione alla bozza tramite URL pubblico o codice di incorporamento]:** chiunque riceve l’URL pubblico può aggiungersi alla bozza con il proprio indirizzo e-mail e nome (se non è un utente della bozza) o il proprio indirizzo e-mail e password della bozza (se è un utente della bozza). (Nota: la password della bozza non uguale a una password di [!DNL Workfront].)

Queste stesse impostazioni possono essere impostate quando la bozza viene caricata nella sezione [!UICONTROL Impostazioni bozza] nella parte inferiore della finestra di caricamento.

![Immagine della sezione [!UICONTROL Impostazioni bozza] nella parte inferiore della finestra di caricamento.](assets/proof-settings-on-upload-page.png)

### [!UICONTROL Attività bozza]

Questa pagina tiene traccia di tutte le attività che si sono verificate sulla bozza, oltre ai messaggi e-mail inviati relativi a questa bozza.

![Immagine della sezione [!UICONTROL Attività bozza] nella pagina della stessa con l’opzione [!UICONTROL Attività bozza] evidenziata nel menu del pannello a sinistra.](assets/proofing-activity-in-details.png)

Timestamp della sezione [!UICONTROL Attività] in cui sono presenti i commenti e le decisioni effettuati, oltre a chi li ha realizzati. Inoltre, tiene traccia dell’inizio delle fasi relative al flusso di lavoro di bozza, quando un destinatario ha aperto per la prima volta una bozza e altre informazioni utili per un responsabile o proprietario di bozza. Questi dettagli possono risultare utili quando desideri conoscere, ad esempio, il perché una fase del flusso di lavoro di bozza non ha mai avuto inizio.

Timestamp della sezione [!UICONTROL Messaggi] in cui sono presenti avvisi e messaggi e-mail inviati ai destinatari, i mittenti e il contenuto del messaggio. Ciò può risultare utile durante la risoluzione dei problemi, nel caso in cui qualcuno affermi di non aver ricevuto un’e-mail relativa a una bozza. Puoi verificare se e quando è stato inviato un messaggio e-mail.

[!DNL Workfront] consiglia al responsabile di bozza e al proprietario di bozza di acquisire familiarità con le informazioni contenute in queste due sezioni. La combinazione di queste informazioni con le istruzioni su come leggere la barra di avanzamento [!UICONTROL SOCD], ti consente di comprendere e gestire le bozze in modo efficace, indipendentemente dalla posizione che occupano all’interno del flusso di lavoro di bozza.

Dopo aver terminato il lavoro nella sezione [!UICONTROL Dettagli documento], utilizza il percorso breadcrumb per tornare alla sezione [!UICONTROL Documenti] di progetto, attività o problema a cui è allegata la bozza.

![Immagine del percorso breadcrumb nell’intestazione.](assets/proof-breadcrumb.png)

<!--
#### Learn more
* [!UICONTROL Document details] overview
* Add a custom form to a document
* Request document approvals
* Summary for documents overview
* View activity on a proof within [!DNL Workfront]
-->
