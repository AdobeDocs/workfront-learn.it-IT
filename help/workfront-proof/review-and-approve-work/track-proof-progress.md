---
title: Tracciare l’avanzamento bozza
description: Scopri come utilizzare indicatori [!UICONTROL SOCD], avanzamento bozza e rapporti per monitorare l’avanzamento di una bozza in  [!DNL  Workfront].
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User
level: Beginner
thumbnail: track-proof-progress.png
jira: KT-10111
exl-id: 343483fe-487a-4a23-914d-2807a00630f9
source-git-commit: 8ad86921177da189503211635116146e886dbd17
workflow-type: tm+mt
source-wordcount: '767'
ht-degree: 64%

---

# Tracciare l’avanzamento bozza

In qualità di project manager, proof manager o altre parti interessate nel processo di revisione e approvazione, è necessario monitorare l’avanzamento delle bozze. Puoi farlo con gli **indicatori di avanzamento bozza** incorporati in [!DNL Workfront's] nella pagina [!UICONTROL Documenti] o scrivendo rapporti personalizzati.

Per visualizzare lo stato di avanzamento della bozza in [!DNL Workfront], è necessario disporre di una licenza Pianificazione, Lavoro o Revisione ed essere un utente bozza. Se non sei sicuro che il tuo profilo [!DNL Workfront] soddisfi questi requisiti, rivolgiti all&#39;amministratore del sistema di verifica della tua organizzazione.

## Tracciare l’avanzamento bozza con indicatori [!UICONTROL SOCD] e stato della bozza

Ottieni una visione di alto livello dell’avanzamento bozza attraverso il processo di revisione e approvazione utilizzando le icone [!UICONTROL SOCD] nell’elenco dei [!UICONTROL Documenti]. Queste icone indicano le azioni specifiche eseguite sulla bozza.

![Immagine dell’elenco dei [!UICONTROL Documenti] in un progetto [!DNL  Workfront] con le icone [!UICONTROL SOCD] evidenziate.](assets/manage-proofs-socd.png)

Le icone indicano il lavoro svolto su una bozza dal momento dell’invio della bozza ai destinatari al momento in cui questi prendono una decisione sulla bozza.

* **S:** la bozza è stata inviata ai destinatari.
* **O:** la bozza è stata aperta.
* **C:** sono stati effettuati commenti sulla bozza.
* **D:** è stata presa una decisione sulla bozza (approvata, respinta, ecc.).

I colori indicano se l’azione è completa o meno.

* **Bianco —** Il passaggio non è ancora stato eseguito.
* **Verde:** il passaggio è stato completato.
* **Arancione —** La scadenza della bozza è entro 24 ore e il passaggio non è stato eseguito.
* **Rosso -** La scadenza della bozza è stata superata e il passaggio non è stato eseguito.

Il [!UICONTROL SOCD] nell&#39;elenco [!UICONTROL Documenti], nel pannello di riepilogo o in [!UICONTROL Dettagli documento] è un riepilogo di alto livello dell&#39;avanzamento della bozza. [!DNL Workfront] configura questa impostazione in base al destinatario &quot;più indietro&quot; nel processo di verifica.

Ad esempio, se sono presenti tre revisori/approvatori e solo due di essi hanno esaminato la bozza e formulato commenti, allora le icone [!UICONTROL SOCD] mostrano che la bozza è stata inviata ([!UICONTROL S]) e aperta ([!UICONTROL O]) ma che non sono stati fatti commenti ([!UICONTROL C]).

**Una volta presa una decisione finale** (ad esempio, Approvato o Rifiutato) su una bozza, tutti gli indicatori SOCD potrebbero apparire verdi per gli utenti in quella fase, anche se non sono state eseguite singole azioni (ad esempio l&#39;apertura della bozza o la creazione di commenti). Si tratta di un comportamento a livello di sistema progettato per riflettere il completamento complessivo della fase, non il coinvolgimento individuale.

**Prima della registrazione di una decisione**, ogni indicatore SOCD riflette l&#39;attività utente effettiva (ad esempio, bianco se non è stata eseguita alcuna azione, verde se l&#39;azione è stata completata). Dopo la decisione, il sistema presuppone il completamento del flusso di lavoro e aggiorna di conseguenza tutti gli indicatori.

Se desideri conoscere l’andamento di ogni singolo destinatario di bozza, apri il flusso di lavoro bozza. L’avanzamento bozza generale è indicato nella parte superiore della finestra. Ogni fase riporta il proprio indicatore di avanzamento nella barra grigia.  E accanto a ogni utente c&#39;è il progresso di quell&#39;individuo.

![Immagine della sezione [!UICONTROL Flusso di lavoro bozza] di un documento.](assets/manage-proofs-socd-in-proofing-workflow-window.png)

## Stato della bozza

Lo stato della bozza si basa sullo stato dei destinatari della bozza della fase. Lo stato generale della bozza è visibile sulla pagina [!UICONTROL Documenti] a destra degli indicatori [!UICONTROL SOCD], in modo da poter facilmente stabilire la presenza di una decisione di bozza.

![Immagine dell’elenco dei [!UICONTROL Documenti] in un progetto [!DNL  Workfront] con lo stato generale della bozza evidenziato.](assets/manage-proofs-overall-status.png)

Questo stato della bozza indica lo stato generale della bozza. Ad esempio, se due destinatari hanno approvato la bozza, i loro stati individuali mostreranno [!UICONTROL Approvata]. Tuttavia, il terzo destinatario non ha ancora preso una decisione, quindi lo stato della persona è [!UICONTROL In sospeso]. Pertanto, lo stato generale è indicato come [!UICONTROL In sospeso].

Se per la tua organizzazione sono stati configurati stati personalizzati, verranno utilizzati tali stati. In caso contrario, verranno visualizzate le opzioni di stato standard di:

* [!UICONTROL In Attesa]
* [!UICONTROL Approvato]
* [!UICONTROL Approvato con modifiche]
* [!UICONTROL Modifiche necessarie]
* [!UICONTROL Non pertinente]

Apri la finestra del flusso di lavoro di bozza per visualizzare lo stato della bozza relativo ai destinatari assegnati ai ruoli bozza [!UICONTROL Revisore e Approvatore] o [!UICONTROL Approvatore].

## Rapporti in [!DNL Workfront]

Puoi anche sfruttare le funzionalità di reporting di [!DNL Workfront's] per tenere traccia delle bozze durante il processo di revisione e approvazione.

Un rapporto di approvazione bozza consente di tenere traccia delle approvazioni in sospeso per garantirne il rispetto delle scadenze.

![Immagine di un rapporto di approvazione bozza in [!DNL  Workfront].](assets/proof-approval-report.png)

Un rapporto sulla versione del documento consente di gestire e tenere traccia delle versioni di una bozza.

![Immagine di un rapporto sulla versione del documento in [!DNL  Workfront].](assets/document-version-report.png)

Ti consigliamo di lavorare con il consulente di [!DNL Workfront] per creare rapporti che soddisfino i requisiti dell’organizzazione. Alcuni dei rapporti richiedono familiarità con il reporting in modalità testo di [!DNL Workfront's].

## Tocca a te

Rivolgiti al team o all’amministratore del sistema di verifica per scoprire quale tipo di reporting utilizzerai in Workfront per garantire il corretto funzionamento dei flussi di lavoro delle bozze.

<!--
### Learn more
* Learn to create reports in [!DNL Workfront] with the Basic Report Creation course.
* View progress and status of a proof
* View activity on a proof within [!DNL Workfront]
-->
