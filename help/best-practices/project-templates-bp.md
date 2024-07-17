---
title: Best practice - Modelli di progetto
description: Esplora i consigli sulle best practice forniti dagli esperti di Adobe Workfront in merito all’impostazione, alla gestione e all’utilizzo dei modelli di progetto in Workfront.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
jira: KT-10919
exl-id: 17cd2e49-ee16-4b80-a8b2-ccc254fa8014
source-git-commit: d39151288d8b749940c5183063392ee471769445
workflow-type: tm+mt
source-wordcount: '1743'
ht-degree: 100%

---

# Best practice - Modelli di progetto

## Che cos’è una “best practice” di Adobe Workfront?

Le best practice sono linee guida che rappresentano una linea d’azione efficace ed efficiente; sono facilmente adottabili da te e dagli utenti della tua azienda; e possono essere replicate con successo in tutta l’organizzazione.

Mentre esamini questi consigli, tieni presente che alcune best practice di Workfront sono universali mentre altre potrebbero essere più specifiche per un dato argomento. Utilizza queste best practice come una base comune per le impostazioni e l’utilizzo del sistema Workfront.

## Esplorazione di questa pagina

Scorrendo questa pagina, troverai innanzitutto un elenco di alto livello di tutte le best practice relative all’argomento. Questo ti consente di rivedere i consigli senza immergerti nei dettagli delle motivazioni.

“Perché queste sono best practice?” che si trova dopo l’elenco di alto livello, fornisce maggiori dettagli su alcune delle best practice e sul motivo per cui sono considerate un processo, uno strumento ecc. da implementare con la tua istanza di Workfront.

</br>
</br>

## Best practice per i modelli di progetto

* Utilizza i modelli per creare progetti.

* Stabilisci una convenzione di denominazione per i modelli di progetto.

* Stabilisci un gruppo selezionato di utenti che possono creare e aggiornare modelli di progetto.

* Utilizza la condivisione di progetti in un modello di progetto per concedere automaticamente l’accesso ai progetti creati utilizzando tale modello.

* Assegna mansioni o team alle attività, non singoli utenti.

* Evita di essere troppo granulare quando crei attività in un modello di progetto. Limita il numero di attività in un modello di progetto a quelle necessarie per completare il lavoro.

* Utilizza la descrizione dell’attività per acquisire i piccoli passaggi dell’attività, anziché suddividerla in più attività.

* Assicurati che le attività del modello includano le durate delle attività, le ore pianificate e i predecessori.

* Preconfigura i dettagli del progetto e allega i moduli personalizzati al modello.

* Rivedi e aggiorna regolarmente i modelli di progetto.

* Controlla i modelli per assicurarti che contengano tutte le informazioni necessarie prima di condividerli e che altri utenti inizino a utilizzarli.

* Quando modifichi l’opzione Pianifica da in un modello, esamina e aggiorna i vincoli dell’operazione.

* Controlla il team del progetto sul modello e rimuovi gli utenti che non saranno associati al progetto.

</br>
</br>

## Perché queste sono best practice?

**Best practice**

Utilizza i modelli per creare progetti.

**Ecco perché**

I modelli di progetto eliminano le supposizioni dei project manager (e di altri utenti che creano progetti) sulle attività da includere in un progetto, su come strutturare la timeline e così via. I modelli sono il modo più efficace per accelerare la creazione del progetto.

È importante sottolineare che i modelli forniscono coerenza tra progetti di tipo simile, in modo che persone, processi e punti dati siano sempre dettagliati nello stesso modo. Anche i progetti con tempi di esecuzione rapidi (uno o due giorni) e attività minime possono trarre vantaggio dalla creazione di modelli di progetto.

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

Disporre di modelli di progetto coerenti e ben strutturati è fondamentale per una buona gestione del lavoro e per un reporting accurato. Limita il numero di utenti che possono modificare i modelli per evitare modifiche accidentali o non approvate.

</br>
</br>

**Best practice**

Utilizza la condivisione di progetti in un modello di progetto per concedere automaticamente l’accesso ai progetti creati utilizzando tale modello.

**Ecco perché**

L’accesso a progetti specifici è concesso attraverso il progetto stesso. Se lo stesso gruppo di persone ha sempre bisogno di accedere ai progetti creati con un modello specifico, aggiungi tali persone nel modello sotto l’opzione Condivisione progetto. Non solo è possibile controllare l’accesso ai progetti non appena vengono creati, ma questo semplifica gli sforzi di scalabilità nel caso in cui le autorizzazioni debbano essere modificate in futuro.

