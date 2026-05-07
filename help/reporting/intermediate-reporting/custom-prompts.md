---
title: Creare prompt personalizzati utilizzando la modalità testo
description: Scopri che cos’è un prompt personalizzato, come crearne uno personalizzato utilizzando la modalità testo e alcuni esempi che è possibile utilizzare nel reporting in Workfront.
activity: use
feature: Reports and Dashboards
thumbnail: 336822.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
last-substantial-update: '2025-08-05T00:00:00.000Z'
jira: KT-9087
exl-id: 1bb0832e-e888-4154-b78d-24c6d69f629f
doc-type: video
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: c6dd2ac5-f5bd-4e59-9101-25b156918623
subfeature_v2:
  - id: cec4c78b-dd2b-46ec-b824-6ca30f0eb7b2
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-06T13:58:55.263Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 207
ht-degree: 92%

---

# Creare prompt personalizzati utilizzando la modalità testo

In questo video scoprirai:

* Che cos’è un prompt personalizzato
* Come creare un prompt personalizzato utilizzando la modalità testo
* Alcuni esempi che è possibile utilizzare nel reporting

>[!VIDEO](https://video.tv.adobe.com/v/336822/?quality=12&learn=on&enablevpops=0)

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
