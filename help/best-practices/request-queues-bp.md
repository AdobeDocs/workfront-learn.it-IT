---
title: 'Procedure consigliate: code di richiesta'
description: Scopri le best practice consigliate dagli esperti Adobe Workfront sull’impostazione, la gestione e l’utilizzo delle code di richiesta Workfront.
feature: Resource Management
role: Admin, Leader, User
level: Beginner
kt: 10921
exl-id: dbb961f9-c207-49f1-9545-ec127f983c15
source-git-commit: 444f059d3cc26d8e3074a7145bc5419407c786cf
workflow-type: tm+mt
source-wordcount: '1480'
ht-degree: 0%

---

# Procedure consigliate: code di richiesta

## Qual è una &quot;best practice&quot; di Adobe Workfront?

Le migliori pratiche sono linee guida che rappresentano un&#39;azione efficace ed efficiente; sono facilmente adottati da te e dagli utenti della tua azienda; e può essere replicato correttamente in tutta l’organizzazione.

Quando si esaminano queste raccomandazioni, tenere presente che alcune best practice di Workfront sono universali, mentre altre potrebbero essere più specifiche per l’argomento. Utilizza queste best practice come framework per guidare le impostazioni e l’utilizzo del sistema Workfront.

## Navigazione in questa pagina

Scorrendo questa pagina, troverai innanzitutto un elenco di alto livello contenente tutte le best practice per l’argomento. Questo ti consente di rivedere le raccomandazioni senza immergerti nei dettagli del &quot;perché&quot;.

Perché queste best practice? area, disponibile dopo l’elenco di alto livello, fornisce maggiori dettagli su alcune delle best practice e sui motivi per cui vengono considerate un processo, uno strumento, ecc., dovresti considerare l’implementazione con la tua istanza Workfront.

</br>
</br>

## Best practice per le code di richiesta

* Includi una descrizione per ogni elemento di una coda di richiesta: il progetto della coda di richiesta, i gruppi di argomenti, gli argomenti della coda e le regole di indirizzamento.

* Crea uno stato di progetto denominato &quot;Coda richieste&quot; o &quot;Operativo&quot; che equivale a &quot;Corrente&quot; per distinguere i progetti in coda richieste da altri progetti.

* Se prevedi di utilizzare le approvazioni dei problemi con le richieste inviate tramite una coda, crea uno stato di problema denominato Rifiutato.

* Assegna moduli personalizzati &quot;universali&quot; per richiedere code per acquisire il maggior numero possibile di dati coerenti a livello aziendale.

* Evita di condividere le code di richiesta con &quot;tutti&quot;. Imposta le impostazioni dei dettagli della coda in modo che gli utenti vedano solo le code pertinenti in base alle loro esigenze.

* Crea e assegna un dashboard contenente i rapporti sulla coda delle richieste in modo che i responsabili del traffico, gli amministratori di sistema o gli utenti assegnati possano lavorare direttamente sui problemi.

* Utilizza i modelli di layout per rimuovere le opzioni di configurazione della coda di richiesta dal menu del pannello a sinistra dei progetti per gli utenti che non hanno bisogno di creare code.

* Crea una coda di richiesta dell’amministratore di sistema per consentire agli utenti di porre domande relative a Workfront, effettuare richieste relative alle impostazioni di sistema, pianificare nuovi corsi di formazione per gli utenti, ecc.

* Controlla regolarmente le code di richiesta per identificare e annullare la condivisione delle code che non vengono utilizzate.

* Utilizza i gruppi di argomenti per organizzare più di 10 argomenti della coda in una coda di richiesta per creare elenchi più brevi e facili da gestire.

* Controlla il numero totale di code di richiesta disponibili agli utenti suddividendo una coda di richiesta utilizzando gruppi di argomenti e argomenti della coda, anziché creare più code.

* Imposta le regole di routing per ogni argomento della coda. Come minimo, impostare una regola di routing predefinita.

* Sfrutta i gruppi di argomenti e gli argomenti della coda quando è necessario indirizzare selettivo.

* Indirizza le richieste a un team, anziché a un singolo utente.


