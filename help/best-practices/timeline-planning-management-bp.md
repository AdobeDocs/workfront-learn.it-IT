---
title: Best practice- Pianificazione e gestione della timeline
description: Esplora le best practice consigliate dagli esperti di Adobe Workfront in merito all’impostazione, alla gestione e all’utilizzo delle timeline di progetto in Workfront.
feature: Get Started with Workfront
role: Admin, Leader, User
level: Beginner
jira: KT-10929
exl-id: 8c18746d-e23a-44d0-b1e3-ebf5ba8d022f
TQID: https://experienceleague.adobe.com/dHR6MHjya-MlhyDeL6MJvMPzaIkPpp91zfYe6ebcbL0
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bdid: f8a45b24-4be7-4f1b-909b-60d06b483a20
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: 36674ed53c8645f556862bb2d99f3bfd6c993c1e
workflow-type: tm+mt
source-wordcount: 1117
ht-degree: 96%

---

# Best practice- Pianificazione e gestione della timeline

## Che cos’è una “best practice” di Adobe Workfront?

Le best practice sono linee guida che rappresentano una linea d’azione efficace ed efficiente; sono facilmente adottabili da te e dagli utenti della tua azienda; e possono essere replicate con successo in tutta l’organizzazione.

Mentre esamini questi consigli, tieni presente che alcune best practice di Workfront sono universali mentre altre potrebbero essere più specifiche per un dato argomento. Utilizza queste best practice come una base comune per le impostazioni e l’utilizzo del sistema Workfront.

## Esplorazione di questa pagina

Mentre scorri questa pagina, troverai innanzitutto un elenco di alto livello di tutte le best practice per questo argomento. Questo ti consente di rivedere i consigli senza entrare nei dettagli del “perché”.

L’area &quot;Perché queste best practice?&quot;, che si trova dopo l’elenco di alto livello, fornisce maggiori dettagli su alcune delle best practice e sul perché vengono considerate un processo, uno strumento, ecc., è consigliabile implementarle con l’istanza di Workfront.

</br>
</br>

## Best practice per la pianificazione e la gestione della timeline

* Tutti i progetti completati devono avere uno stato che indica che sono completati.

* Durante la copia di un progetto, imposta lo stato del nuovo progetto su Pianificazione.

* Chiedi agli utenti di registrare il tempo effettivo trascorso sulle attività in modo da poter confrontare le ore effettive con quelle pianificate.

* Se possibile, utilizza le durate delle attività e i predecessori per generare e aggiornare la timeline di un progetto, anziché selezionare date di inizio e completamento specifiche.

* Chiedi agli utenti di aggiornare lo stato delle attività, la percentuale di completamento e le ore effettive ogni giorno (o ogni settimana in base a una pianificazione prestabilita).

* Imposta lo stato del progetto su Pianificazione durante l’aggiornamento del piano di progetto per impedire l’invio automatico delle notifiche quando vengono apportate modifiche.

* Rimuovi dal team del progetto gli utenti ai quali non è stato assegnato un lavoro nel progetto.

* Posiziona Project Metrics (Metriche del progetto) nella parte superiore del menu del pannello a sinistra per gli utenti che usano Workfront principalmente per visualizzare i dati.


</br>
</br>


## Perché queste sono best practice?

**Best practice**

Tutti i progetti completati devono avere uno stato che indica che sono completati.


**Ecco perché**

Assicurati che tutti i progetti completati abbiano lo stato Completato (o equivalente) per mantenere pulita e corrente l’istanza di Workfront. Mantenendo aggiornati gli stati dei progetti e chiudendoli, gli utenti possono facilmente capire quale lavoro è già stato svolto, in modo da potersi concentrare sulle priorità attive. Inoltre, assicura che i dati dei rapporti su progetti, attività, risorse, ecc. siano accurati.


</br>
</br>

**Best practice**

Durante la copia di un progetto, imposta lo stato del nuovo progetto su Pianificazione.

**Ecco perché**

Lo stato Pianificazione (o equivalente) impedisce a Workfront di inviare notifiche su assegnazioni, modifiche alla timeline e così via prima che il progetto sia pronto. Quando copi un progetto, viene visualizzata una finestra di dialogo con le opzioni del progetto; modifica lo stato qui, mentre regola altre opzioni in modo che i dati non vengano copiati dal progetto originale alla versione copiata.

</br>
</br>

**Best practice**

Chiedi agli utenti di registrare il tempo effettivo trascorso sulle attività in modo da poter confrontare le ore effettive con quelle pianificate.


**Ecco perché**

