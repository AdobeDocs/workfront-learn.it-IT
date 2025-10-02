---
title: Creare prompt personalizzati
description: Scopri che cos’è un prompt personalizzato, come crearne uno personalizzato utilizzando la modalità testo e alcuni esempi che è possibile utilizzare nel reporting in Workfront.
activity: use
feature: Reports and Dashboards
thumbnail: 336822.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
last-substantial-update: 2025-08-05T00:00:00Z
jira: KT-9087
exl-id: 1bb0832e-e888-4154-b78d-24c6d69f629f
doc-type: video
source-git-commit: 1fafcafb173ceb4115612e1c33ca36564c7a6c3d
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 97%

---

# Creare prompt personalizzati

In questo video scoprirai:

* Che cos’è un prompt personalizzato
* Come creare un prompt personalizzato utilizzando la modalità testo
* Alcuni esempi che è possibile utilizzare nel reporting

>[!VIDEO](https://video.tv.adobe.com/v/3412691/?quality=12&learn=on&captions=ita)

## Attività &quot;Crea prompt personalizzati&quot;


### Attività: creare prompt personalizzati

1. Crea un prompt personalizzato che mostri i seguenti stati di progetto nel menu a discesa del prompt:
   * In Pianificazione
   * Attuali
   * Completato
   * Morto
1. Modifica il prompt per visualizzare i progetti correnti in scadenza questo mese.

### Risposte

1. I prompt personalizzati devono avere un aspetto simile a questo e la seguente modalità testo:

   ![Immagine della schermata per creare un nuovo filtro in modalità testo](assets/cp-01.png)

   Dopo aver salvato il prompt personalizzato, il menu a discesa del prompt dovrebbe essere simile al seguente:

1. La modalità testo nel prompt personalizzato deve essere simile alla seguente:

![Immagine della schermata per creare un nuovo filtro in modalità testo](assets/cp-02.png)

```
   status=CUR&plannedCompletionDate=$$TODAYbm&plannedCompletionDate_Mod=between&plannedCompletionDate_Range=$$TODAYem 
```

L’etichetta a discesa dei prompt attivi deve essere aggiornata per riflettere la modifica nel codice come segue:

![Immagine della schermata per creare un nuovo filtro in modalità testo](assets/cp-02a.png)
