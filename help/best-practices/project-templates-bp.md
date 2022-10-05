---
title: Procedure consigliate - Modelli di progetto
description: Scopri le best practice consigliate dagli esperti Adobe Workfront sull’impostazione, la gestione e l’utilizzo dei modelli di progetto Workfront.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
kt: 10919
exl-id: 17cd2e49-ee16-4b80-a8b2-ccc254fa8014
source-git-commit: 444f059d3cc26d8e3074a7145bc5419407c786cf
workflow-type: tm+mt
source-wordcount: '1614'
ht-degree: 0%

---

# Procedure consigliate - Modelli di progetto

## Qual è una &quot;best practice&quot; di Adobe Workfront?

Le migliori pratiche sono linee guida che rappresentano un&#39;azione efficace ed efficiente; sono facilmente adottati da te e dagli utenti della tua azienda; e può essere replicato correttamente in tutta l’organizzazione.

Quando si esaminano queste raccomandazioni, tenere presente che alcune best practice di Workfront sono universali, mentre altre potrebbero essere più specifiche per l’argomento. Utilizza queste best practice come framework per guidare le impostazioni e l’utilizzo del sistema Workfront.

## Navigazione in questa pagina

Scorrendo questa pagina, troverai innanzitutto un elenco di alto livello contenente tutte le best practice per l’argomento. Questo ti consente di rivedere le raccomandazioni senza immergerti nei dettagli del &quot;perché&quot;.

Perché queste best practice? area, disponibile dopo l’elenco di alto livello, fornisce maggiori dettagli su alcune delle best practice e sui motivi per cui vengono considerate un processo, uno strumento, ecc., dovresti considerare l’implementazione con la tua istanza Workfront.

</br>
</br>

## Best practice per i modelli di progetto

* Utilizza i modelli durante la creazione di progetti.

* Stabilisci una convenzione di denominazione per i modelli di progetto.

* Stabilisci un gruppo selezionato di utenti che possono creare e aggiornare modelli di progetto.

* Utilizza Condivisione progetti in un modello di progetto per concedere automaticamente l’accesso ai progetti creati utilizzando tale modello.

* Assegnare ruoli o team di lavoro alle attività, non a singoli utenti.

* Evita di diventare troppo granulare durante la creazione di attività in un modello di progetto. Limita il numero di attività in un modello di progetto a quelle necessarie per completare il lavoro.

* Utilizzare la descrizione dell&#39;attività per acquisire i piccoli passaggi dell&#39;attività, anziché suddividerla in più attività.

* Assicurati che le attività del modello includano le durate delle attività, le ore pianificate e i predecessori.

* Preconfigurare i dettagli del progetto e allegare moduli personalizzati al modello.

* Revisione periodica e aggiornamento dei modelli di progetto.

* Controlla i modelli per assicurarti che abbiano tutte le informazioni necessarie prima di condividerle e che altri inizino a utilizzarle.

* Quando si regola l&#39;opzione Pianifica da in un modello, esaminare e aggiornare i vincoli dell&#39;attività.

* Controlla il team del progetto nel modello e rimuovi gli utenti che non saranno associati al progetto.

</br>
</br>

## Perché queste best practice sono?

**Best practice**

Utilizza i modelli durante la creazione di progetti.

**Ecco perché**

I modelli di progetto evitano le supposizioni dei project manager (e di altri che creano progetti) relative alle attività che un progetto deve contenere, alla struttura della timeline e così via. I modelli sono il modo più efficace per accelerare la creazione dei progetti.

È importante notare che i modelli forniscono coerenza tra progetti di tipi simili, in modo che le persone, i processi e i punti dati siano sempre descritti nello stesso modo. Anche i progetti con modifiche rapide (uno o due giorni) e le attività minime possono trarre vantaggio dalla creazione con modelli di progetto.

Questa coerenza tra i progetti consente di ottenere dati più precisi, fondamentale quando si prendono decisioni per il team, il reparto e l’organizzazione.

</br>
</br>

**Best practice**

Stabilisci una convenzione di denominazione per i modelli di progetto.

**Ecco perché**

