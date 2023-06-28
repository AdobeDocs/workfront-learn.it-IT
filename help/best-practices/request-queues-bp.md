---
title: Best practice - Code di richieste
description: Esplora le best practice consigliate dagli esperti Adobe Workfront in merito all’impostazione, alla gestione e all’utilizzo delle code di richieste Workfront.
feature: Resource Management
role: Admin, Leader, User
level: Beginner
jira: KT-10921
exl-id: dbb961f9-c207-49f1-9545-ec127f983c15
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '1480'
ht-degree: 0%

---

# Best practice - Code di richieste

## Cos’è una &quot;best practice&quot; di Adobe Workfront?

Le best practice sono linee guida che rappresentano una linea di condotta efficace ed efficiente, sono facilmente adottabili da te e dagli utenti della tua azienda e possono essere replicate correttamente all’interno dell’organizzazione.

Mentre esamini questi consigli, tieni presente che alcune best practice di Workfront sono universali, mentre altre potrebbero essere più specifiche per l’argomento. Utilizza queste best practice come framework per guidare le impostazioni e l’utilizzo del sistema Workfront.

## Navigazione in questa pagina

Scorrendo questa pagina, troverai innanzitutto un elenco di alto livello di tutte le best practice per l’argomento. Questo ti consente di rivedere i consigli senza immergerti nei dettagli di &quot;perché&quot;.

La sezione &quot;Perché sono queste best practice?&quot; , disponibile dopo l’elenco di alto livello, fornisce maggiori dettagli su alcune delle best practice e sul perché sono considerate un processo, uno strumento, ecc., è consigliabile implementarle con l’istanza di Workfront.

</br>
</br>

## Best practice per le code di richieste

* Includere una descrizione per ogni elemento di una coda di richieste, ovvero il progetto della coda di richieste, i gruppi di argomenti, gli argomenti della coda e le regole di instradamento.

* Crea uno stato di progetto denominato &quot;Coda richieste&quot; o &quot;Operativo&quot; che sia uguale a &quot;Corrente&quot; per distinguere i progetti della coda richieste da altri progetti.

* Se prevedi di utilizzare le approvazioni dei problemi con le richieste inviate tramite una coda, crea uno stato di problema denominato Rifiutato.

* Assegna moduli personalizzati &quot;universali&quot; alle code di richieste per acquisire il maggior numero possibile di dati coerenti a livello aziendale.

* Evita di condividere le code di richieste con &quot;tutti&quot;. Impostare le impostazioni dei dettagli della coda in modo che gli utenti possano visualizzare solo le code pertinenti alle proprie esigenze.

* Crea e assegna un dashboard contenente i report della coda di richieste in modo che i gestori del traffico, gli amministratori di sistema o gli utenti assegnati possano lavorare direttamente sui problemi.

* Utilizza i modelli di layout per rimuovere le opzioni di configurazione della coda richieste dal menu del pannello a sinistra dei progetti, per gli utenti che non hanno bisogno di creare code.

* Creare una coda di richieste di amministratore di sistema per consentire agli utenti di porre domande relative a Workfront, effettuare richieste relative alle impostazioni di sistema, pianificare nuovi corsi di formazione per gli utenti, ecc.

* Controlla regolarmente le code di richieste per identificare e annullare la condivisione delle code non utilizzate.

* Utilizza i gruppi di argomenti per organizzare più di 10 argomenti della coda in una coda di richieste per creare elenchi più brevi e facili da gestire.

* Controllare il numero totale di code di richieste disponibili per gli utenti suddividendo una coda di richieste utilizzando gruppi di argomenti e argomenti della coda, anziché creare più code.

* Impostare le regole di instradamento per ogni argomento della coda. Impostare almeno una regola di instradamento predefinita.

* Utilizza i gruppi di argomenti e gli argomenti della coda quando è necessario il routing selettivo.

* Indirizza le richieste a un team, anziché a un singolo utente.


</br>
</br>


## Perché si tratta di procedure ottimali?


**Best practice**

