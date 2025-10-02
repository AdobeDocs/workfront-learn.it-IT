---
title: Creare un’espressione di dati SUB, SUM, DIV o PROD
description: Scopri come utilizzare e creare le espressioni matematiche di base in un campo calcolato di Adobe  [!DNL Workfront].
feature: Custom Forms
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: 335177.png
jira: KT-8914
exl-id: e767b73b-1591-4d96-bb59-2f2521e3efa3
doc-type: video
source-git-commit: bbdf99c6bc1be714077fd94fc3f8325394de36b3
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 89%

---

# Creare un’espressione di dati SUB, SUM, DIV o PROD

In questo video scoprirai:

* Funzionamento delle espressioni SUB, SUM, DIV e PROD
* Come creare un’espressione di dati SUB in un campo calcolato

>[!VIDEO](https://video.tv.adobe.com/v/3414001/?quality=12&learn=on&enablevpops=1&captions=ita)

## Ulteriori informazioni: espressione ROUND

### Creare un’espressione ROUND

L’espressione ROUND accetta qualsiasi numero e lo arrotonda a un determinato numero di cifre decimali.

Nella maggior parte dei casi, l’espressione di dati ROUND viene utilizzata insieme a un’altra espressione di dati e quando il campo del formato viene lasciato come Testo o Numero.

Creiamo un campo calcolato per determinare la differenza tra il numero di ore pianificate e quelle effettivamente registrate per un’attività, che richiederà l’espressione SUB e avrà un aspetto simile al seguente:

**SUB({workRequired},{actualWorkRequired})**

Poiché il tempo viene tracciato in minuti e il formato preferito è quello di visualizzare le informazioni in ore, anche l’espressione deve essere divisa per 60 e avere un aspetto simile al seguente:

**DIV(SUB({workRequired},{actualWorkRequired}),60)**

Se il formato viene modificato in Numero durante la creazione del campo calcolato nel modulo personalizzato, è possibile modificare il formato numerico quando si aggiunge il campo in una vista.

![Bilanciatore del carico di lavoro con rapporto sull’utilizzo](assets/round01.png)

Tuttavia, se durante la creazione di un campo personalizzato il formato viene lasciato come Testo, non sarà possibile modificarlo facilmente all’interno della vista. L’espressione ROUND deve essere utilizzata per evitare di visualizzare numeri come questo nel progetto:

![Bilanciatore del carico di lavoro con rapporto sull’utilizzo](assets/round02.png)

<b>Utilizzare l’espressione di dati ROUND in un campo calcolato</b>

L’espressione ROUND include il nome dell’espressione (ROUND) e, in genere, due coordinate. Queste coordinate possono essere un’espressione o un campo in Workfront, seguiti da un numero che indica quante cifre decimali desideri spostare.

Un’espressione è strutturata nel modo seguente: ROUND(data point, #)

Nell&#39;espressione che calcola la differenza tra le ore pianificate e quelle effettive, utilizzare l&#39;espressione DIV(SUB({workRequired},{actualWorkRequired}),60) come primo punto dati. Assicurati quindi che qualsiasi numero provenga da quell’espressione non vada oltre 2 posizioni a destra del decimale.

![Bilanciatore del carico di lavoro con rapporto sull’utilizzo](assets/round03.png)

L&#39;espressione potrebbe essere scritta in questo modo: ROUND(DIV(SUB({workRequired},{actualWorkRequired}),60),2).
