---
title: Informazioni sulla navigazione e la revisione dei progetti in [!UICONTROL Analisi avanzata]
description: Scopri come leggere il grafico del piano di volo in Workfront.
activity: use
feature: Reports and Dashboards
thumbnail: 335047.png
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
kt: 8729
exl-id: 1409a1af-3bdb-40f7-af01-f9de2357b602
source-git-commit: 252ba3ba44f22519a35899fcda9c6bca597a6c2c
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---

# Informazioni sulla navigazione e la revisione dei progetti in [!UICONTROL Analisi avanzata]

In questo video imparerai:

* Come leggere il grafico del piano di volo

>[!VIDEO](https://video.tv.adobe.com/v/335047/?quality=12)

## Grafico a pianta di volo

![Immagine di un grafico a piani di volo con numeri corrispondenti ai punti elenco seguenti](assets/section-2-1.png)

Sul grafico vengono visualizzati i seguenti elementi:

1. I nomi dei progetti sono a sinistra.
1. Le date sono visualizzate in basso.
1. La linea blu verticale mostra la data specifica in cui il mouse si trova al passaggio del mouse.
1. Le linee blu orizzontali mostrano le date di inizio e di fine pianificate del progetto.
1. Le linee verdi indicano che il progetto è su Target.
1. Le linee arancioni indicano che il progetto è a rischio.
1. Le linee rosse indicano che il progetto è in difficoltà.

La visualizzazione di queste informazioni sui progetti consente di determinare:

* Eventi che estendono un progetto oltre la data di completamento pianificata.
* Quando un progetto inizia ad avere problemi.
* Quanti progetti sono aperti nello stesso periodo di tempo.
* Quanti progetti sono attivi.
* Quali progetti necessitano di maggiore attenzione o sostegno.

## La condizione si basa sullo stato di avanzamento

La condizione del progetto è una rappresentazione visiva dell’avanzamento del progetto. Workfront determina la condizione in base allo stato di avanzamento delle attività all’interno del progetto.

![Immagine dei possibili stati di avanzamento](assets/section-2-2.png)

È possibile impostare la condizione di un progetto:

* **Manualmente**, da parte degli utenti con accesso per gestire il progetto, quando il tipo di condizione del progetto è impostato su manuale. Questo consente di impostare la condizione del progetto indipendentemente dal percorso critico.
* **Automaticamente**, di Workfront, quando il tipo di condizione del progetto è impostato su Stato di avanzamento.

Workfront consiglia di impostare il tipo di condizione su Stato avanzamento in modo da avere un&#39;indicazione chiara dell&#39;effettivo avanzamento del progetto, in base all&#39;avanzamento delle attività.

![Immagine dei possibili stati di avanzamento](assets/section-2-3.png)

In questo caso, la condizione del progetto può essere:

* **Su Target**- Quando lo stato di avanzamento dell’ultima attività sul percorso critico è On Time, la condizione del progetto sarà On Target. Il progetto è in fase di completamento in base alla pianificazione.
* **A rischio**- Quando lo stato di avanzamento dell’ultima attività sul percorso critico è Behind o At Risk, la condizione del progetto è At Risk. Il progetto è in procinto di terminare tardi, ma non è ancora in ritardo.
* **In problemi**- Quando lo stato di avanzamento dell’ultima attività sul percorso critico è in ritardo, la condizione del progetto è In problemi. La data di scadenza è passata e il progetto è ora in ritardo.

>[!NOTE]
>
>Le condizioni possono essere personalizzate per il tuo ambiente, quindi potresti trovare più di tre opzioni o i nomi possono essere diversi da quelli sopra indicati. Per informazioni sulla personalizzazione delle condizioni, consulta l’articolo Creare o modificare una condizione personalizzata .
