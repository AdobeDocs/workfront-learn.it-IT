---
title: Guida introduttiva a campi ed espressioni calcolati
description: Scopri come creare espressioni nei campi calcolati per raccogliere dati personalizzati univoci sul lavoro svolto per la tua organizzazione.
feature: System Setup and Administration
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: gs-calc-fields-expressions.png
exl-id: fbd17f01-9e97-4ead-9a56-7ce4f81255ec
source-git-commit: 2b9a31b45ff94222a77c05292ee5b9d8229f5f0b
workflow-type: tm+mt
source-wordcount: '527'
ht-degree: 0%

---

# Guida introduttiva a campi ed espressioni calcolati

<!-- **Note**: The expression examples shown are simple and some may be mitigated by fields already supplied by  . However, the examples are used to illustrate the foundational knowledge needed in order to build expressions in Workfront.-->

[!DNL Workfront] fornisce una varietà di campi comuni in più aree di business e utilizzati regolarmente per la gestione del lavoro. Campi quali data di completamento pianificato, budget del progetto, nome dell’assegnatario dell’attività, ecc.

Tuttavia, ogni organizzazione dispone di dati specifici per il proprio settore e azienda che devono essere raccolti per capire se gli obiettivi aziendali vengono raggiunti. Ad esempio, la tua organizzazione desidera tenere traccia di:

* A quale linea di business contribuirà un progetto.
* Se i finanziamenti provengono da fornitori, interni o entrambi.
* Risoluzione necessaria per le immagini utilizzate.

Anche se tali campi non sono incorporati in [!DNL Workfront], è possibile creare campi di immissione dati personalizzati e campi di risposta precompilati e con selezione multipla tramite un modulo personalizzato.

Questo percorso di apprendimento si concentra sul campo calcolato. Scoprirai cos’è un campo calcolato, i diversi tipi di informazioni che puoi inserire nel campo calcolato tramite espressioni di dati e come creare tali campi calcolati per migliorare la raccolta dati e il reporting.

![Gestione risorse imposta un pager](assets/GS01.png)

**Promemoria modulo personalizzata**

I campi sono specifici dell’oggetto. Ad esempio, se si crea un campo calcolato in un modulo personalizzato per attività, è possibile utilizzarlo in qualsiasi report per le attività.

## Cos’è un campo calcolato?

Un campo calcolato include i dati personalizzati creati utilizzando espressioni di dati e campi Workfront esistenti.

![Bilanciamento del carico di lavoro con rapporto di utilizzo](assets/GS02.png)

Ad esempio, la tua organizzazione dispone di una numerazione di progetto specifica o di un numero di lavoro che include:

* Anno di creazione del progetto,
* le iniziali del proprietario del progetto, e
* La [!DNL Workfront] numero di riferimento del progetto.


Utilizzando le espressioni in un campo calcolato, puoi prendere ogni informazione già memorizzata in [!DNL Workfront] e crea l&#39;ID progetto univoco, o numero di lavoro, che può essere aggiunto a un report come questo:

![Bilanciamento del carico di lavoro con rapporto di utilizzo](assets/GS03.png)

A seconda dei dati specifici necessari, i campi calcolati possono essere semplici utilizzando una o due espressioni o più complessi utilizzando diverse espressioni incorporate. Tieni presente che [!DNL Workfront] possono utilizzare solo i dati già memorizzati o estratti nel sistema per i campi calcolati.

## Espressioni di testo

Ricerca, dissezione e combinazione di informazioni presenti in espressioni di testo [!DNL Workfront] per creare dati più significativi o ottenere maggiori informazioni sul lavoro svolto per la tua organizzazione.

Ad esempio, le espressioni di testo possono essere utilizzate per:

* Mostra &quot;Oltre $5.000&quot; quando le spese del progetto sono superiori a $5.000, o &quot;Sotto $5.000&quot; quando le spese sono inferiori a tale valore, in una colonna di una visualizzazione del progetto.

* Attribuisci a ogni progetto un numero univoco che include l&#39;anno in cui il progetto è stato creato, il  [!DNL Workfront] numero di riferimento, il nome del progetto e le iniziali del proprietario del progetto.

* Crea un rapporto in cui vengono elencati tutti i progetti non assegnati a un portfolio e/o a un programma, in modo da poterli utilizzare nelle riunioni del tuo manager.

Le espressioni di testo possono essere utilizzate in un campo personalizzato per eseguire questi tipi di ricerche e combinazioni in [!DNL Workfront].
TE Quando si esaminano le possibili espressioni di testo, sono disponibili diverse opzioni.

![Gestione risorse imposta un pager](assets/TE01.png)

Esistono sei espressioni di testo utilizzate più spesso:

* CONCAT
* SINISTRA/DESTRA
* CONTAINS
* IF
* ISBLANK