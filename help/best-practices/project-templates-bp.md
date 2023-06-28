---
title: Best practice - Modelli di progetto
description: Esplora i consigli sulle best practice forniti dagli esperti Adobe Workfront in merito all’impostazione, alla gestione e all’utilizzo dei modelli di progetto Workfront.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
jira: KT-10919
exl-id: 17cd2e49-ee16-4b80-a8b2-ccc254fa8014
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '1614'
ht-degree: 0%

---

# Best practice - Modelli di progetto

## Cos’è una &quot;best practice&quot; di Adobe Workfront?

Le best practice sono linee guida che rappresentano una linea di condotta efficace ed efficiente, sono facilmente adottabili da te e dagli utenti della tua azienda e possono essere replicate correttamente all’interno dell’organizzazione.

Mentre esamini questi consigli, tieni presente che alcune best practice di Workfront sono universali, mentre altre potrebbero essere più specifiche per l’argomento. Utilizza queste best practice come framework per guidare le impostazioni e l’utilizzo del sistema Workfront.

## Navigazione in questa pagina

Scorrendo questa pagina, troverai innanzitutto un elenco di alto livello di tutte le best practice per l’argomento. Questo ti consente di rivedere i consigli senza immergerti nei dettagli di &quot;perché&quot;.

La sezione &quot;Perché sono queste best practice?&quot; , disponibile dopo l’elenco di alto livello, fornisce maggiori dettagli su alcune delle best practice e sul perché sono considerate un processo, uno strumento, ecc., è consigliabile implementarle con l’istanza di Workfront.

</br>
</br>

## Best practice per i modelli di progetto

* Utilizza i modelli per creare progetti.

* Stabilisci una convenzione di denominazione per i modelli di progetto.

* Stabilisci un gruppo selezionato di utenti che possono creare e aggiornare modelli di progetto.

* Utilizzare la condivisione di progetti in un modello di progetto per concedere automaticamente l&#39;accesso ai progetti creati utilizzando tale modello.

* Assegna mansioni o team alle attività, non singoli utenti.

* Evitare di diventare troppo granulari durante la creazione di attività in un modello di progetto. Limitare il numero di attività in un modello di progetto a quelle necessarie per completare il lavoro.

* Utilizzare la descrizione dell&#39;attività per acquisire i piccoli passaggi dell&#39;attività, anziché suddividerla in più attività.

* Assicurati che le attività modello includano le durate delle attività, le ore pianificate e i predecessori.

* Preconfigura i dettagli del progetto e allega i moduli personalizzati al modello.

* Rivedere e aggiornare regolarmente i modelli di progetto.

* Controlla i modelli per assicurarti che contengano tutte le informazioni necessarie prima di condividerli e che altri utenti inizino a utilizzarli.

* Quando si modifica l&#39;opzione Pianifica da in un modello, esaminare e aggiornare i vincoli dell&#39;operazione.

* Controlla il team del progetto sul modello e rimuovi gli utenti che non saranno associati al progetto.

</br>
</br>

## Perché si tratta di procedure ottimali?

**Best practice**

Utilizza i modelli per creare progetti.

**Ecco perché**

I modelli di progetto eliminano le supposizioni dei project manager (e di altri utenti che creano progetti) sulle attività da includere in un progetto, su come strutturare la sequenza temporale e così via. I modelli sono il modo più efficace per accelerare la creazione del progetto.

È importante sottolineare che i modelli forniscono coerenza tra progetti di tipo simile, in modo che persone, processi e punti dati siano sempre dettagliati nello stesso modo. Anche i progetti con tempi di esecuzione rapidi (uno o due giorni) e attività minime possono trarre vantaggio dalla creazione con i modelli di progetto.

Questa coerenza tra i progetti consente di ottenere dati più precisi, fondamentale quando si prendono decisioni per il team, il reparto e l’organizzazione.

</br>
</br>

**Best practice**

Stabilisci una convenzione di denominazione per i modelli di progetto.

**Ecco perché**

La denominazione coerente semplifica la ricerca dei modelli. Consente inoltre ai project manager e agli altri utenti che creano progetti di selezionare il modello corretto quando esistono modelli con nomi simili in più team o reparti.

