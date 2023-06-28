---
title: 'Best practice: licenze e livelli di accesso'
description: Esplora le best practice consigliate dagli esperti Adobe Workfront in merito alla configurazione, alla gestione e all’utilizzo delle licenze e dei livelli di accesso di Workfront.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
jira: KT-10914
exl-id: 6be3fab9-16a1-4ab9-89ce-8c53f8358e62
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '1253'
ht-degree: 0%

---

# Best practice: licenze e livelli di accesso

## Cos’è una &quot;best practice&quot; di Adobe Workfront?

Le best practice sono linee guida che rappresentano una linea di condotta efficace ed efficiente, sono facilmente adottabili da te e dagli utenti della tua azienda e possono essere replicate correttamente all’interno dell’organizzazione.

Mentre esamini questi consigli, tieni presente che alcune best practice di Workfront sono universali, mentre altre potrebbero essere più specifiche per l’argomento. Utilizza queste best practice come framework per guidare le impostazioni e l’utilizzo del sistema Workfront.

## Navigazione in questa pagina

Scorrendo questa pagina, troverai innanzitutto un elenco di alto livello di tutte le best practice per l’argomento. Questo ti consente di rivedere i consigli senza immergerti nei dettagli di &quot;perché&quot;.

La sezione &quot;Perché sono queste best practice?&quot; , disponibile dopo l’elenco di alto livello, fornisce maggiori dettagli su alcune delle best practice e sul perché sono considerate un processo, uno strumento, ecc., è consigliabile implementarle con l’istanza di Workfront.

</br>
</br>

## Best practice relative a licenze e livelli di accesso

* Quando si impostano i livelli di accesso, gli utenti possono iniziare con un livello di accesso inferiore.

* Quando si assegnano le licenze di revisione e richiesta, in genere per impostazione predefinita viene impostato il valore Revisione, in quanto fornisce all’utente più autorizzazioni in Adobe Workfront.

* Deseleziona la casella di controllo &quot;Condividi a livello di sistema&quot; su ciascun oggetto in tutti i tuoi livelli di accesso, a meno che tu non voglia specificatamente che tali utenti siano in grado di farlo.

* Prendi in considerazione l’attivazione dell’impostazione &quot;Non consentire mai agli utenti di eliminare commenti&quot; in Impostare restrizioni aggiuntive a un livello di accesso.

* Limitare il numero di amministratori di sistema a favore degli amministratori di gruppo.

* Copiare un livello di accesso esistente e apportare modifiche, anziché creare un nuovo livello di accesso da zero.

* Documentare le operazioni che ogni livello di accesso può eseguire nella casella Descrizione.

* Limiti ai soli livelli di accesso necessari per raggiungere gli obiettivi di lavoro, idealmente quattro o cinque che soddisfino le esigenze della maggior parte degli utenti del sistema.

* Assegnare ad almeno due utenti il livello di accesso amministratore di sistema globale.

* Limita le operazioni che gli utenti possono eseguire con gli elementi di Workfront tramite la condivisione, anziché rimuovere una funzionalità in un livello di accesso.

</br>
</br>


## Perché si tratta di procedure ottimali?

**Best practice**

Quando si impostano i livelli di accesso, gli utenti possono iniziare con un livello di accesso inferiore.



**Ecco perché**

Avvia gli utenti con il minimo accesso di cui avranno bisogno per svolgere il loro lavoro. Se non possono svolgere il loro lavoro a causa di diritti di accesso insufficienti, in genere richiedono un accesso aggiuntivo. Concedere immediatamente agli utenti un accesso eccessivo potrebbe causare problemi di sicurezza. Inoltre, è sempre meglio dare agli utenti più accesso piuttosto che togliergli l’accesso.

</br>
</br>



**Best practice**

Quando si assegnano le licenze di revisione e richiesta, in genere per impostazione predefinita viene impostato il valore Revisione, in quanto fornisce all’utente più autorizzazioni in Adobe Workfront.



**Ecco perché**

Sebbene sia le licenze di revisione che quelle di richiesta possano essere assegnate a un numero illimitato di utenti in Workfront, le licenze di richiesta sono limitate all’elaborazione e all’aggiornamento delle richieste. Una licenza Revisione consente di accedere a progetti e attività in modo più ampio rispetto a una licenza Richiesta, nonché di visualizzare portfolio e programmi, modificare documenti e accedere a strumenti di gestione delle risorse.

</br>
</br>

**Best practice**

Deseleziona la casella di controllo &quot;Condividi a livello di sistema&quot; su ciascun oggetto in tutti i tuoi livelli di accesso, a meno che non vi sia un motivo specifico per cui gli utenti devono essere in grado di condividere a livello di sistema.



**Ecco perché**

La condivisione di un oggetto a livello di sistema viene spesso utilizzata come stampella per consentire a determinati utenti di visualizzare gli elementi in Workfront. Ciò si verifica quando la struttura del gruppo Workfront non è presente o quando le autorizzazioni di condivisione non sono pienamente comprese. Quando gli elementi vengono condivisi a livello di sistema, significa che tutti possono visualizzare l&#39;elemento condiviso. A seconda del tipo di informazioni conservate nel sistema, ciò potrebbe causare problemi di privacy.



