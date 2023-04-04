---
title: Creare un'espressione dati SUB, SUM, DIV o PROD
description: Scopri come utilizzare e creare le espressioni matematiche di base nel campo calcolato a in Adobe [!DNL Workfront].
feature: System Setup and Administration
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: 335177.png
kt: 8914
exl-id: e767b73b-1591-4d96-bb59-2f2521e3efa3
doc-type: video
source-git-commit: 650e4d346e1792863930dcebafacab4c88f2a8bc
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 0%

---

# Creare un&#39;espressione dati SUB, SUM, DIV o PROD

In questo video imparerai:

* Funzionamento delle espressioni SUB, SUM, DIV e PROD
* Come creare un’espressione di dati SUB in un campo calcolato

>[!VIDEO](https://video.tv.adobe.com/v/335177/?quality=12&learn=on)

## Informazioni aggiuntive: Espressione ROUND

### Creare un&#39;espressione ROUND

L&#39;espressione ROUND prende qualsiasi numero e lo arrotonda a un certo numero di posizioni decimali.

Nella maggior parte dei casi, l&#39;espressione di dati ROUND viene utilizzata insieme a un&#39;altra espressione di dati e quando il campo di formato viene lasciato come Testo o Numero.

Creare un campo calcolato per determinare la differenza tra il numero di ore pianificate e effettivamente registrate su un&#39;attività, che richiederà l&#39;espressione SUB e avrà un aspetto simile al seguente:

**SUB({workRequired},{effectiveWorkRequired})**

Poiché il tempo è tracciato in minuti e il formato preferito è quello di mostrare le informazioni in ore, anche l&#39;espressione deve essere divisa per 60 e avere questo aspetto:

**DIV(SUB({workRequired},{effectiveWorkRequired}), 60)**

Se il formato viene modificato in Numero durante la creazione del campo calcolato nel modulo personalizzato, è possibile modificare il formato del numero quando si aggiunge il campo in una visualizzazione.

![Bilanciamento del carico di lavoro con rapporto di utilizzo](assets/round01.png)

Tuttavia, se il formato del campo durante la creazione di un campo personalizzato viene lasciato come Testo, il formato non può essere facilmente modificato all’interno della visualizzazione. L’espressione ROUND deve essere utilizzata per evitare di visualizzare nel progetto numeri come questo:

![Bilanciamento del carico di lavoro con rapporto di utilizzo](assets/round02.png)

<b>Utilizzare l&#39;espressione di dati ROUND in un campo calcolato</b>

L&#39;espressione ROUND include il nome dell&#39;espressione (ROUND) e, in genere, due punti di dati. Questi punti dati possono essere un&#39;espressione o un campo in Workfront, seguiti da un numero che indica quante posizioni decimali si desidera utilizzare.

Un&#39;espressione sarebbe strutturata in questo modo: ROUND(punto dati, #)

Nell&#39;espressione che calcola la differenza tra le ore pianificate e effettive, utilizza questa espressione —DIV(SUB({workRequired},{effectiveWorkRequired}),60) come primo punto di dati. Assicurati quindi che qualsiasi numero venga da quell&#39;espressione non superi 2 posizioni a destra del decimale.

![Bilanciamento del carico di lavoro con rapporto di utilizzo](assets/round03.png)

L&#39;espressione potrebbe essere scritta così: ROUND(DIV(SUB({workRequired},{effectiveWorkRequired}), 60), 2).
