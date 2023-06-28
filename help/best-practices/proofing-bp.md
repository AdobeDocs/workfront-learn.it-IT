---
title: Best practice - Strumenti di correzione
description: Esplora le best practice consigliate dagli esperti Adobe Workfront in merito all’impostazione, alla gestione e all’utilizzo degli strumenti di verifica in Workfront.
feature: Workfront Proof
role: Admin, Leader, User
level: Beginner
jira: KT-10920
exl-id: 394485ee-bb8f-4248-86a9-4c86174dd37f
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '1179'
ht-degree: 0%

---

# Best practice - Strumenti di correzione

## Cos’è una &quot;best practice&quot; di Adobe Workfront?

Le best practice sono linee guida che rappresentano una linea di condotta efficace ed efficiente, sono facilmente adottabili da te e dagli utenti della tua azienda e possono essere replicate correttamente all’interno dell’organizzazione.

Mentre esamini questi consigli, tieni presente che alcune best practice di Workfront sono universali, mentre altre potrebbero essere più specifiche per l’argomento. Utilizza queste best practice come framework per guidare le impostazioni e l’utilizzo del sistema Workfront.

## Navigazione in questa pagina

Scorrendo questa pagina, troverai innanzitutto un elenco di alto livello di tutte le best practice per l’argomento. Questo ti consente di rivedere i consigli senza immergerti nei dettagli di &quot;perché&quot;.

La sezione &quot;Perché sono queste best practice?&quot; , disponibile dopo l’elenco di alto livello, fornisce maggiori dettagli su alcune delle best practice e sul perché sono considerate un processo, uno strumento, ecc., è consigliabile implementarle con l’istanza di Workfront.

</br>
</br>

## Best practice per la verifica in Workfront

* Crea modelli di flusso di lavoro per la verifica.

* Nelle impostazioni di Workfront, disabilita l’impostazione &quot;Send emails from Workfront when a comment is made on a proof&quot; (Invia e-mail da quando viene inserito un commento su una bozza).

* Utilizzare solo Read Only o Reviewer per l&#39;impostazione &quot;Roles for non-recipients that open a document proof&quot; (Ruoli per non destinatari che aprono una bozza di documento) in Workfront.

* Regola le impostazioni di back-end della bozza in modo che gli utenti possano visualizzare le scadenze in un formato di orologio di 12 ore.

* Stabilisci una scadenza predefinita per la bozza come parte delle impostazioni di sistema.

* Nascondi l’opzione di decisione Bozza non rilevante.

* Non riordinare le opzioni di decisione bozza nelle impostazioni bozza.

* Impostazione delle impostazioni predefinite per i ruoli delle bozze e gli avvisi e-mail.

* Imposta il ruolo di bozza del creatore della bozza su Revisore.

* Evita di usare il ruolo di bozza Approvatore.

* Evita l’opzione di avviso e-mail All Activity proof (Tutte le attività).

</br>
</br>

## Perché si tratta di procedure ottimali?

**Best practice**

Crea modelli di flusso di lavoro per la verifica.

**Ecco perché**

I modelli non solo velocizzano e semplificano il processo di creazione e assegnazione delle bozze, ma forniscono anche coerenza tra i flussi di lavoro delle bozze per tipi di risorse simili. Inoltre, garantiscono che a ogni destinatario della bozza vengano assegnati il ruolo di bozza e l’avviso e-mail appropriati e che sia stata impostata una scadenza.

</br>
</br>

**Best practice**

Nelle impostazioni di Workfront, disabilita l’impostazione &quot;Send emails from Workfront when a comment is made on a proof&quot; (Invia e-mail da quando viene inserito un commento su una bozza).



**Ecco perché**

Quando questa impostazione è abilitata (che è per impostazione predefinita), gli utenti possono ricevere più notifiche e-mail per ogni commento su una bozza, una dalla funzionalità di correzione e una da Workfront stessa. Tali notifiche duplicate causano confusione e interruzioni delle notifiche e-mail, nonché una casella in entrata e-mail completa, che può in ultima analisi causare l’ignoramento delle notifiche delle bozze ricevute dagli utenti. Il che, a sua volta, potrebbe significare scadenze non rispettate.



**Nota**: questa impostazione si trova nel menu principale di Workfront > Configurazione > E-mail > Revisione e approvazione.

</br>
</br>

**Best practice**

Utilizzare solo Read Only o Reviewer per l&#39;impostazione &quot;Roles for non-recipients that open a document proof&quot; (Ruoli per non destinatari che aprono una bozza di documento) in Workfront.



**Ecco perché**

Le altre opzioni per questa impostazione richiedono tutte una decisione di bozza, che può far deragliare il flusso di lavoro di bozza. In genere, gli utenti che non vengono aggiunti al flusso di lavoro della bozza devono solo visualizzarla o aggiungere commenti, non approvare la bozza, pertanto le opzioni Sola lettura o Revisore sono la scelta migliore.



**Nota**: questa impostazione si trova nel menu principale di Workfront > Configurazione > Revisione e approvazione.

</br>
</br>

**Best practice**

