---
title: Utilizzare le espressioni ISBLANK e CONTAINS
description: Scopri come utilizzare e creare le espressioni ISBLANK e CONTAINS nel campo calcolato di un Adobe [!DNL Workfront].
feature: Custom Forms
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: isblank-contains.png
exl-id: 819ffec8-e7e6-4a3c-a589-1348aa09e27d
source-git-commit: 409147f9a62302d28e14b834981992a0421d4e4b
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 0%

---

# Utilizzare le espressioni ISBLANK e CONTAINS

Entrambe le espressioni CONTAINS e ISBLANK vengono utilizzate per fornire valori true o false semplici. La differenza consiste nel fatto che l&#39;espressione ISBLANK controlla se il campo contiene un valore mentre l&#39;espressione di testo CONTAINS cerca una stringa specifica all&#39;interno di un campo.

Ad esempio, per verificare se un progetto ha una descrizione, utilizza l’espressione ISBLANK. Se il campo descrizione è vuoto, l’espressione restituisce il valore true. Se il campo descrizione non è vuoto, restituisce il valore false.

![Bilanciatore dei carichi di lavoro con rapporto sull’utilizzo](assets/isblank01.png)

Per cercare un valore specifico nella descrizione, come &quot;evento benefico&quot;, utilizza l’espressione di testo CONTAINS. Se trova &quot;evento benefico&quot; nella descrizione, il campo calcolato indica &quot;true&quot;. Se non viene trovato un &quot;evento di beneficenza&quot;, viene visualizzato &quot;false&quot;.

![Bilanciatore dei carichi di lavoro con rapporto sull’utilizzo](assets/isblank02.png)

## ISBLANK

L&#39;espressione di testo ISBLANK include il nome dell&#39;espressione e una coordinata.

**ISBLANK({data point})**

![Bilanciatore dei carichi di lavoro con rapporto sull’utilizzo](assets/isblank03.png)

Nell’esempio precedente, dove desideri sapere se il progetto ha una descrizione, l’espressione sarebbe:

ISBLANK({description})

## CONTAINS

L&#39;espressione di testo CONTAINS include il nome dell&#39;espressione, la parola o la frase che si sta cercando e il campo in cui eseguire la ricerca.

**CONTAINS(&quot;phrase&quot;,{fields})**

Assicurati di racchiudere tra virgolette la parola o la frase che stai cercando, altrimenti l’espressione non sarà valida.

Nell’esempio precedente (cercando &quot;evento di beneficenza&quot; nella descrizione del progetto), l’espressione sarebbe:

**CONTAINS(&quot;evento di beneficenza&quot;,{description})**

![Bilanciatore dei carichi di lavoro con rapporto sull’utilizzo](assets/isblank04.png)

**Nota**: l’espressione CONTAINS distingue tra maiuscole e minuscole. Ad esempio, se &quot;Evento di beneficenza&quot; è scritto in maiuscolo nel campo di descrizione, inserisci tale frase nell’espressione.

**CONTAINS(&quot;Evento benefico&quot;,{description})**

Entrambe le espressioni ISBLANK e CONTAINS sono utili per verificare se è presente un valore. Tuttavia, può essere più utile sapere qual è il valore, visualizzarlo effettivamente o avere una sorta di descrittore per fornire informazioni migliori.

Ad esempio, invece di sapere che un progetto è stato convertito da una richiesta, vuoi conoscere il nome della richiesta originale.

In tal caso, utilizzare l&#39;espressione CONTAINS insieme a un&#39;espressione IF.

Nella maggior parte dei casi, le espressioni di testo ISBLANK e CONTAINS vengono utilizzate con un&#39;espressione di testo IF.