</br>
</br>

**Best practice**

Stabilisci un gruppo selezionato di utenti che possono creare e aggiornare modelli di progetto.

**Ecco perché**

Disporre di modelli di progetto coerenti e ben strutturati è fondamentale per una buona gestione del lavoro e per una creazione di rapporti accurata. Limita il numero di utenti che possono modificare i modelli per evitare modifiche accidentali o non approvate.

</br>
</br>

**Best practice**

Utilizzare la condivisione di progetti in un modello di progetto per concedere automaticamente l&#39;accesso ai progetti creati utilizzando tale modello.

**Ecco perché**

L&#39;accesso a progetti specifici è concesso attraverso il progetto stesso. Se lo stesso gruppo di persone ha sempre bisogno di accedere ai progetti creati con un modello specifico, aggiungili nell’opzione Condivisione progetto del modello. Non solo è possibile controllare l’accesso ai progetti non appena vengono creati, ma questo semplifica gli sforzi di scalabilità se le autorizzazioni devono essere modificate in futuro.

**Nota**: la condivisione dei modelli consente di accedere al modello stesso. Per creare progetti con il modello, l’utente deve disporre almeno delle autorizzazioni di visualizzazione.

</br>
</br>

**Best practice**

Assegna mansioni o team alle attività, non singoli utenti.

**Ecco perché**

Quando un singolo utente cambia posizione o lascia l’organizzazione, dovrai aggiornare manualmente i modelli di progetto che includono tale persona. Questa operazione richiede tempo da parte degli amministratori di sistema o di gruppo o dei project manager.

Se si utilizzano i ruoli o i team nei modelli, le modifiche all&#39;assegnazione del personale non avranno un effetto diretto sui modelli di progetto, in quanto a chiunque sia stato assegnato tale ruolo o tale team potrebbe essere assegnato il lavoro. Questo aiuta a garantire che il lavoro non scivoli attraverso le fessure. Le assegnazioni dei ruoli semplificano anche l’assegnazione del lavoro ai singoli utenti, in quanto Workfront può mostrarti un elenco di persone assegnate a quel ruolo.

Inoltre, le mansioni vengono utilizzate dagli strumenti di pianificazione delle risorse di Workfront per consentire di calcolare le risorse necessarie e pianificare il lavoro futuro.

</br>
</br>

**Best practice**

Evitare di diventare troppo granulari durante la creazione di attività in un modello di progetto. Limitare il numero di attività in un modello di progetto a quelle necessarie per completare il lavoro.

**Ecco perché**

Modelli di progetto troppo complicati si traducono in una cattiva esperienza per gli utenti: project manager, responsabili delle risorse, membri del team e altro ancora. Troppe attività rendono difficile la gestione della sequenza temporale del progetto, con scadenze sovrapposte e più attività assegnate agli stessi ruoli o singoli utenti.


</br>
</br>

**Best practice**

Utilizzare la descrizione dell&#39;attività per acquisire i piccoli passaggi dell&#39;attività, anziché suddividerla in più attività.

**Ecco perché**

Se più attività in una riga vengono assegnate alla stessa mansione/individuo, ciò indica che tali attività possono essere combinate. Se a un utente sono state assegnate troppe attività, il lavoro da completare potrebbe essergli utile e influire sull’adozione di Workfront.

</br>
</br>

**Best practice**

Assicurati che le attività modello includano le durate delle attività, le ore pianificate e i predecessori.

**Ecco perché**

Questi tre elementi, durate, ore pianificate e predecessori, sono gli elementi costitutivi della cronologia del progetto. Questi sono fondamentali per sapere quanto tempo e quando sarà necessario lavorare. Gli strumenti di gestione delle risorse di Workfront durano e pianificano le ore, oltre alle assegnazioni di mansioni, per calcolare la capacità delle risorse, la disponibilità e altro ancora.

Se non sai come stimare le durate o le ore pianificate per la prima volta, rivolgiti al team di progetto per definire alcune stime iniziali. Dopo aver utilizzato il modello, incontra nuovamente il team del progetto per determinare dove è possibile apportare modifiche per rendere il modello più accurato. Se gli utenti registrano il tempo in Workfront, puoi confrontare le ore pianificate di un progetto con le ore effettive per vedere dove sono necessari gli adeguamenti.


