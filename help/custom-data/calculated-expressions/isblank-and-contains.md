---
title: Utilizzare le espressioni ISBLANK e CONTAINS
description: Scopri come utilizzare e creare le espressioni ISBLANK e CONTAINS in un campo calcolato in Adobe  [!DNL Workfront].
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
ht-degree: 100%

---

# Utilizzare le espressioni ISBLANK e CONTAINS

Entrambe le espressioni CONTAINS e ISBLANK vengono utilizzate per fornire semplici valori vero o falso. La differenza è che l’espressione ISBLANK controlla se il campo contiene un valore mentre l’espressione di testo CONTAINS cerca una stringa specifica all’interno di un campo.

Ad esempio, per vedere se un progetto ha una descrizione, utilizza l’espressione ISBLANK. Se il campo della descrizione è vuoto, l’espressione restituisce il valore true. Se il campo descrizione non è vuoto, restituisce il valore false.

![Bilanciamento del carico di lavoro con rapporto sull’utilizzo](assets/isblank01.png)

Per cercare un valore specifico nella descrizione, ad esempio “evento di beneficenza”, utilizza l’espressione di testo CONTAINS. Se nella descrizione viene trovato “evento di beneficenza”, il campo calcolato indica “true”. Viene visualizzato “false”; se non trova “evento di beneficenza”.

![Bilanciatore del carico di lavoro con rapporto sull’utilizzo](assets/isblank02.png)

## ISBLANK

L’espressione di testo ISBLANK include il nome dell’espressione e una coordinata.

**ISBLANK({data point})**

![Bilanciatore del carico di lavoro con rapporto sull’utilizzo](assets/isblank03.png)

Nell’esempio precedente, in cui desideravi sapere se il progetto avesse una descrizione, l’espressione sarebbe:

ISBLANK({description})

## CONTAINS

L’espressione di testo CONTAINS include il nome dell’espressione, la parola o la frase che stai cercando e il campo in cui cercare.

**CONTAINS(&quot;frase&quot;,{fields})**

Assicurati di racchiudere tra virgolette la parola o la frase che stai cercando, altrimenti l’espressione non sarà valida.

Nell’esempio precedente (ricerca di “evento di beneficenza” nella descrizione del progetto), l’espressione sarebbe:

**CONTAINS(&quot;evento di beneficienza&quot;,{description})**

![Bilanciatore del carico di lavoro con rapporto sull’utilizzo](assets/isblank04.png)

**Nota**: l’espressione CONTAINS fa distinzione tra maiuscole e minuscole. Ad esempio, se “Evento di beneficenza” è scritto in maiuscolo nel campo della descrizione, scrivi in maiuscolo quella frase nell’espressione.

**CONTAINS(&quot;Evento di beneficienza&quot;,{description})**

Entrambe le espressioni ISBLANK e CONTAINS sono utili se vuoi vedere se è presente un valore. Tuttavia, potrebbe essere più utile sapere qual è il valore, vederlo effettivamente o avere una sorta di descrittore per fornire informazioni approfondite.

Ad esempio, invece di sapere semplicemente che un progetto è stato convertito da una richiesta, vuoi conoscere il nome della richiesta originale.

In tal caso, utilizza l’espressione CONTAINS insieme a un’espressione IF.

Nella maggior parte dei casi, le espressioni di testo ISBLANK e CONTAINS vengono utilizzate con un’espressione di testo IF.
