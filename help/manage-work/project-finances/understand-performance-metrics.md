---
title: Comprendere le metriche delle prestazioni
description: 'Scopri come utilizzare le metriche delle prestazioni: il [!UICONTROL Metodo indice prestazioni] ([!UICONTROL PIM]) e [!UICONTROL Stima al completamento] ([!UICONTROL EAC]).'
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: understand-performance-metrics.png
type: Tutorial
role: User
level: Intermediate
jira: KT-10065
exl-id: 190c66f5-b412-48bd-8695-3bd7da088ccb
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '433'
ht-degree: 0%

---

# Comprendere le metriche delle prestazioni

Due metriche delle prestazioni utilizzate dai project manager includono [!UICONTROL Metodo indice prestazioni] ([!UICONTROL PIM]) e [!UICONTROL Stima al completamento] ([!UICONTROL EAC]). Le impostazioni predefinite a livello di sistema possono essere impostate in [!DNL Workfront] e si applicano ai progetti appena creati. [!UICONTROL PIM] può quindi essere modificato su singoli progetti.

**[!UICONTROL MIP]**

Le impostazioni per [!UICONTROL PIM] controllare come [!DNL Workfront] calcola altre metriche delle prestazioni del progetto, ad esempio [!UICONTROL Indice Performance Costi] ([!UICONTROL CPI]), [!UICONTROL Indice Performance Costo Programmato] ([!UICONTROL CSI]), [!UICONTROL Indice Performance Schedule] ([!UICONTROL SPI]), e [!UICONTROL Stima al completamento] ([!UICONTROL EAC]).

Opzioni per [!UICONTROL PIM] sono basati su ore e su costi.

* **Basato su Ore** — Workfront utilizza le ore pianificate per calcolare l&#39;IPC e l&#39;CES del progetto. Il CES del progetto viene visualizzato come numero, in ore.
* **Basato su Costo** — Workfront utilizza il costo della manodopera pianificato per calcolare l&#39;IPC e l&#39;EAC del progetto. EAC viene visualizzato come valore di valuta. Quando si utilizza questa opzione, assicurarsi che gli assegnatari delle attività (utenti e/o mansioni) siano associati ai tassi di costo.

**[!UICONTROL CRS]**

[!UICONTROL EAC] rappresenta il costo totale previsto dell&#39;attività o del progetto al completamento. Le opzioni vengono calcolate a livello di progetto e riportate dalle attività/sottoattività.

* **Calcola a livello di progetto** — [!UICONTROL EAC] per l&#39;attività e il progetto padre vengono determinati utilizzando le ore effettive/i costi effettivi della manodopera in [!UICONTROL EAC] formule. Il calcolo include le ore/i costi effettivi e le spese aggiunte direttamente all&#39;attività o al progetto padre.
* R **Esegui il rollup da attività/sottoattività** — [!UICONTROL EAC] per l&#39;attività e il progetto padre vengono determinati sommando i [!UICONTROL EAC] per ogni attività figlio. Questo calcolo esclude le ore/i costi effettivi aggiunti direttamente a un&#39;attività o a un progetto padre.

Il [!UICONTROL EAC] i calcoli sono elencati in [Calcola stima al completamento (EAC)](https://experienceleague.adobe.com/docs/workfront/using/manage-work/projects/project-finances/calculate-eac.html?lang=en).

**Metriche delle prestazioni: Impostazioni**

Per impostare [!UICONTROL PIM] e [!UICONTROL EAC] impostazioni predefinite di sistema:

1. Seleziona **[!UICONTROL Configurazione]** dal menu principale.
1. Clic **[!UICONTROL Preferenze progetto]** nel menu del pannello sinistro, fai clic su **[!UICONTROL Progetti]**
1. In [!UICONTROL Stato progetto] sezione, trova [!UICONTROL Metodo indice prestazioni]. Selezionare Basato su ore o Basato su Costo.
1. Per [!UICONTROL Stima al completamento], selezionare Calcola a livello di progetto o Riporta da attività/sottoattività.
1. Clic **[!UICONTROL Salva]** nella parte inferiore della finestra.

![Un&#39;immagine del [!UICONTROL Preferenze progetto] screen](assets/setting-up-finances-1.png)

**Imposta [!UICONTROL PIM] su singoli progetti**

1. Vai alla pagina di destinazione di un progetto.
1. Clic **[!UICONTROL Dettagli progetto]** dal pannello a sinistra.
1. Apri **[!UICONTROL Finanza]** sezione.
1. Fare doppio clic sul testo seguente **[!UICONTROL Metodo indice prestazioni]** per modificarlo.
1. Selezionare Basato su ore o Basato su Costo.
1. Clic **[!UICONTROL Salva]** Modifiche di fine.

![Un&#39;immagine del [!UICONTROL Dettagli progetto] screen](assets/setting-up-finances-2.png)

[!UICONTROL PIM] può essere impostato su un modello di progetto, nel [!UICONTROL Finanza] sezione dei dettagli del modello.
