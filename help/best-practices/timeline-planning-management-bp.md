---
title: 'Best practice: pianificazione e gestione della timeline'
description: Scopri le best practice consigliate dagli esperti Adobe Workfront sull’impostazione, la gestione e l’utilizzo delle timeline dei progetti in Workfront.
feature: Get Started with Workfront
role: Admin, Leader, User
level: Beginner
kt: 10929
exl-id: 8c18746d-e23a-44d0-b1e3-ebf5ba8d022f
source-git-commit: 444f059d3cc26d8e3074a7145bc5419407c786cf
workflow-type: tm+mt
source-wordcount: '1110'
ht-degree: 0%

---

# Best practice: pianificazione e gestione della timeline

## Qual è una &quot;best practice&quot; di Adobe Workfront?

Le migliori pratiche sono linee guida che rappresentano un&#39;azione efficace ed efficiente; sono facilmente adottati da te e dagli utenti della tua azienda; e può essere replicato correttamente in tutta l’organizzazione.

Quando si esaminano queste raccomandazioni, tenere presente che alcune best practice di Workfront sono universali, mentre altre potrebbero essere più specifiche per l’argomento. Utilizza queste best practice come framework per guidare le impostazioni e l’utilizzo del sistema Workfront.

## Navigazione in questa pagina

Scorrendo questa pagina, troverai innanzitutto un elenco di alto livello contenente tutte le best practice per l’argomento. Questo ti consente di rivedere le raccomandazioni senza immergerti nei dettagli del &quot;perché&quot;.

Perché queste best practice? area, disponibile dopo l’elenco di alto livello, fornisce maggiori dettagli su alcune delle best practice e sui motivi per cui vengono considerate un processo, uno strumento, ecc., dovresti considerare l’implementazione con la tua istanza Workfront.

</br>
</br>

## Best practice di pianificazione e gestione della timeline

* Tutti i progetti completati devono avere uno stato che ne rifletta la completezza.

* Durante la copia di un progetto, impostare lo stato del nuovo progetto su Planning.

* Chiedere agli utenti di registrare il tempo effettivo trascorso sulle attività in modo da poter confrontare le ore effettive con le ore pianificate.

* Utilizza le durate delle attività e i predecessori quando possibile per generare e aggiornare una timeline del progetto, anziché selezionare date di inizio e di completamento specifiche.

* Chiedi agli utenti di aggiornare i loro stati delle attività, la percentuale di completamento e le ore effettive ogni giorno (o su una pianificazione impostata ogni settimana).

* Impostare lo stato del progetto su Planning durante l&#39;aggiornamento del piano di progetto per evitare che le notifiche vengano inviate automaticamente quando vengono apportate modifiche.

* Rimuovi utenti dal team del progetto a cui non è stato assegnato il lavoro nel progetto.

* Posiziona Metriche progetto nella parte superiore del menu del pannello di sinistra per gli utenti che utilizzano principalmente Workfront per visualizzare i dati.


</br>
</br>


## Perché queste best practice sono?

**Best practice**

Tutti i progetti completati devono avere uno stato che ne rifletta la completezza.


**Ecco perché**

Assicurare che tutti i progetti completati abbiano uno stato Completo (o equivalente) mantiene l’istanza Workfront pulita e corrente. Mantenendo gli stati del progetto aggiornati e chiudendoli, gli utenti possono facilmente individuare il lavoro già svolto, in modo da concentrarsi sulle priorità attive. Inoltre, garantisce che i dati dei rapporti relativi a progetti, attività, risorse, ecc. siano accurati.


</br>
</br>

**Best practice**

Durante la copia di un progetto, impostare lo stato del nuovo progetto su Planning.

**Ecco perché**

Lo stato Planning (o un equivalente) impedisce che le notifiche Workfront relative alle assegnazioni, alle modifiche della timeline e così via vengano inviate prima che il progetto sia pronto. Quando copi un progetto, viene visualizzata una finestra di dialogo con le opzioni di progetto; cambia lo stato qui, mentre regoli altre opzioni in modo che i dati non vengano copiati dal progetto originale alla versione copiata.

</br>
</br>

**Best practice**

Chiedere agli utenti di registrare il tempo effettivo trascorso sulle attività in modo da poter confrontare le ore effettive con le ore pianificate.


**Ecco perché**

Sapere quanto tempo ci vuole per eseguire un&#39;attività consente di aggiornare i modelli di progetto per una migliore precisione nella pianificazione dei progetti futuri. Significa anche che le stime delle risorse, utilizzando gli strumenti di gestione delle risorse di Workfront, sono più precise.