La denominazione coerente semplifica la ricerca dei modelli. Inoltre, consente ai project manager e agli altri utenti che creano progetti di selezionare il modello corretto quando sono presenti modelli con nomi simili tra più team o dipartimenti.

</br>
</br>

**Best practice**

Stabilisci un gruppo selezionato di utenti che possono creare e aggiornare modelli di progetto.

**Ecco perché**

L’utilizzo di modelli di progetto coerenti e ben costruiti è fondamentale per una buona gestione del lavoro e per un reporting accurato. Limita il numero di utenti che possono modificare i modelli per evitare modifiche accidentali o non approvate.

</br>
</br>

**Best practice**

Utilizza Condivisione progetti in un modello di progetto per concedere automaticamente l’accesso ai progetti creati utilizzando tale modello.

**Ecco perché**

L&#39;accesso a progetti specifici è concesso attraverso il progetto stesso. Se lo stesso gruppo di persone deve sempre accedere ai progetti creati con un modello specifico, aggiungili nell’opzione Condivisione progetti nel modello. Non solo puoi controllare l’accesso ai progetti non appena vengono creati, ma ottimizza anche le attività di scalabilità in caso di necessità di modificare le autorizzazioni in futuro.

**Nota**: La condivisione di modelli consente l’accesso al modello stesso. Per creare progetti con il modello, un utente deve disporre almeno delle autorizzazioni di visualizzazione.

</br>
</br>

**Best practice**

Assegnare ruoli o team di lavoro alle attività, non a singoli utenti.

**Ecco perché**

Quando un singolo utente cambia posizione o lascia l&#39;organizzazione, dovrai aggiornare manualmente i modelli di progetto che includono tale persona. Questo richiede tempo da parte degli amministratori di sistema o di gruppo o dei project manager.

Se si utilizzano ruoli di lavoro o team nei modelli, le modifiche al personale non avranno un effetto diretto sui modelli di progetto, perché a tutti gli utenti a cui è stato assegnato quel ruolo o a quel team potrebbe essere assegnato il lavoro. Questo aiuta a garantire che il lavoro non scivoli attraverso le fessure. Le assegnazioni dei ruoli di lavoro facilitano inoltre l&#39;assegnazione del lavoro ai singoli utenti, in quanto Workfront può mostrare un elenco di persone a cui è stato assegnato quel ruolo di lavoro.

Inoltre, i ruoli di lavoro vengono utilizzati dagli strumenti di pianificazione delle risorse di Workfront per consentire di calcolare le risorse necessarie e pianificare il lavoro futuro.

</br>
</br>

**Best practice**

Evita di diventare troppo granulare durante la creazione di attività in un modello di progetto. Limita il numero di attività in un modello di progetto a quelle necessarie per completare il lavoro.

**Ecco perché**

I modelli di progetto eccessivamente complicati causano un’esperienza negativa per gli utenti: project manager, gestori di risorse, membri del team e altro ancora. Troppe attività rendono difficile gestire la timeline del progetto, con scadenze sovrapposte e più attività assegnate agli stessi ruoli o singoli utenti.


</br>
</br>

**Best practice**

Utilizzare la descrizione dell&#39;attività per acquisire i piccoli passaggi dell&#39;attività, anziché suddividerla in più attività.

**Ecco perché**

Se più attività di una riga vengono assegnate allo stesso ruolo/singolo processo, ciò indica che tali attività possono essere combinate. Avere troppe attività assegnate a un utente può far sentire loro che c&#39;è più lavoro da completare, che può influenzare l&#39;adozione di Workfront.

</br>
</br>

**Best practice**

Assicurati che le attività del modello includano le durate delle attività, le ore pianificate e i predecessori.

**Ecco perché**

Questi tre elementi, le durate, le ore pianificate e i predecessori, sono gli elementi costitutivi della cronologia del progetto. Sono fondamentali per sapere quanto tempo ci vorrà e quando sarà necessario fare. Le durate e le ore pianificate degli strumenti di gestione delle risorse di Workfront, oltre alle assegnazioni dei ruoli, consentono di calcolare la capacità delle risorse, la disponibilità e altro ancora.

