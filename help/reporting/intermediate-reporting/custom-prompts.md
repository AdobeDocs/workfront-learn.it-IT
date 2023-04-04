---
title: Creare prompt personalizzati
description: Scopri cos’è un prompt personalizzato, come creare un prompt personalizzato utilizzando la modalità testo e alcuni esempi che puoi utilizzare nel reporting in Workfront.
activity: use
feature: Reports and Dashboards
thumbnail: 336822.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 9087
exl-id: 1bb0832e-e888-4154-b78d-24c6d69f629f
doc-type: video
source-git-commit: 650e4d346e1792863930dcebafacab4c88f2a8bc
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 2%

---

# Creare prompt personalizzati

In questo video imparerai:

* Richiesta personalizzata
* Come creare un prompt personalizzato utilizzando la modalità testo
* Alcuni esempi utilizzabili nei rapporti

>[!VIDEO](https://video.tv.adobe.com/v/336822/?quality=12&learn=on)

## Attività: Creare prompt personalizzati

1. Crea un prompt personalizzato che mostra i seguenti stati del progetto nel menu a discesa dei prompt:
   * In Pianificazione
   * Attuali
   * Completato
   * Morto
1. Modifica il prompt per visualizzare i progetti correnti che sono previsti questo mese.

## Risposte

1. I prompt personalizzati devono avere un aspetto simile a questo e avere la seguente modalità testo:

   ![Immagine della schermata per creare un nuovo filtro in modalità testo](assets/cp-01.png)

   Una volta salvato il prompt personalizzato, il menu a discesa del prompt dovrebbe avere l&#39;aspetto seguente:

1. La modalità testo nel prompt personalizzato dovrebbe essere simile alla seguente:

![Immagine della schermata per creare un nuovo filtro in modalità testo](assets/cp-02.png)

```
   status=CUR&plannedCompletionDate=$$TODAYbm&plannedCompletionDate_Mod=between&plannedCompletionDate_Range=$$TODAYem 
```

E l’etichetta a discesa per i prompt attivi deve essere aggiornata per riflettere la modifica nel codice come riportato di seguito:

![Immagine della schermata per creare un nuovo filtro in modalità testo](assets/cp-02a.png)
