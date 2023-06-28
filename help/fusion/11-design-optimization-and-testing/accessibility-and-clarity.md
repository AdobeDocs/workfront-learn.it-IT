---
title: Accessibilità e chiarezza
description: Scopri alcune best practice di base per semplificare la lettura, la condivisione e la comprensione degli scenari.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11037
exl-id: ba2c5c64-ab4d-42d3-8a69-6b9df1373b29
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 0%

---

# Accessibilità e chiarezza

Nelle prime fasi del corso di formazione su Workfront Fusion, hai imparato alcune best practice di base per semplificare la lettura, la condivisione e la comprensione degli scenari. Queste procedure semplificano la risoluzione dei problemi o il supporto dell’istanza di Workfront Fusion per gli utenti futuri di Workfront Fusion. Pagalo seguendo le linee guida riportate di seguito durante la progettazione degli scenari.

## Etichette e note

Come regola generale, un obiettivo principale in Workfront Fusion è sempre quello di disporre di semplici progettazioni di scenari. Di seguito sono riportati alcuni modi per creare progettazioni semplici da interpretare.

* Accertati di denominare tutti i moduli. Fare clic con il pulsante destro del mouse su un modulo e selezionare Rinomina. Le etichette dei moduli devono essere brevi ma comprensibili per le prestazioni del modulo. Ad esempio, &quot;Crea Mktg Proj con Modello Ch&quot;.
  ![Immagine di uno scenario con gestione degli errori](assets/design-optimization-and-testing-1.png)
* Etichettare anche i percorsi di indirizzamento. Anche se un percorso non utilizza un filtro direttamente dopo un router, è possibile applicare un’etichetta senza compilare la logica del filtro. In questo modo altri utenti possono capire quali bundle passano, quali percorsi e perché. Per creare un&#39;etichetta per un percorso di router senza filtro, fare clic con il pulsante destro del mouse sul percorso, aggiungere un&#39;etichetta e salvare.
  ![Immagine di uno scenario con gestione degli errori](assets/design-optimization-and-testing-2.png)
* Se applicabile, aggiungi note in uno scenario se l’etichetta di un modulo o di un percorso di instradamento sarà troppo breve per chiarire cosa sta effettivamente accadendo. È possibile aggiungere note ogni volta che si desidera durante il processo di progettazione e iterazione.

Tuttavia, potrebbe essere più semplice da leggere e comprendere se aggiungi note alla fine del progetto dello scenario quando sei pronto per il lancio. Lavora dalla fine della progettazione dello scenario (l’angolo in basso a destra) all’indietro. In questo modo, le note applicabili all’inizio dello scenario si trovano in cima all’elenco quando si apre il pannello delle note.

Dopo aver salvato o chiuso il pannello note, le note vengono ordinate in base all&#39;ultima creazione. Nell&#39;immagine seguente, la prima nota creata viene visualizzata nella parte inferiore dell&#39;elenco. Le note venivano create intenzionalmente dall&#39;basso a destra fino al percorso indicato sopra e infine fino al trigger, essenzialmente nell&#39;ordine inverso in cui un pacchetto di dati passava attraverso lo scenario. In questo modo le note vengono visualizzate nell’ordine in cui lo scenario viene effettivamente eseguito sul bundle di dati.

![Immagine di uno scenario con gestione degli errori](assets/design-optimization-and-testing-3.png)

## Modelli Workfront Fusion

Un ottimo modo per semplificare l’etichettatura di moduli e percorsi di routing consiste nell’utilizzare i modelli. I modelli di best practice consentono di creare più rapidamente scenari per casi d’uso comuni.

### Esempio di modello

Quando avvii uno scenario, controlla innanzitutto se è disponibile un modello che possa essere utile. Ad esempio, per creare uno scenario che inizi scaricando un documento CSV da Workfront, quindi lo analizza.

Fai clic sulla sezione Modelli per verificare se eventuali modelli pubblici soddisfano le tue esigenze.

![Immagine di uno scenario con gestione degli errori](assets/design-optimization-and-testing-4.png)

Fare clic sulla scheda Modelli di team per verificare se un utente del team ha creato un modello che potrebbe essere utile.

Se si trova un modello da utilizzare, fare clic sul nome per aprirlo.

![Immagine di uno scenario con gestione degli errori](assets/design-optimization-and-testing-5.png)

Quindi vai all’angolo in alto a destra, fai clic su Opzioni e seleziona Crea scenario.

![Immagine di uno scenario con gestione degli errori](assets/design-optimization-and-testing-6.png)

### Creare un modello

È possibile creare un modello nella sezione Modelli team. Il modello creato è disponibile per te e per il tuo team, ma quando fai clic sul pulsante Pubblica puoi condividerlo con persone esterne al team.

![Immagine di uno scenario con gestione degli errori](assets/design-optimization-and-testing-7.png)

Durante la creazione di un modello, puoi includere una procedura guidata per guidare gli utenti che lo utilizzano nella creazione dei loro scenari, modificando le connessioni, i dati mappati e altri campi del pannello a seconda delle necessità.

Selezionare la casella di controllo &quot;Usa in procedura guidata&quot; per aggiungere le istruzioni che saranno disponibili quando qualcuno crea uno scenario utilizzando il modello. Queste informazioni verranno visualizzate nel campo Aiuto. Per consentire agli utenti di visualizzare questo testo quando utilizzano il modello, abilita Usa come valore predefinito.

![Immagine di uno scenario con gestione degli errori](assets/design-optimization-and-testing-8.png)

## Vuoi saperne di più? Consigliamo quanto segue:

[Documentazione di Workfront Fusion](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