Ad esempio, potresti lavorare con diversi fornitori all’interno di Workfront per verificare lo stato di avanzamento, fornire approvazioni, ecc. Se la casella di controllo &quot;Condividi a livello di sistema&quot; è un’opzione, è possibile selezionarla o impostarla come predefinita, rendendo le informazioni disponibili a tutti i fornitori.



Deselezionando completamente l’opzione, lo si rende così un utente, con l’autorizzazione di condividere, deve determinare la persona o le persone specifiche (tramite un’azienda, un gruppo o un team) con cui desidera condividere l’oggetto.

</br>
</br>

**Best practice**

Prendi in considerazione l’attivazione dell’impostazione &quot;Non consentire mai agli utenti di eliminare commenti&quot; in Impostare restrizioni aggiuntive a un livello di accesso.



**Ecco perché**

L’attivazione di questa opzione garantisce che le comunicazioni passate non vengano rimosse da Workfront. Alcune organizzazioni richiedono che la cronologia completa dei commenti venga conservata a scopo di audit.

</br>
</br>

**Best practice**

Limitare il numero di amministratori di sistema a favore degli amministratori di gruppo.



**Ecco perché**

Gli amministratori di sistema hanno accesso a tutto ciò che si trova in Workfront, incluse le impostazioni di sistema globali. Gli amministratori del gruppo di impostazioni a cui possono accedere sono controllati dall’amministratore di sistema e si applicano solo a quel gruppo specifico.



La possibilità di disporre di amministratori di gruppo consente agli amministratori di sistema di delegare molte responsabilità, consentendo loro di concentrarsi su elementi di immagine più grandi, anziché sulla manutenzione quotidiana di Workfront. Gli amministratori di gruppi possono essere più facilmente in contatto con le esigenze dei loro gruppi, il che offre un servizio migliore agli utenti.

</br>
</br>


**Best practice**

Copiare un livello di accesso esistente e apportare modifiche, anziché creare un nuovo livello di accesso da zero.



**Ecco perché**

La copia di un livello di accesso esistente fornisce una base coerente per i nuovi livelli di accesso, garantendo che le impostazioni iniziali siano identiche. Anche questo consente di risparmiare tempo, poiché gli amministratori di sistema non dovranno impostare un livello di accesso completamente da zero.

</br>
</br>

**Best practice**

Documentare le operazioni che ogni livello di accesso può eseguire nella casella Descrizione.



**Ecco perché**

Descrivere dettagliatamente le impostazioni per ciascun tipo di oggetto. Questo consente agli amministratori di sistema, presenti e futuri, di sapere esattamente cosa fa ogni livello di accesso senza doversi immergere nel livello di accesso stesso per rivedere le impostazioni.



Questo può anche semplificare il confronto dei livelli di accesso quando li si visualizza in un rapporto. Il campo di descrizione può essere aggiunto rapidamente alla vista per vedere rapidamente come si differenziano ed eventualmente perché è stato creato un diverso livello di accesso.

</br>
</br>

**Best practice**

Limiti ai soli livelli di accesso necessari per raggiungere gli obiettivi di lavoro, idealmente quattro o cinque che soddisfino le esigenze della maggior parte degli utenti del sistema.


**Ecco perché**

Il livello di accesso garantisce che, quando un oggetto Workfront viene condiviso con un utente, quest’ultimo disponga dei diritti necessari per modificarlo, eliminarlo e così via. Puoi rendere i livelli di accesso più generali, perché la condivisione su singoli elementi può essere configurata per essere più specifica.


Inoltre, avere meno livelli di accesso può facilitare la gestione di un sistema privo di ingombri e l’implementazione di una strategia, il che può anche portare a un onboarding più rapido quando le persone si uniscono all’azienda o cambiano reparto.

</br>
</br>

**Best practice**

Assegnare ad almeno due utenti il livello di accesso amministratore di sistema globale.

**Ecco perché**

Più di una persona dovrebbe capire perché Workfront è stato configurato nel modo in cui era, come gestirlo/manutenerlo e come supportare gli utenti. Se una persona è fuori sede, lascia l’organizzazione, è occupata, ecc., questo assicura che ci sia un’altra persona che dispone delle informazioni e delle conoscenze necessarie per gestire correttamente il sistema.

</br>
</br>

**Best practice**

Limita le operazioni che gli utenti possono eseguire con gli elementi di Workfront tramite la condivisione, anziché rimuovere una funzionalità in un livello di accesso.


**Ecco perché**

I livelli di accesso controllano cosa gli utenti possono fare con elementi specifici a livello globale. Le autorizzazioni di condivisione per ciascun progetto, attività, portfolio, documento e così via controllano le operazioni che un singolo utente può eseguire con quell’elemento specifico. Invece di rimuovere una funzionalità per tutti coloro che dispongono di un livello di accesso specifico, perfeziona le autorizzazioni di condivisione per elementi specifici in modo che gli utenti abbiano controlli limitati.