Tenendo conto della durata del lavoro delle attività è possibile aggiornare i modelli di progetto per una maggiore precisione nella pianificazione dei progetti futuri. Significa anche che le stime delle risorse, utilizzando gli strumenti di gestione delle risorse di Workfront, sono più precise.

</br>
</br>

**Best practice**

Se possibile, utilizza le durate delle attività e i predecessori per generare e aggiornare la timeline di un progetto, anziché selezionare date di inizio e completamento specifiche.

**Ecco perché**

L’utilizzo di durate e predecessori insieme a vincoli di attività flessibili (Il più presto possibile e Il più tardi possibile) consente di apportare modifiche automatiche alle date della timeline che “si sovrappongono” al piano del progetto. Quando ad esempio la durata di un’attività aumenta di un giorno, viene modificata la data di completamento pianificata dell’attività, che a sua volta determina la modifica delle date di completamento delle attività seguenti.

Se si selezionano date di inizio e di completamento specifiche per le attività, il vincolo dell’attività viene modificato in un vincolo che “blocca” la data (Deve iniziare il, Deve finire il, Date fisse), il che significa che è necessario eseguire manualmente alcuni aggiornamenti delle date della timeline.

</br>
</br>


**Best practice**

Chiedi agli utenti di aggiornare lo stato delle attività, la percentuale di completamento e le ore effettive ogni giorno (o ogni settimana in base a una pianificazione prestabilita).

**Ecco perché**

I rapporti in Workfront sono accurati solo quanto i dati immessi in Workfront. Quando le informazioni che indicano l’avanzamento del lavoro, come lo stato e la percentuale di completamento, non vengono aggiornate regolarmente, i rapporti che mostrano l’avanzamento del lavoro non saranno precisi. L’aggiornamento su base giornaliera offre la massima precisione nei dati di reporting in tempo reale.


Lo stato dell’attività consente inoltre di informare gli utenti quando un lavoro precedente è stato completato e le nuove attività possono iniziare. Se lo stato dell’attività non viene modificato per riflettere l’avanzamento effettivo sull’elemento di lavoro, Workfront non può inviare le notifiche appropriate.

</br>
</br>

**Best practice**

Imposta lo stato del progetto su Pianificazione durante l’aggiornamento del piano di progetto per impedire l’invio automatico delle notifiche quando vengono apportate modifiche.

**Ecco perché**

Le modifiche apportate al piano di progetto possono generare più notifiche quando vengono modificate le assegnazioni delle attività, le date di inizio e di completamento pianificate e altre impostazioni. Questo può disturbare gli utenti e creare confusione su assegnazioni, scadenze corrette, ecc.

Lo stato Pianificazione indica a Workfront di non inviare notifiche sul progetto ai membri del team di progetto (utenti a cui sono state assegnate attività/problemi o altri utenti con accesso al progetto) perché il piano di progetto è ancora in fase di sviluppo o il progetto non è ancora pronto per essere pubblicato. Una volta completate le modifiche, torna allo stato Attuale del progetto e verranno inviate le notifiche. Seguendo questo processo si riduce al minimo il numero di notifiche ricevute dagli utenti.

</br>
</br>

**Best practice**

Rimuovi dal team del progetto gli utenti ai quali non è stato assegnato un lavoro nel progetto.


**Ecco perché**

Quando si assegna a un utente un’attività o un problema relativo a un progetto, l’utente viene aggiunto all’elenco dei team del progetto nelle sezioni Pianificazione e Persone. Tuttavia, rimane nell’elenco dei team del progetto anche se è stato rimosso dall’assegnazione. Questo potrebbe causare confusione nell’utente, perché come parte del team di progetto, riceve le notifiche sull’attività nel progetto e visualizza il progetto nell’elenco Progetti che mi interessano.


Inoltre, i membri del team di progetto ottengono le autorizzazioni per il progetto e le relative attività, problemi e documenti. Questo può comportare l’accesso degli utenti a elementi in Workfront di cui non hanno bisogno o che non dovrebbero avere.

</br>
</br>

**Best practice**

Posiziona Project Metrics (Metriche del progetto) nella parte superiore del menu del pannello a sinistra per gli utenti che usano Workfront principalmente per visualizzare i dati.

**Ecco perché**

La maggior parte dei leader, dei dirigenti e degli altri utenti che non gestiscono progetti o eseguono assegnazioni di attività apprezzerebbe vedere questo livello di metriche del progetto alla prima apertura del progetto. Utilizza un modello layout per spostare Metriche del progetto nella parte superiore del menu del pannello a sinistra in una pagina di progetto, per renderlo più visibile e più facilmente accessibile da parte degli utenti.
