---
title: Comprendere le metriche delle prestazioni
description: 'Scopri come utilizzare le metriche delle prestazioni: il [!UICONTROL Metodo indice prestazioni] ([!UICONTROL PIM]) e la [!UICONTROL Stima al completamento] ([!UICONTROL EAC]).'
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: understand-performance-metrics.png
type: Tutorial
role: User
level: Intermediate
jira: KT-10065
hide: true
source-git-commit: d7347d41099e0faf6b47a6fe0e58091105e4e41d
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 100%

---

# Comprendere le metriche delle prestazioni

Due metriche delle prestazioni utilizzate dai project manager includono il [!UICONTROL Metodo indice prestazioni] ([!UICONTROL  PIM]) e la [!UICONTROL Stima al completamento] ([!UICONTROL  EAC]). È possibile configurare le impostazioni predefinite a livello di sistema in [!DNL Workfront] e applicarle ai progetti appena creati. Il [!UICONTROL PIM] può quindi essere modificato per singoli progetti.

**[!UICONTROL MIP]**

Le impostazioni per il [!UICONTROL PIM] controllano il modo in cui [!DNL Workfront] calcola altre metriche delle prestazioni del progetto, ad esempio l’[!UICONTROL Indice Performance Costi] ([!UICONTROL CPI]), l’[!UICONTROL Indice Performance Costo Programmato] ([!UICONTROL CSI]), l’[!UICONTROL Indice Performance Pianificazione] ([!UICONTROL SPI]), e la [!UICONTROL Stima al completamento] ([!UICONTROL EAC]).

Le opzioni per il [!UICONTROL PIM] sono basate su ore e su costi.

* **Basato su ore**: Workfront utilizza le ore pianificate per calcolare il CPI e l’EAC del progetto. L’EAC del progetto viene visualizzato come numero, in ore.
* **Basato su Costo**: Workfront utilizza il costo della manodopera pianificato per calcolare il CPI e l’EAC del progetto. L’EAC viene visualizzato come valore di valuta. Quando utilizzi questa opzione, assicurati che gli assegnatari delle attività (utenti e/o mansioni) siano associati ai tassi di costo.

**[!UICONTROL EAC]**

L’[!UICONTROL EAC] rappresenta il costo totale previsto per l’attività o il progetto al momento del completamento. Le opzioni vengono calcolate a livello di progetto e riportate dalle attività/attività secondarie.

* **Calcola a livello di progetto**: l’[!UICONTROL EAC] per l’attività principale e il progetto vengono determinati utilizzando le ore effettive/i costi effettivi della manodopera nelle formule [!UICONTROL EAC]. Il calcolo include le ore/i costi effettivi e le spese aggiunte direttamente all’attività principale o al progetto.
* **Riporta dalle attività/attività secondarie**: l’[!UICONTROL EAC] per l’attività principale e il progetto vengono determinati sommando l’[!UICONTROL EAC] per ogni attività secondaria. Questo calcolo esclude le ore/i costi effettivi aggiunti direttamente a un’attività principale o a un progetto.

I calcoli [!UICONTROL EAC] sono elencati in [Calcola stima al completamento (EAC)](https://experienceleague.adobe.com/docs/workfront/using/manage-work/projects/project-finances/calculate-eac.html?lang=it).

**Metriche delle prestazioni: impostazioni**

Per configurare le impostazioni predefinite di sistema per [!UICONTROL PIM] e [!UICONTROL EAC]:

1. Seleziona **[!UICONTROL Configurazione]** dal menu principale.
1. Fai clic su **[!UICONTROL Preferenze progetto]** nel menu del pannello sinistro, quindi fai clic su **[!UICONTROL Progetti]**
1. Nella sezione [!UICONTROL Stato del progetto], trova il [!UICONTROL Metodo indice prestazione]. Seleziona Basato su ore o Basato su Costo.
1. Per [!UICONTROL Stima al completamento], seleziona Calcola a livello di progetto o Riporta da attività/attività secondaria.
1. Fai clic su **[!UICONTROL Salva]** nella parte inferiore della finestra.

![Immagine della schermata [!UICONTROL Preferenze progetto] ](assets/setting-up-finances-1.png)

**Imposta il [!UICONTROL PIM] per singoli progetti**

1. Vai alla pagina di destinazione di un progetto.
1. Fai clic su **[!UICONTROL Dettagli progetto]** dal pannello a sinistra.
1. Apri la sezione **[!UICONTROL Finanza]**.
1. Fai doppio clic sul testo seguente **[!UICONTROL Metodo indice prestazioni]** per modificarlo.
1. Seleziona Basato su ore o Basato su Costo.
1. Fai clic su **[!UICONTROL Salva]** modifiche per terminare.

![Immagine della schermata [!UICONTROL Dettagli progetto]](assets/setting-up-finances-2.png)

Il[!UICONTROL PIM] può essere impostato su un modello di progetto, nella sezione [!UICONTROL Finanza] dei dettagli del modello.