Per istruzioni su come condividere i progetti creati utilizzando un modello, consulta il capitolo “Come condividere i progetti creati utilizzando un modello” in [Condividere un modello di progetto](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/manage-work/create-and-manage-project-templates/share-a-project-template.html?lang=it).

**Nota**: la condivisione del modello garantisce l’accesso al modello stesso. Per creare progetti con il modello, l’utente deve disporre almeno delle autorizzazioni di visualizzazione.

</br>
</br>

**Best practice**

Assegna mansioni o team alle attività, non singoli utenti.

**Ecco perché**

Quando un singolo utente cambia posizione o lascia l’organizzazione, dovrai aggiornare manualmente i modelli di progetto che includono tale persona. Questa operazione richiede tempo da parte degli amministratori di sistema o di gruppo, oppure dei project manager.

Se utilizzi mansioni o team sui modelli, le modifiche al personale non avranno alcun effetto diretto sui modelli di progetto, perché chiunque venga assegnato a quella mansione o a quel team potrebbe essere incaricato del lavoro. Ciò aiuta a garantire che il lavoro non vada perduto. Le assegnazioni della mansione semplificano anche l’assegnazione del lavoro ai singoli utenti, in quanto Workfront è in grado di mostrare un elenco di persone assegnate a una determinata mansione.

Inoltre, le mansioni vengono utilizzate dagli strumenti di pianificazione delle risorse di Workfront per consentire di calcolare le risorse necessarie e pianificare il lavoro futuro.

</br>
</br>

**Best practice**

Evita di essere troppo granulare quando crei attività in un modello di progetto. Limita il numero di attività in un modello di progetto a quelle necessarie per completare il lavoro.

**Ecco perché**

I modelli di progetto eccessivamente complicati comportano un’esperienza negativa per gli utenti: project manager, responsabili risorse, membri del team e altri ancora. Un numero eccessivo di attività rende difficile la gestione della timeline del progetto, con scadenze di attività che si sovrappongono e più attività che vengono assegnate alle stesse mansioni o ai singoli utenti.


</br>
</br>

**Best practice**

Utilizza la descrizione dell’attività per acquisire i piccoli passaggi dell’attività, anziché suddividerla in più attività.

**Ecco perché**

Se più attività consecutive vengono assegnate alla stessa mansione/utente, ciò indica che tali attività potrebbero essere combinate. Assegnare troppe attività a un utente potrebbe fargli percepire un aumento del carico di lavoro, cosa che potrebbe indurlo ad adottare Workfront.

</br>
</br>

**Best practice**

Assicurati che le attività del modello includano le durate delle attività, le ore pianificate e i predecessori.

**Ecco perché**

Questi tre aspetti (durate, ore pianificate e predecessori) sono gli elementi costitutivi della timeline del progetto. Questi sono fondamentali per sapere quanto tempo richiederà il lavoro e quando dovrà essere svolto. Gli strumenti di gestione delle risorse di Workfront utilizzano durate e ore pianificate, oltre alle assegnazioni di ruoli, per calcolare la capacità delle risorse, la disponibilità e altro ancora.

Se non hai la certezza di come stimare le durate o le ore pianificate per la prima volta, collabora con il team del progetto per definire alcune stime iniziali. Una volta utilizzato il modello, incontra nuovamente il team del progetto per determinare dove potrebbero essere apportate modifiche per rendere il modello più accurato. Se gli utenti registrano il tempo in Workfront, puoi confrontare le ore pianificate di un progetto con le ore effettive, per vedere dove è necessario apportare delle modifiche.


</br>
</br>

**Best practice**

Preconfigura i dettagli del progetto e allega i moduli personalizzati al modello.

**Ecco perché**

Assicurati che le informazioni standard per tutti i progetti siano inserite nel modello di progetto. Questo non solo contribuisce ad accelerare la creazione dei progetti, ma anche la disponibilità delle informazioni necessarie e la coerenza tra i diversi progetti.

Allega i moduli personalizzati del progetto che corrispondono ai moduli personalizzati della richiesta per richiamare le informazioni inviate quando si converte la richiesta in un progetto utilizzando il modello.