Includere una descrizione per ogni elemento di una coda di richieste, ovvero il progetto della coda di richieste, i gruppi di argomenti, gli argomenti della coda e le regole di instradamento.

**Ecco perché**

Le descrizioni consentono agli amministratori di gruppi, ai futuri amministratori di sistema o ad altri che gestiscono code di richieste di sapere esattamente cosa fa ogni parte della coda di richieste.

Le informazioni descrittive vengono visualizzate anche quando passi il cursore sull’icona delle informazioni nel campo della finestra della nuova richiesta.

La descrizione non deve essere necessariamente lunga, ma solo un breve commento sullo scopo o sull’utilizzo dell’elemento.

</br>
</br>

**Best practice**

Crea uno stato di progetto denominato &quot;Coda richieste&quot; o &quot;Operativo&quot; che sia uguale a &quot;Corrente&quot; per distinguere i progetti della coda richieste da altri progetti.

**Ecco perché**

Una coda di richieste &quot;vive&quot; in un progetto e deve trovarsi in uno stato uguale a Corrente affinché la coda sia attiva.

Per distinguere una richiesta dai progetti di lavoro effettivi con stato &quot;Corrente&quot;, creare uno stato da utilizzare solo sulle code di richiesta denominate &quot;Coda di richiesta&quot; o &quot;Operativa&quot;. Puoi quindi utilizzare questo stato per escludere o includere i progetti della coda di richieste durante la scrittura dei rapporti.

</br>
</br>

**Best practice**

Creare uno stato di problema denominato &quot;Rifiutato&quot; quando si utilizzano approvazioni di problemi e impostare l&#39;opzione Se rifiutato sullo stato &quot;Rifiutato&quot;.

**Ecco perché**

L&#39;utilizzo dello stato &quot;Rifiutato&quot; indica chiaramente che la richiesta è stata esaminata e rifiutata.

</br>
</br>

**Best practice**

Assegna moduli personalizzati &quot;universali&quot; alle code di richieste per acquisire il maggior numero possibile di dati coerenti a livello aziendale.

**Ecco perché**

Un modulo personalizzato &quot;universale&quot; raccoglie le informazioni standard necessarie per la richiesta, indipendentemente dal tipo di richiesta inviata.

L’utilizzo di un modulo personalizzato &quot;universale&quot; consente di ridurre il numero di moduli personalizzati da creare e mantenere. Inoltre, garantisce che tutte le richieste raccolgano le stesse informazioni nello stesso modo, con conseguente coerenza nelle attività di reporting e analisi dei dati.

</br>
</br>

**Best practice**

Evita di condividere le code di richieste con &quot;tutti&quot;.  Impostare le impostazioni dei dettagli della coda in modo che gli utenti possano visualizzare solo le code pertinenti alle proprie esigenze.

**Ecco perché**

Nella maggior parte dei casi, una coda di richieste deve essere condivisa solo con un determinato gruppo di persone come un team, un fornitore, clienti e così via. Quando i richiedenti visualizzano solo ciò di cui hanno bisogno nell’elenco della coda delle richieste, è più semplice trovare e navigare.

</br>
</br>


**Best practice**

Crea e assegna un dashboard contenente i report della coda di richieste in modo che i gestori del traffico, gli amministratori di sistema o gli utenti assegnati possano lavorare direttamente sui problemi.

**Ecco perché**

Consentire agli utenti di accedere in modo semplice e rapido alle richieste in arrivo significa non perdere il lavoro nel miscuglio.

</br>
</br>

**Best practice**

Utilizza i modelli di layout per rimuovere le opzioni di configurazione della coda richieste dal menu del pannello a sinistra dei progetti, per gli utenti che non hanno bisogno di creare code.


**Ecco perché**

In questo modo tutte le code di richieste seguono il processo appropriato per la creazione (ad esempio vengono esaminate da un comitato di governance) e vengono configurate correttamente da un amministratore di sistema o di gruppo.

Inoltre, questo aiuta a mantenere l’elenco delle code organizzato e concentrato sui tipi di richieste di cui la tua organizzazione ha bisogno.

