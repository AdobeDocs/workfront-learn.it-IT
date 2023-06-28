---
title: Rapporto sulle bozze
description: Scopri come utilizzare le funzionalità di reporting per gestire l’avanzamento della bozza.
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
thumbnail: report-on-proofs.png
jira: KT-10233
exl-id: 9a1a9e16-61cc-4f95-977a-8870b7fd0dda
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 0%

---

# Rapporto sulle bozze

[!DNL Workfront]Le funzioni di verifica digitale di consentono di gestire i progetti e i relativi flussi di lavoro di revisione in un’unica posizione — [!DNL Workfront]. Ottieni informazioni utili sul lavoro di verifica svolto con i tipi di rapporto, le origini dei campi e i nomi dei campi che visualizzano le informazioni di revisione e approvazione.

È consigliabile utilizzare [!DNL Workfront] per creare rapporti che soddisfino i requisiti aziendali. Alcuni dei rapporti richiedono familiarità con [!DNL Workfront]Generazione rapporti in modalità testo di.

Inizia con questi rapporti standard di base per aiutare i team a gestire le bozze attraverso un processo di revisione e approvazione in [!DNL Workfront].

## [!UICONTROL Approvazione bozza]

Questo tipo di rapporto consente di tenere traccia delle approvazioni di bozze in sospeso per garantire il rispetto delle scadenze.

![Seleziona [!UICONTROL Approvazione bozza] dal [!UICONTROL Nuovo rapporto] menu a discesa](assets/proof-system-setups-proof-approval-report.png)

Le opzioni di visualizzazione e filtro includono [!UICONTROL data della decisione], [!UICONTROL approvazione bozza], [!UICONTROL fase approvatore], [!UICONTROL modello di workflow], e [!UICONTROL informazioni richiedente]. Con la generazione rapporti in modalità testo, è possibile creare un raggruppamento che organizza l&#39;elenco in base al nome del documento. Consulta [Comprendere la modalità testo di base per i raggruppamenti](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/intermediate-reporting/basic-text-mode-for-groupings.html?lang=en).

Quando scrivi i rapporti sull’approvazione delle bozze, accertati di ricevere informazioni relative alla versione più recente delle bozze. [!DNL Workfront] consiglia di includere l’origine e il nome del campo seguenti nel filtro:

**[!UICONTROL Approvazione bozza]>>[!UICONTROL È la versione del documento corrente]**

![Scheda Filtri in Report Builder](assets/proof-system-setups-proof-approval-report-is-current-version.png)

Ciò è utile quando esegui rapporti sulle bozze con più versioni, in modo che nel rapporto venga elencata solo la versione corrente di ciascuna bozza che richiede l’approvazione. Questo filtra le versioni precedenti su cui non è più necessario lavorare.

## [!UICONTROL Versione documento]

Questo tipo di rapporto consente di gestire e tenere traccia delle versioni di [!DNL Workfront].

![Seleziona [!UICONTROL Versione documento] dal [!UICONTROL Nuovo rapporto] menu a discesa](assets/proof-system-setups-document-version-report.png)

Le opzioni di visualizzazione includono informazioni da [!UICONTROL versione del documento], [!UICONTROL documento], [!UICONTROL immesso da], [!UICONTROL stato approvazione bozza], [!UICONTROL autore bozza], e [!UICONTROL provider di documenti].

I raggruppamenti possono essere eseguiti da [!UICONTROL versione del documento], [!UICONTROL immesso da], [!UICONTROL stato approvazione bozza], o informazioni sul proprietario della bozza.

I filtri includono [!UICONTROL versione del documento], [!UICONTROL livello di accesso], [!UICONTROL documento], [!UICONTROL immesso da], [!UICONTROL stato approvazione bozza], [!UICONTROL autore bozza], e informazioni sul provider di documenti.

È possibile visualizzare il nome della fase di verifica attualmente attiva per ogni documento del report con questa colonna in una visualizzazione:

**[!UICONTROL Versioni documento] >> [!UICONTROL Fasi di bozza attive]**

![Scheda Filtri in Report Builder](assets/proof-system-setups-active-proof-stages.png)

Se non è attiva alcuna fase, la colonna è vuota.

Anche questa origine campo >> nome campo è disponibile come filtro in un rapporto.

Utilizza il [!UICONTROL Autore bozza] origine campo per creare rapporti sulle informazioni relative all’utente che ha creato la bozza. Scegli la [!UICONTROL Nome] origine campo per visualizzare il nome del creatore della bozza in una visualizzazione.

**[!UICONTROL Autore bozza] >> [!UICONTROL Nome]**

Anche questa combinazione di origine campo >> nome campo è disponibile come filtro.

![Scheda Filtri in Report Builder](assets/proof-system-setups-proof-creator-name.png)

<!--
Learn More Icon
Learn how to create reports in [!DNL Workfront] with the Report Creation class.
Access to proofing functionality
-->