</br>
</br>


## Perché queste best practice sono?


**Best practice**

Includi una descrizione per ogni elemento di una coda di richiesta: il progetto della coda di richiesta, i gruppi di argomenti, gli argomenti della coda e le regole di indirizzamento.

**Ecco perché**

Le descrizioni consentono agli amministratori di gruppo, ai futuri amministratori di sistema o a altri utenti che mantengono le code di richiesta di sapere esattamente cosa fa ogni parte della coda di richiesta.

Le informazioni di descrizione vengono visualizzate anche quando passi il cursore sull’icona delle informazioni sul campo nella nuova finestra di richiesta.

La descrizione non deve essere lunga, ma può contenere solo un breve commento sullo scopo o sull’utilizzo dell’elemento.

</br>
</br>

**Best practice**

Crea uno stato di progetto denominato &quot;Coda richieste&quot; o &quot;Operativo&quot; che equivale a &quot;Corrente&quot; per distinguere i progetti in coda richieste da altri progetti.

**Ecco perché**

Una coda di richiesta &quot;vive&quot; in un progetto e deve essere in uno stato uguale a Corrente affinché la coda sia attiva.

Per distinguere una richiesta da progetti di lavoro effettivi con stato &quot;Current&quot; (Corrente), creare uno stato da utilizzare solo nelle code di richiesta denominate &quot;Request Queue&quot; (Coda richieste) o &quot;Operations&quot; (Operativo). Puoi quindi utilizzare questo stato per escludere o includere progetti nella coda delle richieste durante la scrittura di rapporti.

</br>
</br>

**Best practice**

Crea uno stato di problema denominato &quot;Rifiutato&quot; quando utilizzi le approvazioni dei problemi e imposta l&#39;opzione Se rifiutato sullo stato &quot;Rifiutato&quot;.

**Ecco perché**

Utilizzando uno stato &quot;Rifiutato&quot;, questo chiarisce che la richiesta è stata rivista e rifiutata.

</br>
</br>

**Best practice**

Assegna moduli personalizzati &quot;universali&quot; per richiedere code per acquisire il maggior numero possibile di dati coerenti a livello aziendale.

**Ecco perché**

Un modulo personalizzato &quot;universale&quot; raccoglie le informazioni standard necessarie per la richiesta, indipendentemente dal tipo di richiesta inviata.

L’uso di un modulo personalizzato &quot;universale&quot; consente di ridurre il numero di moduli personalizzati da creare e gestire. Inoltre, garantisce che tutte le richieste raccolgano le stesse informazioni allo stesso modo, il che porta a rapporti e analisi dei dati coerenti.

</br>
</br>

**Best practice**

Evita di condividere le code di richiesta con &quot;tutti&quot;.  Imposta le impostazioni dei dettagli della coda in modo che gli utenti vedano solo le code pertinenti in base alle loro esigenze.

**Ecco perché**

Nella maggior parte dei casi, una coda di richiesta deve essere condivisa solo con un determinato gruppo di persone come un team, un fornitore, clienti, ecc. Quando i richiedenti visualizzano solo ciò di cui hanno bisogno nell’elenco della coda delle richieste, è facile trovare e navigare.

</br>
</br>


**Best practice**

Crea e assegna un dashboard contenente i rapporti sulla coda delle richieste in modo che i responsabili del traffico, gli amministratori di sistema o gli utenti assegnati possano lavorare direttamente sui problemi.

**Ecco perché**

Consentire agli utenti di accedere in modo rapido e semplice alle richieste in arrivo significa che il lavoro non viene perso nel miscuglio.

</br>
</br>

**Best practice**

Utilizza i modelli di layout per rimuovere le opzioni di configurazione della coda di richiesta dal menu del pannello a sinistra dei progetti per gli utenti che non hanno bisogno di creare code.


**Ecco perché**

In questo modo tutte le code di richiesta passano attraverso il processo di creazione corretto (ad esempio, vengono esaminate da un comitato di governance) e vengono configurate correttamente da un amministratore di sistema o di gruppo.

Inoltre, questo consente di mantenere l’elenco delle code organizzato e concentrato sui tipi di richieste necessari alla tua organizzazione.

