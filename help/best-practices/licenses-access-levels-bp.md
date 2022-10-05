---
title: Best practice - Licenze e livelli di accesso
description: Scopri le best practice consigliate dagli esperti Adobe Workfront sull’impostazione, la gestione e l’utilizzo delle licenze e dei livelli di accesso Workfront.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
kt: 10914
exl-id: 6be3fab9-16a1-4ab9-89ce-8c53f8358e62
source-git-commit: 444f059d3cc26d8e3074a7145bc5419407c786cf
workflow-type: tm+mt
source-wordcount: '1253'
ht-degree: 0%

---

# Best practice - Licenze e livelli di accesso

## Qual è una &quot;best practice&quot; di Adobe Workfront?

Le migliori pratiche sono linee guida che rappresentano un&#39;azione efficace ed efficiente; sono facilmente adottati da te e dagli utenti della tua azienda; e può essere replicato correttamente in tutta l’organizzazione.

Quando si esaminano queste raccomandazioni, tenere presente che alcune best practice di Workfront sono universali, mentre altre potrebbero essere più specifiche per l’argomento. Utilizza queste best practice come framework per guidare le impostazioni e l’utilizzo del sistema Workfront.

## Navigazione in questa pagina

Scorrendo questa pagina, troverai innanzitutto un elenco di alto livello contenente tutte le best practice per l’argomento. Questo ti consente di rivedere le raccomandazioni senza immergerti nei dettagli del &quot;perché&quot;.

Perché queste best practice? area, disponibile dopo l’elenco di alto livello, fornisce maggiori dettagli su alcune delle best practice e sui motivi per cui vengono considerate un processo, uno strumento, ecc., dovresti considerare l’implementazione con la tua istanza Workfront.

</br>
</br>

## Best practice per licenze e livelli di accesso

* Inizia con meno accesso per gli utenti durante la configurazione dei livelli di accesso.

* Quando si assegnano le licenze di revisione e richiesta, in genere viene eseguito il controllo come impostazione predefinita perché fornisce all&#39;utente più autorizzazioni in Adobe Workfront.

* Deseleziona la casella di controllo &quot;Condividi tutto il sistema&quot; su ogni oggetto in tutti i livelli di accesso, a meno che tu non desideri che gli utenti siano in grado di farlo.

* È consigliabile attivare l’impostazione &quot;Non consentire mai agli utenti di eliminare commenti&quot; in Imposta restrizioni aggiuntive a livello di accesso.

* Limita il numero di amministratori di sistema a favore degli amministratori di gruppo.

* Copia un livello di accesso esistente e apporta modifiche, anziché creare un nuovo livello di accesso da zero.

* Nella casella Descrizione è possibile documentare le operazioni di ogni livello di accesso.

* Puoi limitarti a raggiungere solo i livelli di accesso necessari per raggiungere gli obiettivi di lavoro, idealmente quattro o cinque che soddisfano le esigenze della maggior parte degli utenti del sistema.

* Assegna almeno due utenti al livello di accesso globale dell’amministratore di sistema.

* Limita le operazioni degli utenti con gli elementi Workfront tramite la condivisione, anziché rimuovere una funzionalità a livello di accesso.

</br>
</br>


## Perché queste best practice sono?

**Best practice**

Inizia con meno accesso per gli utenti durante la configurazione dei livelli di accesso.



**Ecco perché**

Avvia gli utenti con l’accesso minimo di cui avranno bisogno per svolgere il loro lavoro. Se non possono svolgere il loro lavoro a causa di diritti di accesso insufficienti, in genere richiedono un accesso aggiuntivo. Concedere agli utenti un accesso troppo rapido potrebbe portare a problemi di sicurezza. Inoltre, è sempre meglio dare agli utenti più accesso che rimuovere l’accesso.

</br>
</br>



**Best practice**

Quando si assegnano le licenze di revisione e richiesta, in genere viene eseguito il controllo come impostazione predefinita perché fornisce all&#39;utente più autorizzazioni in Adobe Workfront.



**Ecco perché**

Sebbene sia le licenze di revisione che di richiesta possano essere assegnate a un numero illimitato di utenti in Workfront, le licenze di richiesta sono limitate praticamente solo a fare e aggiornare le richieste. Una licenza di revisione ha più accesso ai progetti e alle attività rispetto a una licenza di richiesta, così come la possibilità di visualizzare portfolio e programmi, modificare documenti e accedere agli strumenti di gestione delle risorse.

</br>
</br>

**Best practice**

Deseleziona la casella di controllo &quot;Condividi tutto il sistema&quot; su ogni oggetto in tutti i livelli di accesso, a meno che non vi sia un motivo specifico per cui gli utenti devono essere in grado di condividere a livello di sistema.



**Ecco perché**

La condivisione di un sistema di oggetti viene spesso utilizzata come stampella per consentire ad alcuni utenti di visualizzare gli elementi in Workfront. Questo accade quando la struttura del gruppo Workfront manca o quando le autorizzazioni di condivisione non sono completamente comprese. Quando gli elementi sono condivisi a livello di sistema, significa che tutti possono vedere l&#39;elemento condiviso. A seconda del tipo di informazioni conservate nel sistema, ciò potrebbe causare problemi di privacy.