</br>
</br>

**Best practice**

Preconfigura i dettagli del progetto e allega i moduli personalizzati al modello.

**Ecco perché**

Assicurati che le informazioni standard per tutti i progetti siano inserite nel modello di progetto. Questo non solo contribuisce ad accelerare la creazione dei progetti, ma garantisce anche la disponibilità delle informazioni necessarie e la coerenza tra i diversi progetti.

Allega i moduli personalizzati del progetto che corrispondono ai moduli personalizzati della richiesta per richiamare le informazioni inviate quando si converte la richiesta in un progetto utilizzando il modello.

</br>
</br>

**Best practice**

Rivedere e aggiornare regolarmente i modelli di progetto.

**Ecco perché**

Quando i processi e i team cambiano, è necessario aggiornare i modelli di progetto. Stabilisci una cadenza regolare, ad esempio trimestrale, per verificare e vedere quali modelli non vengono utilizzati attivamente. Puoi disattivarli, in modo che siano ancora in Workfront ma non vengano visualizzati negli elenchi di selezione dei modelli.

</br>
</br>

**Best practice**

Controlla i modelli per assicurarti che contengano tutte le informazioni necessarie prima di condividerli e che altri utenti inizino a utilizzarli.


**Ecco perché**

Poiché i modelli verranno utilizzati più volte per creare progetti, assicurati che tutto sia configurato correttamente e completamente. Ciò garantisce coerenza tra tutti i progetti e dati accurati per la generazione dei rapporti.

Oltre alle impostazioni delle attività, come la durata e le ore pianificate, di seguito sono riportati alcuni aspetti da esaminare prima di condividere i modelli:

* Impostazione Schedule From
* Vincoli attività
* Proprietario del progetto, sponsor, gruppo e società
* Portfolio e programma
* Percorso e passaggi di Milestone
* Processi di approvazione
* Assicuratevi che gli utenti assegnati alle attività sui progetti abbiano accesso a Contribute al progetto
* Gruppi di risorse
* Notifiche promemoria
* Pianificazione
* Impostazione della valuta (se applicabile)
* Allega documenti standard
* Allegare i necessari moduli doganali
* Controlla il team del progetto per assicurarti che non siano assegnate altre persone

</br>
</br>

**Best practice**

Quando si modifica l&#39;opzione Pianifica da in un modello, esaminare e aggiornare i vincoli dell&#39;operazione.

**Ecco perché**

La combinazione di vincoli di attività diversi in un progetto può causare calcoli di date pianificati imprevisti e confusi. Ad esempio, se per l&#39;opzione Pianifica da è selezionata l&#39;opzione Data inizio, per impostazione predefinita alle attività create nel progetto viene assegnato il vincolo Attività il più presto possibile. Se in seguito si cambia l&#39;opzione Pianifica da a Data completamento, per impostazione predefinita tutte le attività create presentano un vincolo Attività il più tardi possibile. Una combinazione non intenzionale di attività con ciascuno di questi vincoli può causare confusione nelle date pianificate nella sequenza temporale del progetto.


</br>
</br>

**Best practice**

Controlla il team del progetto sul modello e rimuovi gli utenti che non lavoreranno con il progetto.

**Ecco perché**

Quando crei un modello da un progetto esistente, vengono visualizzate le persone a cui sono state assegnate attività/problemi nel progetto. Quando si lavora con il modello, è possibile rimuovere le persone a cui era stato precedentemente assegnato un lavoro o modificare un&#39;assegnazione creata personalmente sul modello.

Tutti questi utenti verranno elencati come parte del team del progetto, nelle sezioni Persone e pianificazione del progetto. Di conseguenza, verranno propagati a tutti i progetti creati da tale modello. Questo potrebbe causare confusione nell’utente, perché come parte del team di progetto, riceve le notifiche sull’attività sul progetto, visualizza il progetto nell’elenco Progetti a cui appartengo e ottiene le autorizzazioni per il progetto e le relative attività, problemi e documenti.