</br>
</br>

**Best practice**

Crea una coda di richiesta dell’amministratore di sistema per consentire agli utenti di porre domande relative a Workfront, effettuare richieste relative alle impostazioni di sistema, pianificare nuovi corsi di formazione per gli utenti, ecc.

**Ecco perché**

Questo fornisce una posizione centralizzata in cui gli utenti possono inviare domande e consentire agli amministratori di raccogliere, monitorare e rispondere ai problemi relativi a Workfront.

Inoltre, queste informazioni possono essere utilizzate per mostrare al leadership il tempo, lo sforzo e il valore del ruolo di amministratore di sistema e come giustificazione per un amministratore di sistema aggiuntivo.

</br>
</br>


**Best practice**

Controlla regolarmente le code di richiesta per identificare e annullare la condivisione delle code che non vengono utilizzate.

**Ecco perché**

Un controllo regolare delle impostazioni e degli elementi nel sistema Adobe Workfront consente di mantenerli privi di vincoli e privi di elementi non necessari. Se una coda non viene più utilizzata o monitorata, assicurati che gli utenti non possano più accedervi, in modo che le richieste di lavoro non cadano in un vuoto.

</br>
</br>


**Best practice**

Utilizza i gruppi di argomenti per organizzare più di 10 argomenti della coda in una coda di richiesta per creare elenchi più brevi e facili da gestire.

**Ecco perché**

I gruppi di argomenti aumentano l&#39;adozione degli utenti e creano meno confusione riducendo l&#39;elenco iniziale di opzioni tra cui selezionare. Questo consente agli utenti di trovare facilmente ciò che stanno cercando senza sovraccaricarli quando tentano di inviare una richiesta.

Inoltre, consente agli amministratori di sistema e/o ai gestori delle code di creare un percorso di navigazione fluido per gli utenti e un modo migliore per organizzare e creare rapporti sui tipi di richieste inviate.

</br>
</br>

**Best practice**

Controlla il numero totale di code di richiesta disponibili agli utenti suddividendo una coda di richiesta utilizzando gruppi di argomenti e argomenti della coda, anziché creare più code.

**Ecco perché**

Troppe code di richiesta rendono difficile agli utenti trovare ciò di cui hanno bisogno.

Il minor numero di code aiuta anche i coordinatori del traffico, gli amministratori di sistema o altri utenti che gestiscono le code, consentendo loro di trovare le informazioni necessarie più rapidamente, senza dover passare a più progetti di coda delle richieste.

Crea più code di richiesta se è necessario un accesso diverso per code di richiesta diverse o se il consolidamento delle code confonderebbe gli utenti.

</br>
</br>

**Best practice**

Imposta le regole di routing per ogni argomento della coda. Come minimo, impostare una regola di routing predefinita.

**Ecco perché**

Le regole di instradamento assicurano che a qualcuno venga sempre assegnata la richiesta in arrivo in modo che il lavoro non cada attraverso le fessure.

</br>
</br>

**Best practice**

Sfrutta i gruppi di argomenti e gli argomenti della coda quando è necessario indirizzare selettivo.

**Ecco perché**

Impossibile applicare le regole di instradamento ai campi di un modulo personalizzato. Quindi, se diversi tipi di richieste devono essere indirizzati a diversi team/singoli utenti, fai in modo che ogni tipo di richiesta sia indirizzato correttamente al proprio gruppo di argomenti/argomento della coda.

</br>
</br>

**Best practice**

Indirizza le richieste a un team, anziché a un singolo utente.

**Ecco perché**

Quando le richieste vengono inviate al team, l&#39;intero team può visualizzare le richieste che vengono effettuate e quali potrebbero essere le conseguenze del lavoro in corso. Tutti possono guardare la pagina Team per individuare nuovi elementi o tenere traccia delle novità di un report su un dashboard.

Inoltre, quando il gestore del traffico o un’altra persona incaricata di rivedere o assegnare le richieste in arrivo non è disponibile, viene automaticamente disponibile un backup che consente di accedere alle informazioni richieste.