Ad esempio, potresti lavorare con diversi fornitori all’interno di Workfront per verificare lo stato di avanzamento, fornire approvazioni e così via. Se la casella di controllo &quot;Condividi a livello di sistema&quot; è un&#39;opzione, può essere selezionata o impostata come predefinita, rendendo le informazioni disponibili a tutti i fornitori.



Deselezionando completamente l’opzione , l’utente deve determinare la persona o le persone specifiche, tramite una società, un gruppo o un team, con cui desidera condividere l’oggetto, con cui deve essere autorizzato a condividerlo.

</br>
</br>

**Best practice**

È consigliabile attivare l’impostazione &quot;Non consentire mai agli utenti di eliminare commenti&quot; in Imposta restrizioni aggiuntive a livello di accesso.



**Ecco perché**

Attivando questa opzione, le comunicazioni passate non vengono rimosse da Workfront. Alcune organizzazioni richiedono che la cronologia completa dei commenti sia conservata a scopo di controllo.

</br>
</br>

**Best practice**

Limita il numero di amministratori di sistema a favore degli amministratori di gruppo.



**Ecco perché**

Gli amministratori di sistema possono accedere a tutto ciò che si trova in Workfront, incluse le impostazioni di sistema globali. Gli amministratori del gruppo di impostazioni a cui possono accedere sono controllati dall&#39;amministratore di sistema e si applicano solo a quel gruppo specifico.



L&#39;utilizzo di amministratori di gruppo consente agli amministratori di sistema di delegare molte responsabilità, consentendo loro di concentrarsi su elementi più grandi, piuttosto che sulla manutenzione quotidiana di Workfront. Gli amministratori dei gruppi possono essere più facilmente in contatto con le esigenze dei loro gruppi, il che fornisce un servizio migliore per gli utenti.

</br>
</br>


**Best practice**

Copia un livello di accesso esistente e apporta modifiche, anziché creare un nuovo livello di accesso da zero.



**Ecco perché**

Copiare un livello di accesso esistente fornisce una base coerente per i nuovi livelli di accesso, garantendo che le impostazioni iniziali siano identiche. Inoltre, questo è un risparmio di tempo, in quanto gli amministratori di sistema non dovranno impostare un livello di accesso completamente da zero.

</br>
</br>

**Best practice**

Nella casella Descrizione è possibile documentare le operazioni di ogni livello di accesso.



**Ecco perché**

La descrizione contiene un elenco delle impostazioni relative a ciascun tipo di oggetto. Questo aiuta gli amministratori di sistema, presenti e futuri, a sapere esattamente cosa fa ogni livello di accesso senza doversi immergere nel livello di accesso stesso per rivedere le impostazioni.



Questo può anche semplificare il confronto dei livelli di accesso quando li si visualizza in un rapporto. È possibile aggiungere rapidamente il campo di descrizione alla visualizzazione per vedere rapidamente le differenze e, eventualmente, il motivo per cui è stato creato un diverso livello di accesso.

</br>
</br>

**Best practice**

Puoi limitarti a raggiungere solo i livelli di accesso necessari per raggiungere gli obiettivi di lavoro, idealmente quattro o cinque che soddisfano le esigenze della maggior parte degli utenti del sistema.


**Ecco perché**

Il livello di accesso assicura che quando un oggetto Workfront viene condiviso con un utente, l&#39;utente disponga dei diritti necessari per modificarlo, eliminarlo, ecc. Puoi rendere i livelli di accesso più generali perché la condivisione su singoli elementi può essere configurata in modo da essere più specifica.


Inoltre, un minor numero di livelli di accesso può facilitare il mantenimento di un sistema privo di ingombro e l&#39;implementazione di una strategia, che può anche portare a un onboarding più rapido quando le persone si uniscono all&#39;azienda o al reparto di commutazione.

</br>
</br>

**Best practice**

Assegna almeno due utenti al livello di accesso globale dell’amministratore di sistema.

**Ecco perché**

Più di una persona deve comprendere perché Workfront è stato configurato nel modo in cui era, come gestirlo/gestirlo e come supportare gli utenti. Se una persona è fuori ufficio, lascia l&#39;organizzazione, è occupata, ecc, questo assicura che ci sia un&#39;altra persona che ha le informazioni e le conoscenze per gestire con successo il sistema.

</br>
</br>

**Best practice**

Limita le operazioni degli utenti con gli elementi Workfront tramite la condivisione, anziché rimuovere una funzionalità a livello di accesso.


**Ecco perché**

I livelli di accesso controllano le operazioni che gli utenti possono eseguire con elementi specifici a livello globale. Le autorizzazioni di condivisione per ogni progetto, attività, portfolio, documento e così via controllano le operazioni che un singolo utente può eseguire con quel particolare elemento. Invece di rimuovere una funzionalità per tutti coloro che dispongono di un livello di accesso specifico, ottimizza le autorizzazioni di condivisione per elementi specifici in modo che gli utenti abbiano controlli limitati.
