---
title: Report sulle bozze
description: Scopri come utilizzare le funzionalità di reporting di per gestire l’avanzamento delle prove.
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
thumbnail: report-on-proofs.png
kt: 10233
exl-id: 9a1a9e16-61cc-4f95-977a-8870b7fd0dda
source-git-commit: a0aa8328842d2db1235edc42664eb0b18f4038e4
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 0%

---

# Rapporto sulle bozze

[!DNL Workfront]Le funzioni di correzione digitale consentono di gestire i progetti e i relativi flussi di lavoro di revisione in un’unica posizione — [!DNL Workfront]. Ottieni informazioni utili sul lavoro di correzione svolto con tipi di report, origini campo e nomi di campo che visualizzano informazioni di revisione e approvazione.

È consigliabile lavorare con [!DNL Workfront] per creare rapporti che soddisfino i requisiti dell’organizzazione. Alcuni rapporti richiedono familiarità con [!DNL Workfront]Generazione di rapporti in modalità testo .

Inizia con questi rapporti standard di base per aiutare i team a gestire le bozze attraverso un processo di revisione e approvazione in [!DNL Workfront].

## [!UICONTROL Approvazione bozza]

Questo tipo di rapporto ti aiuta a tenere traccia delle approvazioni delle prove in sospeso per assicurarsi che le scadenze vengano rispettate.

![Seleziona [!UICONTROL Approvazione della bozza] dal [!UICONTROL Nuovo rapporto] menu a discesa](assets/proof-system-setups-proof-approval-report.png)

Le opzioni di visualizzazione e filtro includono [!UICONTROL data della decisione], [!UICONTROL approvazione a prova], [!UICONTROL fase approvatore], [!UICONTROL modello di flusso di lavoro]e [!UICONTROL informazioni richieste]. Con il reporting in modalità testo, è possibile creare un raggruppamento che organizza l’elenco in base al nome del documento.

Quando scrivi rapporti di approvazione delle prove, assicurati di ricevere informazioni relative alla versione più recente delle bozze. [!DNL Workfront] consiglia di includere l’origine del campo e il nome del campo nel filtro:

**[!UICONTROL Approvazione della bozza]>>[!UICONTROL È la versione corrente del documento]**

![Scheda Filtri nel generatore di report](assets/proof-system-setups-proof-approval-report-is-current-version.png)

Questa funzione è utile quando esegui rapporti su bozze con più versioni, in modo che nel rapporto venga elencata solo la versione corrente di ogni bozza che necessita di approvazione. Questo filtra le versioni precedenti sulle quali non è più necessario lavorare.

## [!UICONTROL Versione documento]

Questo tipo di rapporto ti consente di gestire e tenere traccia delle versioni in [!DNL Workfront].

![Seleziona [!UICONTROL Versione documento] dal [!UICONTROL Nuovo rapporto] menu a discesa](assets/proof-system-setups-document-version-report.png)

Le opzioni di visualizzazione includono informazioni dal [!UICONTROL versione documento], [!UICONTROL documento], [!UICONTROL inserito da], [!UICONTROL stato di approvazione della prova], [!UICONTROL creatore di prove]e [!UICONTROL document provider].

I raggruppamenti possono essere effettuati da [!UICONTROL versione documento], [!UICONTROL inserito da], [!UICONTROL stato di approvazione della prova]o informazioni sul proprietario della bozza.

I filtri includono [!UICONTROL versione documento], [!UICONTROL livello di accesso], [!UICONTROL documento], [!UICONTROL inserito da], [!UICONTROL stato di approvazione della prova], [!UICONTROL creatore di prove]e informazioni sul provider di documenti.

È possibile visualizzare il nome della fase di correzione attiva per ogni documento del report con questa colonna in una visualizzazione:

**[!UICONTROL Versioni dei documenti] >> [!UICONTROL Stadi di prova attivi]**

![Scheda Filtri nel generatore di report](assets/proof-system-setups-active-proof-stages.png)

Se non è attiva alcuna fase, la colonna è vuota.

L’origine del campo >> nome del campo è disponibile anche come filtro in un rapporto.

Utilizza la [!UICONTROL Creatore di prove] origine del campo per creare rapporti sulle informazioni relative all’utente che ha creato la bozza. Scegli la [!UICONTROL Nome] origine del campo per visualizzare il nome dell’autore della bozza in una visualizzazione.

**[!UICONTROL Creatore di prove] >> [!UICONTROL Nome]**

Questa casella combinata origine campo >> nome campo è disponibile anche come filtro.

![Scheda Filtri nel generatore di report](assets/proof-system-setups-proof-creator-name.png)

<!--
Learn More Icon
Learn how to create reports in [!DNL Workfront] with the Report Creation class.
Access to proofing functionality
-->