Se non sei sicuro di come stimare le durate o le ore pianificate per la prima volta, collabora con il team del progetto per definire alcune stime iniziali. Una volta utilizzato il modello, incontra nuovamente il team del progetto per determinare dove è possibile apportare modifiche per rendere il modello più preciso. Se gli utenti accedono a Workfront, puoi confrontare le ore pianificate di un progetto con le ore effettive per vedere dove sono necessarie le modifiche.


</br>
</br>

**Best practice**

Preconfigurare i dettagli del progetto e allegare moduli personalizzati al modello.

**Ecco perché**

Assicurati che le informazioni standard per tutti i progetti siano inserite nel modello di progetto. Questo aiuta non solo ad accelerare la creazione del progetto, ma garantisce che le informazioni necessarie siano disponibili e che siano coerenti tra i progetti.

Allega moduli personalizzati del progetto che corrispondono a moduli personalizzati della richiesta per estrarre le informazioni inviate durante la conversione della richiesta in un progetto utilizzando il modello.

</br>
</br>

**Best practice**

Revisione periodica e aggiornamento dei modelli di progetto.

**Ecco perché**

Man mano che i processi e i team cambiano, i modelli di progetto devono essere aggiornati. Stabilisci una cadenza regolare, ad esempio trimestrale, per verificare e vedere quali modelli non vengono utilizzati attivamente. Puoi disattivarli, in modo che siano ancora in Workfront ma non vengano visualizzati negli elenchi di selezione dei modelli.

</br>
</br>

**Best practice**

Controlla i modelli per assicurarti che abbiano tutte le informazioni necessarie prima di condividerle e che altri inizino a utilizzarle.


**Ecco perché**

Poiché i modelli verranno utilizzati più volte per creare progetti, dovrai accertarti che tutto sia configurato correttamente e completamente. Questo porta alla coerenza tra tutti i progetti e a dati precisi per la generazione di rapporti.

Oltre alle impostazioni delle attività, come la durata e le ore pianificate, alcuni elementi da rivedere prima di condividere i modelli includono:

* Impostazione di Pianificazione da
* Vincoli dell’attività
* Proprietario del progetto, sponsor, gruppo e azienda
* Portfolio e programma
* Percorso e passaggi Milestone
* Processi di approvazione
* Assicurati che gli utenti con attività assegnate ai progetti abbiano accesso al progetto tramite Contribute
* Gruppi di risorse
* Notifiche promemoria
* Pianificazione
* Impostazione della valuta (se applicabile)
* Allega documenti standard
* Allegare i moduli doganali necessari
* Controlla il team del progetto per assicurarti che non ci siano più persone assegnate

</br>
</br>

**Best practice**

Quando si regola l&#39;opzione Pianifica da in un modello, esaminare e aggiornare i vincoli dell&#39;attività.

**Ecco perché**

La combinazione di vincoli di attività diversi in un progetto può causare calcoli di data pianificati imprevisti e confusi. Ad esempio, se per l&#39;opzione Pianifica da è selezionata la data di inizio, a tutte le attività create in quel progetto viene assegnato per impostazione predefinita il vincolo di attività Al più presto possibile. Se in seguito si passa all&#39;opzione Pianificazione da a Data completamento, per impostazione predefinita tutte le attività create avranno un vincolo di attività Più tardi possibile. La combinazione involontaria di attività con ciascuno di questi vincoli può causare la confusione delle date pianificate nella timeline del progetto.


</br>
</br>

**Best practice**

Controlla il team del progetto nel modello e rimuovi gli utenti che non lavoreranno con il progetto.

**Ecco perché**

Quando crei un modello da un progetto esistente, questo include le persone a cui sono stati assegnati compiti/problemi sul progetto. Mentre lavori con il modello, puoi rimuovere le persone a cui era stato assegnato un lavoro in precedenza o modificare un&#39;assegnazione che hai creato tu stesso sul modello.

Tutti questi utenti saranno elencati come parte del team del progetto, nelle sezioni Persone e Pianificazione del progetto. Di conseguenza, verranno propagati a tutti i progetti creati da quel modello. Questo potrebbe creare confusione per l’utente, perché, come parte del team del progetto, riceve notifiche sull’attività del progetto, vede il progetto nell’elenco Progetti in corso e ottiene le autorizzazioni per il progetto e le sue attività, problemi e documenti.
