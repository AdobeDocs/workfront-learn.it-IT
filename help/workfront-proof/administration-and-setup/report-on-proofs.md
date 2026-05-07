---
title: Rapporto sulle bozze
description: Scopri come utilizzare le funzionalità di reporting per gestire l’avanzamento bozza.
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
thumbnail: report-on-proofs.png
jira: KT-10233
exl-id: 9a1a9e16-61cc-4f95-977a-8870b7fd0dda
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2: id: b18b693b-6d59-4359-95fd-a386b7a615fe
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-05T20:06:01.017Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 454
ht-degree: 100%

---

# Rapporto sulle bozze

Le funzionalità per la verifica delle bozze digitali di [!DNL Workfront] consentono di gestire i progetti e i relativi flussi di lavoro di revisione in un’unica posizione: [!DNL Workfront]. Ottieni informazioni utili sul lavoro di bozza svolto con i tipi di rapporto, le origini dei campi e i nomi dei campi che mostrano le informazioni di revisione e approvazione.

Ti consigliamo di lavorare con il consulente di [!DNL Workfront] per creare rapporti che soddisfino i requisiti dell’organizzazione. Alcuni dei rapporti richiedono familiarità con il reporting in modalità testo di [!DNL Workfront].

Inizia con questi rapporti standard di base per aiutare i team a gestire le bozze attraverso un processo di revisione e approvazione in [!DNL Workfront].

## [!UICONTROL Approvazione bozza]

Questo tipo di rapporto consente di tenere traccia delle approvazioni bozza in sospeso per garantire il rispetto delle scadenze.

![Seleziona [!UICONTROL Approvazione bozza] dal menu a discesa [!UICONTROL Nuovo rapporto]](assets/proof-system-setups-proof-approval-report.png)

Le opzioni di visualizzazione e di filtro includono la [!UICONTROL data della decisione], l’[!UICONTROL  approvazione bozza], la [!UICONTROL fase di approvazione], il [!UICONTROL modello di flusso di lavoro] e le [!UICONTROL informazioni sul richiedente]. Con il reporting in modalità testo è possibile creare un raggruppamento che organizza l’elenco in base al nome del documento. Consulta [Comprendere la modalità testo di base per i raggruppamenti](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/intermediate-reporting/basic-text-mode-for-groupings.html?lang=it).

Quando scrivi rapporti di approvazione bozza, assicurati di ricevere informazioni relative alla versione più recente delle bozze. [!DNL Workfront] consiglia di includere questa origine e questo nome del campo nel filtro:

**[!UICONTROL Approvazione bozza]>>[!UICONTROL È la versione del documento corrente]**

![Scheda Filtri in Report Builder](assets/proof-system-setups-proof-approval-report-is-current-version.png)

Ciò è utile quando stai generando rapporti su bozze che hanno più versioni in modo che il rapporto elenchi solo la versione corrente di ogni bozza che necessita di approvazione. Questo filtra le versioni precedenti su cui non è più necessario lavorare.

## [!UICONTROL Versione documento]

Questo tipo di rapporto consente di gestire e tenere traccia delle versioni di [!DNL Workfront].

![Seleziona [!UICONTROL Versione documento] dal menu a discesa [!UICONTROL Nuovo rapporto]](assets/proof-system-setups-document-version-report.png)

Le opzioni di visualizzazione includono informazioni da: [!UICONTROL Versione documento], [!UICONTROL Documento], [!UICONTROL Immesso da], [!UICONTROL Stato approvazione bozza], [!UICONTROL Autore bozza], e [!UICONTROL Provider di documenti].

I raggruppamenti possono essere eseguiti da [!UICONTROL Versione documento], [!UICONTROL Immesso da], [!UICONTROL Stato approvazione bozza] o informazioni sul proprietario della bozza.

I filtri includono [!UICONTROL Versione documento], [!UICONTROL Livello di accesso], [!UICONTROL Documento], [!UICONTROL Immesso da], [!UICONTROL Stato approvazione bozza], [!UICONTROL Autore bozza] e informazioni sul provider di documenti.

È possibile visualizzare il nome della fase di bozza attualmente attiva per ogni documento del rapporto con questa colonna in una vista:

**[!UICONTROL Versioni documento] >> [!UICONTROL Fasi di bozza attive]**

![Scheda Filtri in Report Builder](assets/proof-system-setups-active-proof-stages.png)

Se non è attiva alcuna fase, la colonna è vuota.

Anche questa origine campo >> nome campo è disponibile come filtro in un rapporto.

Utilizza l’origine campo [!UICONTROL Autore bozza] per segnalare informazioni sull’utente che ha creato la bozza. Scegli l’origine campo [!UICONTROL Nome] per visualizzare il nome dell’autore della bozza in una vista.

**[!UICONTROL Creatore della bozza] >> [!UICONTROL Nome]**

Anche questa combinazione di origine campo >> nome campo è disponibile come filtro.

![Scheda Filtri in Report Builder](assets/proof-system-setups-proof-creator-name.png)

<!--
Learn More Icon
Learn how to create reports in [!DNL Workfront] with the Report Creation class.
Access to proofing functionality
-->