Per istruzioni su come allegare un modulo personalizzato a un oggetto, ad esempio un modello di progetto, consulta [Allegare un modulo personalizzato a un oggetto](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/custom-data/custom-forms/custom-forms-using-a-custom-form.html?lang=it).

</br>
</br>

**Best practice**

Rivedi e aggiorna regolarmente i modelli di progetto.

**Ecco perché**

Man mano che i processi e i team cambiano, i modelli del progetto dovrebbero essere aggiornati. Stabilisci una cadenza regolare, ad esempio trimestrale, per controllare e constatare quali modelli non vengono utilizzati attivamente. Puoi disattivarli, in modo che siano ancora presenti in Workfront ma non vengano visualizzati negli elenchi di selezione dei modelli.

Per istruzioni su come disattivare un modello di progetto, consulta [Disattivare un modello di progetto](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/manage-work/create-and-manage-project-templates/deactivate-a-project-template.html?lang=it).

</br>
</br>

**Best practice**

Controlla i modelli per assicurarti che contengano tutte le informazioni necessarie prima di condividerli e che altri utenti inizino a utilizzarli.


**Ecco perché**

Poiché i modelli verranno utilizzati più e più volte per realizzare progetti, assicurati che tutto sia impostato correttamente e completamente. Ciò garantisce coerenza tra tutti i progetti e dati accurati, per la generazione dei rapporti.

Oltre alle impostazioni delle attività, come la durata e le ore pianificate, di seguito sono riportati alcuni aspetti da rivedere prima di condividere i modelli:

* Impostazione Pianifica da
* Vincoli delle attività
* Proprietario del progetto, sponsor, gruppo e azienda
* Portfolio e programma
* Percorso milestone e passaggi
* Processi di approvazione
* Assicurati che gli utenti assegnati alle attività sui progetti possano accedere al progetto in modalità “Contribuisci”.
* Gruppi di risorse
* Notifiche promemoria
* Pianificazione
* Impostazione valuta (se applicabile)
* Allega documenti standard
* Allega moduli doganali necessari
* Controlla il team del progetto per assicurarti che non vi siano assegnate altre persone

</br>
</br>

**Best practice**

Quando modifichi l’opzione Modalità di pianificazione su un modello, esamina e aggiorna i vincoli dell’attività.

**Ecco perché**

La combinazione di vincoli di attività diversi in un progetto può causare imprevisti e confusione nel calcolo delle date pianificate. Ad esempio, se per l’opzione Modalità di pianificazione è selezionata l’opzione Data inizio, per impostazione predefinita, a tutte le attività create nel progetto viene assegnato il vincolo attività Il prima possibile. Se in seguito passi dall’opzione Modalità di pianificazione a Data di completamento, per impostazione predefinita, tutte le attività create avranno un vincolo attività Il più tardi possibile. Una combinazione non intenzionale di attività con ciascuno di questi vincoli può causare confusione nelle date pianificate della sequenza temporale del progetto.

Per comprendere meglio i vincoli delle attività e come utilizzarli, consulta [Comprendere e gestire i tipi di durata e i vincoli delle attività](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/manage-work/intermediate-projects/understand-and-manage-duration-types-and-task-constraints.html?lang=it).

</br>
</br>

**Best practice**

Controlla il team del progetto sul modello e rimuovi gli utenti che non lavoreranno con il progetto.

**Ecco perché**

Quando crei un modello da un progetto esistente, a meno che non scegli l’opzione Cancella assegnazioni durante la creazione, Workfront richiama le persone a cui sono state assegnate attività/problemi sul progetto nella sezione Persone. Quando si lavora con il modello, è possibile rimuovere le persone a cui era stato precedentemente assegnato un lavoro o modificare un’assegnazione creata personalmente sul modello.

Tutti questi utenti verranno elencati come parte del team del progetto, nelle sezioni Persone e Pianificazione del progetto. Di conseguenza, verranno propagati a tutti i progetti creati da tale modello. Questo potrebbe causare confusione per l’utente, perché come parte del team di progetto, riceve le notifiche sull’attività del progetto, visualizza il progetto nell’elenco Progetti che mi interessano e ottiene le autorizzazioni per il progetto e le attività, i problemi e i documenti relativi.

Per istruzioni su come modificare il team di progetto in un modello di progetto, consulta [Modificare il team di progetto in un modello di progetto](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/manage-work/create-and-manage-project-templates/edit-the-project-team-in-a-project-template.html?lang=it).
