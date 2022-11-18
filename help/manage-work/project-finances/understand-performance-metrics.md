---
title: Comprendere le metriche delle prestazioni
description: 'Scopri come utilizzare le metriche delle prestazioni: [!UICONTROL Metodo indice prestazioni] ([!UICONTROL PIM]) e [!UICONTROL Stima al completamento] ([!UICONTROL EAC]).'
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: understand-performance-metrics.png
type: Tutorial
role: User
level: Intermediate
kt: 10065
exl-id: 190c66f5-b412-48bd-8695-3bd7da088ccb
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Comprendere le metriche delle prestazioni

Due metriche delle prestazioni utilizzate dai project manager includono: [!UICONTROL Metodo indice prestazioni] ([!UICONTROL PIM]) e [!UICONTROL Stima al completamento] ([!UICONTROL EAC]). I valori predefiniti a livello di sistema possono essere impostati in [!DNL Workfront] e si applicano ai progetti appena creati. [!UICONTROL PIM] possono quindi essere modificati su singoli progetti.

**[!UICONTROL MIP]**

Le impostazioni per [!UICONTROL PIM] controllare come [!DNL Workfront] calcola altre metriche delle prestazioni del progetto come [!UICONTROL Indice di prestazione dei costi] ([!UICONTROL CPI]), [!UICONTROL Indice delle prestazioni della pianificazione dei costi] ([!UICONTROL CSI]), [!UICONTROL Indice prestazioni pianificazione] ([!UICONTROL SPI]) e [!UICONTROL Stima al completamento] ([!UICONTROL EAC]).

Opzioni per [!UICONTROL PIM] sono basati su ore e su costi.

* **Basato su ora** — Workfront utilizza le ore previste per il calcolo dell&#39;IPC e dell&#39;EAC del progetto. L’EAC del progetto viene visualizzato come numero, in ore.
* **Basato sui costi** — Workfront utilizza il costo del lavoro previsto per il calcolo dell&#39;IPC e dell&#39;EAC del progetto. L&#39;EAC viene visualizzato come valore di valuta. Quando utilizzi questa opzione, assicurati che gli assegnatari delle attività (utenti e/o ruoli di lavoro) siano associati ai tassi di costo.

**[!UICONTROL CRS]**

[!UICONTROL EAC] rappresenta il costo totale previsto per l&#39;attività o il progetto al completamento. Le opzioni vengono calcolate a livello di progetto e si estendono da attività/sottoattività.

* **Calcola a livello di progetto** — [!UICONTROL EAC] per l&#39;attività padre e il progetto sono determinati utilizzando i costi effettivi di ore/effettivi di manodopera in [!UICONTROL EAC] formule. Il calcolo include ore/costi effettivi e spese aggiunte direttamente all&#39;attività o al progetto padre.
* R **aggregazione da attività/sottoattività** — [!UICONTROL EAC] per l&#39;attività e il progetto padre sono determinati sommando il [!UICONTROL EAC] per ogni attività figlio. Questo calcolo esclude le ore/i costi effettivi aggiunti direttamente a un&#39;attività o a un progetto padre.

La [!UICONTROL EAC] I calcoli sono elencati in &quot;Calcola stima al completamento (EAC)&quot; <!-- link to article -->articolo [!UICONTROL [!DNL Workfront] Uno].

**Metriche delle prestazioni: Impostazioni**

Per impostare [!UICONTROL PIM] e [!UICONTROL EAC] impostazioni predefinite del sistema:

1. Seleziona **[!UICONTROL Configurazione]** dal menu principale.
1. Fai clic su **[!UICONTROL Preferenze del progetto]** nel menu del pannello a sinistra, quindi fai clic su **[!UICONTROL Progetti]**
1. In [!UICONTROL Stato del progetto] sezione, trova [!UICONTROL Metodo indice prestazioni]. Seleziona basato su ore o su costi.
1. Per [!UICONTROL Stima al completamento], seleziona Calcola a livello di progetto o Esegui il rollup da attività/sottoattività.
1. Fai clic su **[!UICONTROL Salva]** in fondo alla finestra.

![Un&#39;immagine del [!UICONTROL Preferenze del progetto] screen](assets/setting-up-finances-1.png)

**Imposta [!UICONTROL PIM] sui singoli progetti**

1. Passa alla pagina di destinazione di un progetto.
1. Fai clic su **[!UICONTROL Dettagli progetto]** dal pannello a sinistra.
1. Apri **[!UICONTROL Finanza]** sezione .
1. Fai doppio clic sul testo sottostante **[!UICONTROL Metodo indice prestazioni]** per modificarlo.
1. Seleziona basato su ore o su costi.
1. Fai clic su **[!UICONTROL Salva]** Modifiche da completare.

![Un&#39;immagine del [!UICONTROL Dettagli progetto] screen](assets/setting-up-finances-2.png)

[!UICONTROL PIM] può essere impostato su un modello di progetto, nel [!UICONTROL Finanza] sezione dei dettagli del modello.