Regola le impostazioni di back-end della bozza in modo che gli utenti possano visualizzare le scadenze in un formato di orologio di 12 ore.



**Ecco perché**

Seleziona l’opzione F j, Y, gi:a nelle impostazioni della bozza per gli utenti che desiderano visualizzare le scadenze/ore della bozza in formato AM/PM. Per le aree che utilizzano un orologio da 12 ore, questo aiuta a chiarire le scadenze.



**Nota**: per trovare questa impostazione, accedi al menu principale di Workfront > Strumenti di correzione > Impostazioni account > Utenti > e modifica il campo Formato data per ogni utente.

</br>
</br>

**Best practice**

Stabilisci una scadenza predefinita per la bozza come parte delle impostazioni di sistema.



**Ecco perché**

Quando viene impostata una scadenza predefinita della bozza (data di caricamento + x numero di giorni lavorativi), se il creatore della bozza dimentica di aggiungere una scadenza, Workfront la applica automaticamente a ogni bozza caricata.



**Nota**: per trovare questa impostazione, accedi al campo Menu principale di Workfront > Strumenti di correzione > Impostazioni account > Impostazioni > Valori predefiniti bozza > Scadenza (+ giorni lavorativi).

</br>
</br>


**Best practice**

Nascondi l’opzione di decisione Bozza non rilevante.



**Ecco perché**

Questa opzione di decisione causa spesso confusione tra gli approvatori, in quanto spesso le organizzazioni non definiscono quando utilizzare l’opzione Non pertinente. L’opzione Non pertinente indica in genere che la bozza non è pertinente per il destinatario della bozza e che non è necessario che prenda una decisione approvata o rifiutata. Selezionando Non pertinente, puoi continuare il flusso di lavoro della bozza.


L’opzione Non rilevante non è necessaria nella maggior parte dei flussi di lavoro per bozze.

**Nota**: per trovare questa impostazione, vai al menu principale di Workfront > Strumenti di correzione > Impostazioni account > Decisioni.

</br>
</br>

**Best practice**

Non riordinare le opzioni di decisione bozza nelle impostazioni bozza.



**Ecco perché**

Ogni impostazione di decisione della bozza contiene un valore/peso specifico che, se riordinato, può generare confusione nelle configurazioni della bozza. L’ordine di decisione e il valore/peso vengono utilizzati come attivatori della fase di bozza e nel reporting.



**Nota**: per trovare questa impostazione, vai al menu principale di Workfront > Strumenti di correzione > Impostazioni account > Decisioni.

</br>
</br>

**Best practice**

Impostazione delle impostazioni predefinite per i ruoli delle bozze e gli avvisi e-mail.



**Ecco perché**

Queste impostazioni si popolano automaticamente durante l’assegnazione di un flusso di lavoro della bozza, velocizzando il processo e contribuendo alla coerenza tra i flussi di lavoro della bozza.



**Nota**: le impostazioni predefinite dell’utente si trovano accedendo al menu principale di Workfront > Strumenti di correzione > Impostazioni account > Utenti > e selezionando l’utente per cui impostare le impostazioni predefinite.

</br>
</br>

**Best practice**

Imposta il ruolo di bozza del creatore della bozza su Revisore.



**Ecco perché**

Il ruolo Bozza revisore consente al creatore della bozza di inserire commenti e accedere ai commenti lasciati da altri utenti. Nella maggior parte dei casi, il creatore della bozza non è tenuto a prendere una decisione su una bozza caricata. I ruoli Approvatore, Revisore e Approvatore, Autore o Moderatore della bozza richiedono tutti una decisione. Se al creatore della bozza viene assegnato uno di questi ruoli di bozza ma non prende mai una decisione, ciò può influenzare negativamente le scadenze della bozza.

</br>
</br>

**Best practice**

Evita di usare il ruolo di bozza Approvatore.



**Ecco perché**

Il ruolo Bozza approvatore non consente all’utente di aggiungere commenti a questa bozza. Questo poteva comportare il rifiuto della bozza da parte di un utente, senza alcuna spiegazione, in quanto l’utente non era in grado di aggiungere commenti. Utilizza invece il ruolo di bozza Revisore e Approvatore in modo che l’utente possa fornire un feedback.

</br>
</br>

**Best practice**

Evita l’opzione di avviso e-mail All Activity proof (Tutte le attività).

**Ecco perché**

Questa opzione invia una notifica e-mail relativa alla bozza ogni volta che si verifica un evento con una bozza: viene inserito un commento, viene inviata una risposta, viene presa una decisione, ecc. In sostanza, il destinatario vede l’attività della bozza così come si verifica.

Per i proprietari e i creatori di bozze, l’avviso e-mail per le decisioni funziona meglio per i flussi di lavoro a bozza multipla e Final Decision (Decisione finale) funziona meglio per i flussi di lavoro a fase singola. In genere, tutti gli altri possono essere impostati su Disabilitato, a meno che non desiderino essere informati di altri utenti che stanno prendendo commenti o decisioni (nel qual caso, una delle opzioni di riepilogo dell’e-mail potrebbe funzionare meglio).
