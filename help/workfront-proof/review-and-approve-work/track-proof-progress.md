---
title: Come tenere traccia dell'avanzamento della bozza
description: Scopri come utilizzare [!UICONTROL SOCD] indicatori, progressi della prova e relazioni per monitorare l'avanzamento di una prova [!DNL  Workfront].
feature: Workfront Proof
type: Tutorial
role: User
level: Beginner
thumbnail: track-proof-progress.png
kt: 10111
exl-id: 343483fe-487a-4a23-914d-2807a00630f9
source-git-commit: 1f7a4da813805691fc0e52d3ad1ea708f9e07a9a
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 1%

---

# Tracciamento avanzamento

In qualità di project manager, responsabile delle prove o altro stakeholder nel processo di revisione e approvazione, dovrai tenere traccia dell’avanzamento delle bozze. Puoi eseguire questa operazione con [!DNL Workfront’s] incorporato **indicatori di avanzamento** sulla [!UICONTROL Documenti] o scrivendo rapporti personalizzati.

Per visualizzare l&#39;avanzamento della bozza in [!DNL Workfront], è necessario disporre di una licenza Plan, Work o Review ed essere un utente di correzione. Se non sei sicuro della tua [!DNL Workfront] profilo soddisfa i seguenti requisiti e verifica con l’amministratore del sistema di correzione della tua organizzazione.

## Tracciare l’avanzamento della bozza con [!UICONTROL SOCD] indicatori e stato della prova

Ottieni una visione di alto livello del progresso della bozza nel processo di revisione e approvazione utilizzando [!UICONTROL SOCD] le icone [!UICONTROL Documenti] elenco. Queste icone indicano le azioni specifiche eseguite sulla bozza.

![Un&#39;immagine del [!UICONTROL Documenti] in un elenco [!DNL  Workfront] con [!UICONTROL SOCD] icone evidenziate.](assets/manage-proofs-socd.png)

Le icone indicano il lavoro svolto su una bozza dal momento in cui la prova viene inviata ai destinatari fino al momento in cui decidono in merito alla bozza.

* **S —** La bozza è stata inviata ai destinatari.
* **O —** La prova è stata aperta.
* **C —** Sono state fatte osservazioni sulla prova.
* **D —** È stata presa una decisione sulla prova (approvata, respinta, ecc.).

I colori indicano se l’azione è completa o meno.

* **Bianco —** Il passaggio non è ancora successo.
* **Verde —** Il passaggio è stato completato.
* **Arancione —** La scadenza della bozza è entro 24 ore e il passaggio non è ancora avvenuto.
* **Rosso —** La scadenza della bozza è stata superata e il passaggio non è ancora avvenuto.

La [!UICONTROL SOCD] sulla [!UICONTROL Documenti] nel pannello di riepilogo o nel [!UICONTROL Dettagli documento], è un riepilogo ad alto livello dei progressi della bozza. [!DNL Workfront] configura in base al destinatario che è il &quot;più indietro&quot; nel processo di correzione.

Ad esempio, se ci sono tre revisori/approvatori e solo due di loro hanno esaminato la prova e fatto commenti, allora il [!UICONTROL SOCD] Le icone mostrano che la bozza è stata inviata ([!UICONTROL S]) e aperta ([!UICONTROL O]) ma non che siano state formulate osservazioni ([!UICONTROL C]).

Se vuoi sapere come sta funzionando ogni singolo destinatario della bozza, apri il flusso di lavoro di correzione. L’avanzamento generale della bozza si trova nella parte superiore della finestra. Ogni fase ha un proprio indicatore di avanzamento nella barra grigia.  E accanto a ogni utente c’è il progresso del singolo.

![Un&#39;immagine del [!UICONTROL Flusso di lavoro di correzione] sezione di un documento.](assets/manage-proofs-socd-in-proofing-workflow-window.png)

## Stato della bozza

Lo stato della bozza si basa sullo stato dei destinatari della bozza dell’area di visualizzazione. Lo stato generale della bozza è visibile sul [!UICONTROL Documenti] a destra di [!UICONTROL SOCD] indicatori, in modo da poter facilmente sapere se hai una decisione sulla bozza.

![Un&#39;immagine del [!UICONTROL Documenti] in un elenco [!DNL  Workfront] progetto con stato di bozza globale evidenziato.](assets/manage-proofs-overall-status.png)

Questo stato indica lo stato generale della bozza. Ad esempio, se due destinatari hanno approvato la bozza, i loro stati individuali vengono visualizzati [!UICONTROL Approvato]. Tuttavia, il terzo destinatario non ha ancora preso una decisione, in modo che lo stato della persona sia [!UICONTROL In sospeso]. Pertanto, lo stato generale appare come [!UICONTROL In sospeso].

Se per la tua organizzazione sono stati configurati degli stati personalizzati, questi verranno utilizzati. In caso contrario, vedrai le opzioni di stato standard di:

* [!UICONTROL In Attesa]
* [!UICONTROL Approvato]
* [!UICONTROL Approvato con modifiche]
* [!UICONTROL Modifiche necessarie]
* [!UICONTROL Non pertinente]

Apri la finestra del flusso di lavoro di correzione per visualizzare lo stato di una bozza per i destinatari assegnati al [!UICONTROL Revisore e approvatore] o [!UICONTROL Approvatore ]ruoli di bozza.

## Rapporti in [!DNL Workfront]

Puoi anche sfruttare [!DNL Workfront’s] funzionalità di reporting per tenere traccia delle bozze man mano che queste attraversano il processo di revisione e approvazione.

Un rapporto di approvazione della bozza consente di tenere traccia delle approvazioni in sospeso per assicurarsi che vengano rispettate le scadenze.

![Immagine di un rapporto di approvazione della prova in [!DNL  Workfront].](assets/proof-approval-report.png)

Un rapporto sulla versione del documento consente di gestire e tenere traccia delle versioni a prova di documento.

![Immagine di un rapporto sulla versione di un documento in [!DNL  Workfront].](assets/document-version-report.png)

È consigliabile lavorare con [!DNL Workfront] per creare rapporti che soddisfino i requisiti dell’organizzazione. Alcuni rapporti richiedono familiarità con [!DNL Workfront’s] generazione rapporti in modalità testo.

## Il tuo turno

Parla con il tuo team o con l’amministratore di sistema di correzione per scoprire che tipo di reporting utilizzerai in Workfront per mantenere in esecuzione senza problemi i flussi di lavoro a prova.

<!--
### Learn more
* Learn to create reports in [!DNL Workfront] with the Basic Report Creation course.
* View progress and status of a proof
* View activity on a proof within [!DNL Workfront]
-->