</br>
</br>

**Best practice**

Creare una coda di richieste di amministratore di sistema per consentire agli utenti di porre domande relative a Workfront, effettuare richieste relative alle impostazioni di sistema, pianificare nuovi corsi di formazione per gli utenti, ecc.

**Ecco perché**

In questo modo, gli utenti possono inviare domande da una posizione centralizzata e gli amministratori possono raccogliere, monitorare e rispondere ai problemi relativi a Workfront.

Inoltre, queste informazioni possono essere utilizzate per mostrare alla leadership il tempo, l&#39;impegno e il valore del ruolo di amministratore di sistema e come giustificazione per un amministratore di sistema aggiuntivo.

</br>
</br>


**Best practice**

Controlla regolarmente le code di richieste per identificare e annullare la condivisione delle code non utilizzate.

**Ecco perché**

Un controllo regolare delle impostazioni e degli elementi nel sistema Adobe Workfront lo consente di mantenere il sistema ordinato e privo di elementi non necessari. Se una coda non viene più utilizzata o monitorata, assicurati che gli utenti non possano più accedervi in modo che le richieste di lavoro non cadano in un vuoto.

</br>
</br>


**Best practice**

Utilizza i gruppi di argomenti per organizzare più di 10 argomenti della coda in una coda di richieste per creare elenchi più brevi e facili da gestire.

**Ecco perché**

I gruppi di argomenti aumentano l’adozione da parte dell’utente e creano meno confusione diminuendo l’elenco iniziale di opzioni tra cui selezionare. Questo consente agli utenti di trovare facilmente ciò che cercano senza sopraffarli quando tentano di inviare una richiesta.

Inoltre, consente agli amministratori di sistema e/o ai responsabili delle code di richieste di creare un percorso di navigazione fluido per gli utenti e un modo migliore per organizzare e generare rapporti sui tipi di richieste inviate.

</br>
</br>

**Best practice**

Controllare il numero totale di code di richieste disponibili per gli utenti suddividendo una coda di richieste utilizzando gruppi di argomenti e argomenti della coda, anziché creare più code.

**Ecco perché**

Troppe code di richieste rendono difficile agli utenti trovare ciò di cui hanno bisogno.

Un numero inferiore di code consente inoltre ai coordinatori del traffico, agli amministratori di sistema o ad altri utenti di gestire le code, consentendo loro di trovare le informazioni necessarie più rapidamente, senza dover passare a più progetti di code di richieste.

Creare più code di richiesta se è necessario un accesso diverso per le diverse code di richiesta o se il consolidamento delle code potrebbe confondere gli utenti.

</br>
</br>

**Best practice**

Impostare le regole di instradamento per ogni argomento della coda. Impostare almeno una regola di instradamento predefinita.

**Ecco perché**

Le regole di instradamento garantiscono che a qualcuno venga sempre assegnata la richiesta in ingresso in modo che il lavoro non vada perduto.

</br>
</br>

**Best practice**

Utilizza i gruppi di argomenti e gli argomenti della coda quando è necessario il routing selettivo.

**Ecco perché**

Impossibile applicare le regole di indirizzamento ai campi di un modulo personalizzato. Pertanto, se è necessario instradare diversi tipi di richieste a team/singoli utenti diversi, impostare ogni tipo di richiesta come gruppo di argomenti/argomento della coda in modo che il lavoro possa essere instradato correttamente.

</br>
</br>

**Best practice**

Indirizza le richieste a un team, anziché a un singolo utente.

**Ecco perché**

Quando le richieste vengono inviate al team, questo offre all’intero team la visibilità delle richieste in corso e di ciò che potrebbe comportare il lavoro in programma. Tutti possono guardare la pagina Team per trovare nuovi elementi o tenere traccia delle novità con un rapporto su un dashboard.

Inoltre, quando il gestore del traffico o un’altra persona incaricata di esaminare o assegnare le richieste in ingresso non è disponibile, garantisce che sia automaticamente disponibile un backup e che abbia accesso alle informazioni della richiesta.
