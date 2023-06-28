---
title: Tracciamento avanzamento bozza
description: Scopri come utilizzare [!UICONTROL SOCD] indicatori, avanzamento bozza e rapporti per monitorare l’avanzamento di una bozza in [!DNL  Workfront].
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User
level: Beginner
thumbnail: track-proof-progress.png
jira: KT-10111
exl-id: 343483fe-487a-4a23-914d-2807a00630f9
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 1%

---

# Tracciamento avanzamento bozza

In qualità di project manager, proof manager o altre parti interessate nel processo di revisione e approvazione, potrai tenere traccia dell’avanzamento delle bozze. Puoi farlo con [!DNL Workfront’s] incorporato **indicatori di avanzamento bozza** il [!UICONTROL Documenti] o scrivendo rapporti personalizzati.

Per visualizzare l’avanzamento della bozza in [!DNL Workfront], è necessario disporre di una licenza Pianificazione, Lavoro o Revisione ed essere un utente di verifica. Se non è sicuro che il suo [!DNL Workfront] il profilo soddisfa questi requisiti, rivolgiti all’amministratore del sistema di verifica della tua organizzazione.

## Tracciare l’avanzamento della bozza con [!UICONTROL SOCD] indicatori e stato della bozza

Ottieni una visualizzazione di alto livello dell’avanzamento della bozza nel processo di revisione e approvazione utilizzando [!UICONTROL SOCD] icone in [!UICONTROL Documenti] elenco. Queste icone indicano le azioni specifiche eseguite sulla bozza.

![Un&#39;immagine del [!UICONTROL Documenti] elenco in un [!DNL  Workfront] progetto con [!UICONTROL SOCD] icone evidenziate.](assets/manage-proofs-socd.png)

Le icone indicano il lavoro svolto su una bozza dal momento dell’invio della bozza ai destinatari al momento in cui prendono una decisione sulla bozza.

* **S —** La bozza è stata inviata ai destinatari.
* **O —** Bozza aperta.
* **C —** Sono stati fatti commenti sulla prova.
* **D —** È stata presa una decisione sulla prova (approvata, respinta, ecc.).

I colori indicano se l&#39;azione è completa o meno.

* **Bianco —** Il passaggio non è ancora capitato.
* **Verde -** Passaggio completato.
* **Arancione —** La scadenza della bozza è entro 24 ore e il passaggio non è ancora avvenuto.
* **Rosso —** La scadenza della bozza è stata superata e il passaggio non è stato completato.

Il [!UICONTROL SOCD] il [!UICONTROL Documenti] nel pannello di riepilogo o nella sezione [!UICONTROL Dettagli documento], è un riepilogo ad alto livello dei progressi della bozza. [!DNL Workfront] configura questo in base al destinatario che è il &quot;più indietro&quot; nel processo di verifica.

Ad esempio, se sono presenti tre revisori/approvatori e solo due di essi hanno esaminato la bozza e formulato commenti, allora il [!UICONTROL SOCD] le icone mostrano che la bozza è stata inviata ([!UICONTROL S]) e aperto ([!UICONTROL O]) ma non che siano state fatte osservazioni ([!UICONTROL C]).

Per conoscere l’andamento di ogni singolo destinatario della bozza, apri il flusso di lavoro di bozza. L’avanzamento complessivo della bozza si trova nella parte superiore della finestra. Ogni fase presenta un proprio indicatore di avanzamento nella barra grigia.  E accanto a ogni utente c&#39;è il progresso di quel individuo.

![Un&#39;immagine del [!UICONTROL Flusso di lavoro bozza] sezione di un documento.](assets/manage-proofs-socd-in-proofing-workflow-window.png)

## Stato bozza

Lo stato della bozza si basa sullo stato dei destinatari della bozza della fase. Lo stato generale della bozza è visibile sul [!UICONTROL Documenti] a destra della pagina [!UICONTROL SOCD] , in modo da poter facilmente stabilire se si ha una decisione sulla bozza.

![Un&#39;immagine del [!UICONTROL Documenti] elenco in un [!DNL  Workfront] progetto con lo stato bozza generale evidenziato.](assets/manage-proofs-overall-status.png)

Questo stato della bozza indica lo stato generale della bozza. Ad esempio, se due destinatari hanno approvato la bozza, i loro stati individuali mostrano [!UICONTROL Approvato]. Tuttavia, il terzo destinatario non ha ancora preso una decisione, pertanto lo status di tale persona è [!UICONTROL In sospeso]. Pertanto, lo stato complessivo è indicato come [!UICONTROL In sospeso].

Se per la tua organizzazione sono stati configurati stati personalizzati, verranno utilizzati tali stati. In caso contrario, verranno visualizzate le opzioni di stato standard di:

* [!UICONTROL In Attesa]
* [!UICONTROL Approvato]
* [!UICONTROL Approvato con modifiche]
* [!UICONTROL Modifiche necessarie]
* [!UICONTROL Non pertinente]

Apri la finestra del flusso di lavoro di verifica per visualizzare lo stato della bozza per i destinatari assegnati al [!UICONTROL Revisore e Approvatore] o [!UICONTROL Approvatore]ruoli bozza.

## Rapporti in [!DNL Workfront]

Puoi anche sfruttare [!DNL Workfront’s] funzionalità di reporting per tenere traccia delle bozze durante il processo di revisione e approvazione.

Un report di approvazione della bozza consente di tenere traccia delle approvazioni in sospeso per garantire il rispetto delle scadenze.

![Immagine di un rapporto di approvazione della bozza in [!DNL  Workfront].](assets/proof-approval-report.png)

Un rapporto sulla versione del documento consente di gestire e tenere traccia delle versioni di una bozza.

![Immagine di un rapporto sulla versione di un documento in [!DNL  Workfront].](assets/document-version-report.png)

È consigliabile utilizzare [!DNL Workfront] per creare rapporti che soddisfino i requisiti aziendali. Alcuni dei rapporti richiedono familiarità con [!DNL Workfront’s] generazione rapporti in modalità testo.

## Tocca a te

Rivolgiti al team o all’amministratore di sistema per verificare quale tipo di reporting utilizzerai in Workfront per garantire il corretto funzionamento dei flussi di lavoro delle bozze.

<!--
### Learn more
* Learn to create reports in [!DNL Workfront] with the Basic Report Creation course.
* View progress and status of a proof
* View activity on a proof within [!DNL Workfront]
-->
