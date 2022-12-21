---
title: Informazioni sulle espressioni campo calcolate
description: Visualizza un elenco di concetti utili per l’utilizzo dei campi calcolati personalizzati in [!DNL Workfront].
feature: System Setup and Administration
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: to-know-expressions.png
exl-id: 512a3071-f47f-4fd4-bf5f-9b18bef8ba59
source-git-commit: 402027429b116f3bd0328595b7c8635dea468fab
workflow-type: tm+mt
source-wordcount: '959'
ht-degree: 0%

---

# Informazioni sulle espressioni campo calcolate

Elenco di concetti che è utile conoscere quando si utilizzano campi calcolati personalizzati in Workfront.

## Casi nei nomi delle espressioni

Quando si tratta di nomi di espressione, il casing conta. Quando si scrive inizialmente un nome di espressione, è possibile utilizzare lettere maiuscole, minuscole o combinate entrambe.

![Messaggio di errore senza maiuscole nel nome dell&#39;espressione](assets/ttk-casingmatters01.png)

Tuttavia, l’espressione deve essere scritta come tutte le lettere maiuscole affinché il sistema riconosca l’espressione e salvi il campo.



## Le ore vengono memorizzate in minuti

Le ore nel database di Workfront sono memorizzate in minuti. Se fai riferimento a campi come Orari pianificati o Ore effettive, suddividi per 60 per mostrare l’ora in ore e non in minuti.

## La spaziatura non influisce sulle espressioni

Il modo consigliato per scrivere espressioni è con una spaziatura minima tra le espressioni e nulla.

* IF(ISBLANK({description}),&quot;Nessuna descrizione&quot;,&quot;Presenta descrizione&quot;)

![Espressioni senza spaziatura tra i campi](assets/spacing01.png)

Tuttavia, se la spaziatura consente di vedere cosa sta succedendo, è possibile aggiungere una certa spaziatura alle espressioni. Gli spazi aggiuntivi non devono impedire all’espressione di raccogliere o calcolare un valore in [!DNL Workfront].

* IF (ISBLANK ({description}), &quot;Nessuna descrizione&quot;, &quot;Presenta descrizione&quot; )

![Espressioni con spaziatura tra i campi](assets/spacing02.png)

Le uniche cose che non possono avere spazi tra loro sono i campi e le parentesi graffe. In caso contrario, riceverai un messaggio di errore e non potrai salvare il campo o il modulo personalizzato.

![Errore di spaziatura tra il nome del campo e la parentesi graffa](assets/spacing03.png)

## Le virgolette devono essere rette

Quando utilizzi le virgolette in un’espressione, accertati che le virgolette siano rette (&quot;). Se le virgolette sono curve (&quot;), la [!DNL Workfront] Il sistema continuerà a visualizzare un messaggio &quot;Espressione personalizzata non valida&quot;.

![Errore con virgolette curve](assets/curvedquotes01.png)

## Aggiornamento dei calcoli al salvataggio del modulo e alla modifica dell’oggetto

Questo è un aspetto importante dei campi calcolati da comprendere.

Le informazioni visualizzate in un campo calcolato rimarranno invariate e diventeranno obsolete a meno che il modulo personalizzato non venga ricalcolato.

È possibile aggiornare le espressioni utilizzando l’opzione Ricalcola espressioni nel menu Altro di un oggetto.

Desideri visualizzare il numero di giorni in cui un problema è stato aperto. Crea un campo calcolato denominato &quot;Giorni aperti&quot; con l’espressione DATEDIFF.

* Nome campo = Giorni aperti
* Espressione = DATEDIFF({entryDate},$$TODAY)

Una volta salvato, il numero di giorni tra la prima creazione o l’immissione del problema in Workfront e la data odierna può essere visualizzato nella pagina dei dettagli di un oggetto o in una visualizzazione di un rapporto.

Quando visualizzi la pagina dei dettagli o la visualizzazione del rapporto il giorno successivo, il numero verrà incrementato di uno. Se oggi il numero è 5, domani dovrebbe essere 6. Il giorno successivo dovrebbe essere 7, poi 8, ecc.

Tuttavia, il campo continuerà a essere visualizzato 5 ogni giorno. Il campo deve essere &quot;rieseguito&quot; o ricalcolato per aggiornare le informazioni.

Per aggiornare un campo utilizzando l’opzione Ricalcola espressioni :

* Fare clic sul nome dell’oggetto per aprirlo.
* Fare clic sul menu Altro.
* Seleziona Ricalcola espressioni dall’elenco.

![Opzione Ricalcola espressione nell&#39;oggetto](assets/recalculate01.png)

È inoltre possibile ricalcolare più espressioni contemporaneamente utilizzando la funzione di &quot;modifica collettiva&quot; in un elenco o in un rapporto. Supponiamo che sia stato creato un rapporto che mostra un elenco di problemi con il calcolo Giorni aperti visualizzato in una colonna. Se desideri ricalcolare tutti i problemi contemporaneamente:

* Seleziona tutti i problemi nel rapporto.
* Seleziona l’opzione di modifica per modificare in serie tutti i problemi selezionati.
* Fai clic sull’etichetta Forms personalizzata a sinistra per scorrere verso il basso fino alla sezione dei moduli personalizzati.
* Seleziona la casella Ricalcola espressioni personalizzate nella parte inferiore della sezione Forms personalizzata .
* Fai clic su Salva modifiche.

![Opzione Ricalcola espressione per più oggetti](assets/recalculate02.png)

La schermata si aggiorna per mostrare le informazioni aggiornate nel campo calcolato.

**Nota**: Anche se esistono altri modi per aggiornare o ricalcolare le espressioni in un campo calcolato, questo è il modo più rapido e semplice.

## I calcoli possono variare da un modulo all’altro all’interno dello stesso campo

Non appena un campo calcolato viene salvato in un modulo personalizzato e il modulo personalizzato viene salvato, il campo calcolato viene aggiunto alla libreria dei campi in modo che possa essere utilizzato in altri moduli personalizzati.

Tuttavia, se si dispone di un campo calcolato nel modulo A e dello stesso campo calcolato nel modulo B, si presume inizialmente che i calcoli siano esattamente gli stessi. Non è sempre così. Il campo calcolato nel modulo A potrebbe essere calcolato in modo completamente diverso nel modulo B.

Quando un campo personalizzato calcolato viene selezionato dalla libreria campi e aggiunto a un modulo personalizzato, il campo viene aggiunto ma il calcolo è vuoto. Uno dei motivi è che il calcolo può fare riferimento a campi che non esistono per un altro tipo di oggetto.

Ad esempio, hai creato un campo calcolato &quot;Giorni da completare&quot; per determinare quanto tempo è necessario per completare un’attività in un progetto.

* WEEKDAYDIFF({currentStartDate},{effectiveCompletionDate})

Vuoi fare la stessa cosa per un&#39;iterazione. È possibile utilizzare la stessa espressione; tuttavia, i campi disponibili per un oggetto attività non sono sempre disponibili per un oggetto iterazione. Quindi [!DNL Workfront] consente di creare il calcolo con i campi oggetto corretti.

**Suggerimento**: Copiare l’espressione calcolata dalla casella Calcolo nel campo Istruzioni durante la creazione di campi personalizzati. Questo campo non viene cancellato quando un campo personalizzato calcolato viene aggiunto al modulo personalizzato dalla Libreria campi.

A seconda delle esigenze, i campi calcolati nei moduli personalizzati possono essere molto semplici o molto complessi. Le espressioni possono incorporare, o nidificare, altre espressioni e valori per fornire il livello di dettaglio necessario per ottenere una migliore immagine di ciò che accade con il lavoro che viene svolto nell’organizzazione.

<!--Depending on the need, calculated fields in custom forms can be quite simple or very complex. Expressions can embed, or nest, other expressions and values to provide the level of detail needed to get a better picture of what is going on with the work being done at your organization. 

Most of the examples and exercises in this course have been relatively simple to provide a base understanding of the expressions most commonly used and how to build those expressions in a custom calculated field. 

Now you’re ready to start building your own calculated custom fields.-->