</br>
</br>

**Best practice**

Utilizza le durate delle attività e i predecessori quando possibile per generare e aggiornare una timeline del progetto, anziché selezionare date di inizio e di completamento specifiche.

**Ecco perché**

L&#39;utilizzo di durate e predecessori insieme a vincoli di attività flessibili (il più presto possibile e il più tardi possibile) consente modifiche automatiche alla data della timeline che &quot;cascata&quot; attraverso il piano di progetto. Ad esempio, quando la durata di un&#39;attività aumenta di un giorno, viene modificata la data di completamento pianificata dell&#39;attività, che a sua volta modifica le date di completamento delle attività seguenti.

Quando si selezionano date di inizio e di completamento specifiche per le attività, il vincolo dell&#39;attività viene impostato su uno che &quot;blocca&quot; la data (deve iniziare il giorno, deve terminare il giorno, date fisse), il che significa che è necessario eseguire manualmente alcuni aggiornamenti della data della timeline.

</br>
</br>


**Best practice**

Chiedi agli utenti di aggiornare i loro stati delle attività, la percentuale di completamento e le ore effettive ogni giorno (o su una pianificazione impostata ogni settimana).

**Ecco perché**

I rapporti in Workfront sono precisi solo quanto i dati immessi in Workfront. Quando le informazioni che indicano l’avanzamento del lavoro, come lo stato e la percentuale di completamento, non vengono aggiornate regolarmente, i rapporti che mostrano l’avanzamento del lavoro non saranno accurati. L’aggiornamento su base giornaliera garantisce la massima precisione nei dati di reporting in tempo reale.


Lo stato dell’attività viene inoltre utilizzato per informare gli utenti del completamento del lavoro precedente e dell’inizio delle attività. Quando lo stato dell’attività non viene modificato per riflettere l’avanzamento effettivo dell’elemento di lavoro, Workfront non può inviare le notifiche appropriate.

</br>
</br>

**Best practice**

Impostare lo stato del progetto su Planning durante l&#39;aggiornamento del piano di progetto per evitare che le notifiche vengano inviate automaticamente quando vengono apportate modifiche.

**Ecco perché**

Le modifiche apportate al piano di progetto possono generare più notifiche in caso di assegnazioni di attività, date di inizio e di completamento pianificate e altre impostazioni modificate. Questo può creare problemi per gli utenti e creare confusione su assegnazioni, scadenze, ecc.

Lo stato Planning comunica a Workfront di non inviare notifiche sul progetto ai membri del team del progetto (utenti a cui sono stati assegnati compiti/problemi o altri con accesso al progetto) perché il piano di progetto è ancora in fase di sviluppo o il progetto non è ancora pronto per essere live. Una volta completate le modifiche, cambia lo stato del progetto in Corrente e le notifiche vengono inviate. Il seguente processo consente di ridurre al minimo la quantità di notifiche ricevute dagli utenti.

</br>
</br>

**Best practice**

Rimuovi utenti dal team del progetto a cui non è stato assegnato il lavoro nel progetto.


**Ecco perché**

Quando si assegna un&#39;attività o un problema a un progetto, l&#39;utente viene aggiunto all&#39;elenco del team del progetto nelle sezioni Pianificazione e Persone del progetto. Tuttavia, rimangono nell’elenco dei team del progetto anche se sono stati rimossi dall’assegnazione. Questo potrebbe creare confusione per l’utente, poiché, come parte del team del progetto, riceve notifiche sull’attività del progetto e visualizza il progetto nell’elenco Progetti in corso.


Inoltre, i membri del team di progetto ottengono le autorizzazioni per il progetto e le relative attività, problemi e documenti. Questo può comportare l’accesso degli utenti agli articoli di Workfront di cui non hanno bisogno o che non dovrebbero avere.

</br>
</br>

**Best practice**

Posiziona Metriche progetto nella parte superiore del menu del pannello di sinistra per gli utenti che utilizzano principalmente Workfront per visualizzare i dati.

**Ecco perché**

La maggior parte dei leader, dirigenti e altri utenti che non gestiscono progetti o non eseguono assegnazioni di attività apprezzerebbe vedere questo livello di metriche del progetto quando aprono un progetto per la prima volta. Utilizza un modello di layout per spostare Metriche progetto nella parte superiore del menu del pannello di sinistra in una pagina di progetto per renderlo più visibile e accessibile agli utenti.
