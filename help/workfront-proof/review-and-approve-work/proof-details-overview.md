---
title: Comprendere i dettagli della bozza
description: Approfondisci i dettagli dietro una bozza in [!DNL  Workfront] attraverso il pannello di riepilogo e [!UICONTROL Dettagli documento] pagina.
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Beginner
thumbnail: understand-proof-details.png
kt: 10110
exl-id: 196f9318-eced-4825-b0fd-8592b6cb3403
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '1029'
ht-degree: 0%

---

# Comprendere i dettagli della bozza

## Visualizza dettagli della bozza

In qualità di responsabile o proprietario della bozza, puoi approfondire i dettagli dietro una bozza attraverso il pannello di riepilogo e la [!UICONTROL Dettagli documento] pagina. Inizia trovando la tua bozza nella [!UICONTROL Documenti] sezione di un progetto, un&#39;attività o un problema.

### Pannello di riepilogo

Il pannello di riepilogo fornisce una panoramica di alto livello dei dettagli di base della bozza. Utilizza l’icona per espandere il pannello quando necessario e comprimerlo quando non lo desideri. Puoi anche passare il cursore sulla miniatura della bozza per aprirla o scaricarla.

![Un&#39;immagine del [!UICONTROL Documenti] di un progetto con una bozza selezionata e il pannello di riepilogo espanso. Vengono evidenziati sia l’icona del pannello di riepilogo che il pannello di riepilogo.](assets/document-summary.png)

Nota: La [!UICONTROL Approvazioni] nel pannello di riepilogo è **documento** approvazioni e **non** legato al processo di revisione e approvazione delle prove di cui hai appreso in questo corso. I due processi sono separati in [!DNL Workfront].

### [!UICONTROL Dettagli Documento]

Se hai bisogno di ulteriori informazioni sulla bozza, la [!UICONTROL Dettagli documento] Il collegamento ti porta alla &quot;pagina&quot; della bozza in [!DNL Workfront].

![Immagine della pagina della bozza in [!DNL  Workfront].](assets/document-details.png)

È importante notare che la capacità di visualizzare le informazioni relative al processo di correzione dipende dalle autorizzazioni di correzione in [!DNL Workfront].

Dalla pagina della bozza, puoi accedere a queste sezioni dal menu del pannello a sinistra:

* **Aggiornamenti —** I commenti fatti nel visualizzatore di prove compaiono qui, con un tag &quot;bozza commento&quot;. È inoltre possibile aggiungere commenti al file, come avviene per i commenti relativi a un’attività o a un progetto (i commenti non vengono visualizzati nel visualizzatore di prove).
* **Approvazioni —** Questa sezione riguarda le approvazioni dei documenti, non le approvazioni di correzione. I due tipi di approvazione sono processi separati in [!DNL Workfront] e non collegarsi tra loro. Se utilizzi flussi di lavoro di prova per le tue revisioni e approvazioni, non utilizzerai questa sezione.
* **Tutte le versioni —** Monitora e gestisci la cronologia delle versioni della bozza. È possibile che sia più semplice accedere a queste informazioni nel pannello di riepilogo nella sezione [!UICONTROL Documenti] elenco.
* **Forms personalizzato —** I moduli personalizzati vengono utilizzati nelle bozze per acquisire informazioni specifiche per l’organizzazione. Queste informazioni possono essere trasmesse con il file a sistemi di archiviazione documenti integrati, ad esempio [!DNL Workfront] DAM o [!DNL Adobe’s] AEM. I moduli personalizzati sono impostati dal [!DNL Workfront] amministratore di sistema o amministratore di gruppo. Parla con il tuo team o con i tuoi amministratori per sapere se userai moduli personalizzati sulle bozze.
* **Flusso di lavoro di correzione —** Gestisci o modifica il flusso di lavoro assegnato alla bozza. È possibile aprire questa finestra utilizzando [!UICONTROL Flusso di lavoro di correzione] link sulla bozza nella [!UICONTROL Documenti] anche elenco. Scopri come apportare modifiche al flusso di lavoro con il video Modifica un flusso di lavoro a prova di .

Esaminiamo due sezioni: [!UICONTROL Impostazioni del visualizzatore di correzione] e [!UICONTROL Attività di correzione].

### [!UICONTROL Impostazioni visualizzatore bozza]

Queste impostazioni consentono di controllare l’accesso alla bozza stessa.

![Un&#39;immagine del [!UICONTROL Impostazioni del visualizzatore di correzione] dalla pagina della bozza con [!UICONTROL Impostazioni del visualizzatore di correzione] evidenziata nel menu del pannello a sinistra.](assets/proofing-settings-on-details-page.png)

* **[!UICONTROL Accesso obbligatorio. Questa bozza non può essere condivisa con gli utenti ospiti] —** La prova può essere condivisa solo con persone che hanno un [!DNL Workfront] licenza di correzione.
* **[!UICONTROL Richiedere la firma elettronica delle decisioni] —** Quando condividi una bozza, il destinatario deve disporre delle autorizzazioni di correzione in [!DNL Workfront] e li fa &quot;firmare elettronicamente&quot; la prova inserendo la loro password di correzione quando prendono una decisione di prova. (Nota: La password di correzione è diversa dalla [!DNL Workfront] password. La password di correzione non è facilmente accessibile, pertanto la maggior parte dei destinatari non conosce questa password.) [!DNL Workfront] consiglia di parlare con [!DNL Workfront] consulente prima di utilizzare questa funzione.
* **[!UICONTROL Blocca la prova quando vengono prese tutte le decisioni necessarie ]—** Ciò blocca la prova di eventuali ulteriori osservazioni, risposte, decisioni, ecc., una volta presa ogni decisione sulla prova. Questo blocca l’intera versione della bozza, non solo una fase specifica del flusso di lavoro di correzione.
* **[!UICONTROL Consenti download del file originale] —** I destinatari della bozza possono scaricare il file sorgente originale della bozza dal visualizzatore di correzione (l’opzione è nel menu del pannello di destra).
* **[!UICONTROL Consenti condivisione di prove tramite URL pubblico o codice di incorporamento] —** I destinatari delle prove possono condividere con chiunque un link di prova accessibile al pubblico.
* **[!UICONTROL Consenti sottoscrizione a bozza tramite URL pubblico o codice di incorporamento] —** Chiunque venga inviato all’URL pubblico può aggiungersi alla bozza con il proprio indirizzo e-mail e nome (se non è un utente a prova di errore) o con il proprio indirizzo e-mail e password di correzione (se un utente a prova di errore). (Nota: La password di correzione non è la stessa di un [!DNL Workfront] password)

Puoi impostare queste stesse impostazioni quando la bozza viene caricata nel [!UICONTROL Impostazioni di bozza] nella parte inferiore della finestra di caricamento.

![Un&#39;immagine del [!UICONTROL Impostazioni di bozza] nella parte inferiore della finestra di caricamento.](assets/proof-settings-on-upload-page.png)

### [!UICONTROL Attività di correzione]

Questa pagina tiene traccia di tutta l’attività che si è verificata sulla bozza, oltre ai messaggi e-mail inviati relativi a questa bozza.

![Un&#39;immagine del [!UICONTROL Attività di correzione] della pagina della bozza con [!UICONTROL Attività di correzione] evidenziata nel menu del pannello a sinistra.](assets/proofing-activity-in-details.png)

La [!UICONTROL Attività] le marche temporali della sezione quando sono stati presi commenti e decisioni, oltre a chi li ha fatti. Monitora anche quando sono iniziate le fasi del flusso di lavoro di correzione, quando un destinatario ha aperto una bozza per la prima volta e altre informazioni che un responsabile o un proprietario della bozza vorrà sapere. Questi dettagli possono essere utili quando cerchi di capire perché, ad esempio, non è mai iniziata una fase del flusso di lavoro di correzione.

La [!UICONTROL Messaggi] marche temporali della sezione quando gli avvisi e i messaggi e-mail sono stati inviati ai destinatari, ai destinatari che li hanno inviati, e il contenuto del messaggio. Questa funzione può essere utile per la risoluzione dei problemi se qualcuno dice di non aver ricevuto un’e-mail su una bozza. Puoi verificare se e quando è stata inviata un’e-mail.

[!DNL Workfront] consiglia al responsabile della bozza e al proprietario della bozza di acquisire familiarità con le informazioni contenute in queste due sezioni. Quando si combinano queste informazioni con la comprensione di come leggere il [!UICONTROL SOCD] barra di avanzamento, è possibile comprendere e gestire le bozze, indipendentemente da dove si trovano nel flusso di lavoro di correzione.

Una volta terminato il lavoro nel [!UICONTROL Dettagli documento] sezione , utilizza la traccia breadcrumb per tornare alla [!UICONTROL Documenti] sezione del progetto, dell&#39;attività o del problema a cui è allegata la bozza.

![Immagine della traccia breadcrumb nell’intestazione.](assets/proof-breadcrumb.png)

<!--
#### Learn more
* [!UICONTROL Document details] overview
* Add a custom form to a document
* Request document approvals
* Summary for documents overview
* View activity on a proof within [!DNL Workfront]
-->
