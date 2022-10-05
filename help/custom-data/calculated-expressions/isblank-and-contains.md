---
title: Utilizzare le espressioni ISBLANK e CONTAINS
description: Scopri come utilizzare e creare le espressioni ISBLANK e CONTAINS nel campo calcolato di un Adobe [!DNL Workfront].
feature: System Setup and Administration
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: isblank-contains.png
exl-id: 819ffec8-e7e6-4a3c-a589-1348aa09e27d
source-git-commit: 2b9a31b45ff94222a77c05292ee5b9d8229f5f0b
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 0%

---

# Utilizzare le espressioni ISBLANK e CONTAINS

Le espressioni CONTAINS e ISBLANK vengono utilizzate per fornire valori semplici true o false. La differenza è che l&#39;espressione ISBLANK controlla se il campo contiene un valore mentre l&#39;espressione di testo CONTAINS cerca una stringa specifica all&#39;interno di un campo.

Ad esempio, per verificare se un progetto ha una descrizione, utilizza l’espressione ISBLANK. Se il campo di descrizione è vuoto, l&#39;espressione restituisce il valore true. Se il campo di descrizione non è vuoto, restituisce un valore di false.

![Bilanciamento del carico di lavoro con rapporto di utilizzo](assets/isblank01.png)

Per cercare un valore specifico nella descrizione, ad esempio &quot;evento di beneficenza&quot;, utilizza l’espressione di testo CONTAINS. Se nella descrizione trova &quot;evento di beneficenza&quot;, il campo calcolato indica &quot;true&quot;. Mostra &quot;false&quot; se non trova &quot;evento di beneficenza&quot;.

![Bilanciamento del carico di lavoro con rapporto di utilizzo](assets/isblank02.png)

## ISBLANK

L&#39;espressione di testo ISBLANK include il nome dell&#39;espressione e un punto dati.

**ISBLANK(punto dati)**

![Bilanciamento del carico di lavoro con rapporto di utilizzo](assets/isblank03.png)

Nell’esempio precedente, dove desideri sapere se il progetto dispone di una descrizione, l’espressione è:

ISBLANK(Descrizione)

## CONTAINS

L&#39;espressione di testo CONTAINS include il nome dell&#39;espressione, la parola o la frase che si sta cercando e il campo da cercare.

**CONTAINS(&quot;frase&quot;,campo)**

Assicurati di inserire delle virgolette sulla parola o sulla frase che stai cercando, altrimenti l’espressione non sarà valida.

Nell’esempio precedente (cercando &quot;evento di beneficenza&quot; nella descrizione del progetto), l’espressione è:

**CONTAINS(&quot;evento di beneficenza&quot;, descrizione)**

![Bilanciamento del carico di lavoro con rapporto di utilizzo](assets/isblank04.png)

**Nota**: L&#39;espressione CONTAINS distingue tra maiuscole e minuscole. Ad esempio, se nel campo di descrizione &quot;Evento di carità&quot; viene utilizzato il maiuscolo, inserire la frase nell’espressione.

**CONTAINS(&quot;Evento di beneficenza&quot;,Descrizione)**

È utile utilizzare sia le espressioni ISBLANK che CONTAINS per verificare se è presente un valore. Tuttavia, può essere più utile sapere qual è il valore, vederlo effettivamente o avere qualche tipo di descrittore per fornire una visione migliore.

Ad esempio, invece di sapere solo che un progetto è stato convertito da una richiesta, vuoi conoscere il nome della richiesta originale.

In tal caso, utilizzare l&#39;espressione CONTAINS insieme a un&#39;espressione IF.

Più spesso, le espressioni di testo ISBLANK e CONTAINS vengono utilizzate con un&#39;espressione di testo IF.
