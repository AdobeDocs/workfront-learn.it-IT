---
title: 'Best practice: bozza'
description: Esplora i consigli sulle best practice degli esperti di Adobe Workfront sulla configurazione, la gestione e l’utilizzo delle bozze in Workfront.
feature: Workfront Proof
role: Admin, Leader, User
level: Beginner
last-substantial-update: 2024-11-06T00:00:00Z
jira: KT-10920
exl-id: 394485ee-bb8f-4248-86a9-4c86174dd37f
source-git-commit: d9ccf45b157a4c66184cca0afadba35ef4c8615e
workflow-type: ht
source-wordcount: '1182'
ht-degree: 100%

---

# Best practice: bozza

## Che cos’è una “best practice” di Adobe Workfront?

Le best practice sono linee guida che rappresentano una linea d’azione efficace ed efficiente; sono facilmente adottabili da te e dagli utenti della tua azienda; e possono essere replicate con successo in tutta l’organizzazione.

Mentre esamini questi consigli, tieni presente che alcune best practice di Workfront sono universali mentre altre potrebbero essere più specifiche per un dato argomento. Utilizza queste best practice come una base comune per le impostazioni e l’utilizzo del sistema Workfront.

## Esplorazione di questa pagina

Scorrendo questa pagina, troverai innanzitutto un elenco di alto livello di tutte le best practice relative all’argomento. Questo ti consente di rivedere i consigli senza immergerti nei dettagli delle motivazioni.

“Perché queste sono best practice?” che si trova dopo l’elenco di alto livello, fornisce maggiori dettagli su alcune delle best practice e sul motivo per cui sono considerate un processo, uno strumento ecc. da implementare con la tua istanza di Workfront.

</br>
</br>

## Best practice sulla bozza in Workfront

* Prenditi tempo per creare i modelli di flusso di lavoro delle bozze.

* Nelle impostazioni di Workfront, disabilita l’impostazione “Invia e-mail da Workfront quando viene fatto un commento su una bozza”.

* Utilizza esclusivamente l’impostazione di Workfront Solo lettura o Revisore per “Ruoli non destinatari che aprono la bozza di un documento”.

* Regola le impostazioni di back-end della bozza in modo che gli utenti possano visualizzare le scadenze in un formato di 12 ore.

* Stabilisci una scadenza bozza predefinita come parte delle impostazioni di sistema.

* Nascondi l’opzione Non pertinente nella Decisione bozza.

* Non riordinare le opzioni di Decisione bozza nelle impostazioni bozza.

* Definisci le impostazioni predefinite per i ruoli bozza e gli avvisi e-mail.

* Imposta il ruolo bozza del Creatore della bozza su Revisore.

* Evita di utilizzare il ruolo bozza Approvatore.

* Evita l’opzione di avviso e-mail “Tutte le attività di bozza”.

</br>
</br>

## Perché queste sono best practice?

**Best practice**

Prenditi tempo per creare i modelli di flusso di lavoro delle bozze.

**Ecco perché**

I modelli non solo velocizzano e semplificano il processo di creazione e assegnazione delle bozze, ma garantiscono anche coerenza tra i flussi di lavoro di bozza per tipi di risorse simili. Inoltre, assicurano che a ogni destinatario della bozza vengano assegnati il ruolo bozza e l’avviso e-mail appropriati e che sia stata impostata una scadenza.

</br>
</br>

**Best practice**

Nelle impostazioni di Workfront, disabilita l’impostazione “Invia e-mail da Workfront quando viene fatto un commento su una bozza”.



**Ecco perché**

Quando questa impostazione è abilitata (che è per impostazione predefinita), gli utenti hanno la possibilità di ricevere più notifiche e-mail per ogni commento su una bozza: una dalla funzionalità di bozza e una da Workfront stesso. Tali notifiche duplicate creano confusione e interruzioni delle notifiche e-mail, nonché una casella di e-mail in entrata piena, che può in ultima analisi portare gli utenti a ignorare le notifiche delle bozze ricevute. Cosa che, a sua volta, potrebbe determinare il mancato rispetto delle scadenze.



**Nota**: questa impostazione si trova nel menu principale di Workfront > Configurazione > E-mail > Revisione e approvazione.

</br>
</br>

**Best practice**

Utilizza esclusivamente l’impostazione di Workfront Solo lettura o Revisore per “Ruoli non destinatari che aprono la bozza di un documento”.



**Ecco perché**

Le altre opzioni per questa impostazione richiedono tutte una Decisione bozza, che può ostacolare il flusso di lavoro di bozza. In genere, le persone non aggiunte al flusso di lavoro di bozza devono solo visualizzarla o creare commenti, non devono approvarla, pertanto le opzioni Sola lettura o Revisore sono la scelta migliore.



**Nota**: questa impostazione si trova nel menu principale di Workfront > Configurazione > Revisione e approvazione.

</br>
</br>

**Best practice**

Regola le impostazioni di back-end della bozza in modo che gli utenti possano visualizzare le scadenze in un formato di 12 ore.



**Ecco perché**

Il formato predefinito è quello di 24 ore, che può confondere coloro che non ne hanno familiarità. Per cambiare il formato, passa al Menu principale di Workfront > Bozza > Impostazioni account > Utenti. Fai doppio clic su un utente per selezionarne uno, quindi modifica il campo Formato data nella sezione Impostazioni personali. Per modificare gli utenti, è necessario selezionarne uno alla volta.

</br>
</br>

**Best practice**

Stabilisci una scadenza bozza predefinita come parte delle impostazioni di sistema.



**Ecco perché**

Quando viene impostata una scadenza bozza predefinita (data di caricamento + numero x di giorni lavorativi), se il creatore della bozza dimentica di aggiungere una scadenza, Workfront applica automaticamente questa scadenza a ogni bozza caricata.



**Nota**: questa impostazione si trova nel menu principale di Workfront > Bozze > Impostazioni account > Impostazioni > Impostazioni predefinite bozza > campo Scadenza (+ giorni lavorativi).

</br>
</br>


**Best practice**

Nascondi l’opzione Non pertinente nella Decisione bozza.



**Ecco perché**

Questa opzione di decisione causa spesso confusione tra gli approvatori, in quanto le organizzazioni non definiscono sempre quando utilizzare l’opzione Non pertinente. L’opzione Non pertinente indica in genere che la bozza non è pertinente per il destinatario della stessa, a cui non è richiesto di prendere una decisione di approvazione o rifiuto. La selezione di Non pertinente consente al flusso di lavoro di bozza di proseguire.


L’opzione Non pertinente non è necessaria nella maggior parte dei flussi di lavoro di bozza.

**Nota**: questa impostazione si trova nel menu principale di Workfront > Bozze > Impostazioni account > Decisioni.

</br>
</br>

**Best practice**

Non riordinare le opzioni di Decisione bozza nelle impostazioni bozza.



**Ecco perché**

Ogni impostazione di decisione bozza contiene un valore/peso specifico che, se riordinato, può generare confusione nelle configurazioni della bozza. L’ordine di decisione e il valore/peso vengono utilizzati come trigger di attivazione della fase di bozza e nella reportistica.



**Nota**: questa impostazione si trova nel menu principale di Workfront > Bozze > Impostazioni account > Decisioni.

</br>
</br>

**Best practice**

Definisci le impostazioni predefinite per i ruoli bozza e gli avvisi e-mail.



**Ecco perché**

Queste impostazioni vengono compilate automaticamente durante l’assegnazione di un flusso di lavoro di bozza, velocizzando il processo e contribuendo alla coerenza tra i flussi di lavoro di bozza.



**Nota**: le impostazioni predefinite dell’utente si trovano nel menu principale di Workfront > Bozze > Impostazioni account > Utenti > e selezionando l’utente per cui impostarle.

</br>
</br>

**Best practice**

Imposta il ruolo bozza del Creatore della bozza su Revisore.



**Ecco perché**

Il ruolo bozza Revisore consente al creatore della bozza di inserire commenti e accedere ai commenti lasciati da altri utenti. Nella maggior parte dei casi, il creatore della bozza non è tenuto a prendere una decisione su una bozza caricata. I ruoli bozza Approvatore, Revisore e Approvatore, Autore o Moderatore richiedono tutti di prendere una decisione. Se al creatore della bozza viene assegnato uno di questi ruoli bozza ma non prende mai decisioni, ciò può influire negativamente sulle scadenze della bozza.

</br>
</br>

**Best practice**

Evita di utilizzare il ruolo bozza Approvatore.



**Ecco perché**

Il ruolo bozza Approvatore non consente all’utente di aggiungere commenti alla bozza. Questo potrebbe comportare il rifiuto della bozza da parte di un utente senza alcuna spiegazione, in quanto l’utente non è in grado di aggiungere commenti. Utilizza invece il ruolo bozza Revisore e Approvatore in modo che l’utente possa fornire un feedback.

</br>
</br>

**Best practice**

Evita l’opzione di avviso e-mail “Tutte le attività di bozza”.

**Ecco perché**

Questa opzione invia una notifica e-mail relativa alla bozza ogni volta che si verifica un evento relativo a essa: viene inserito un commento, viene inviata una risposta, viene presa una decisione, ecc. In sostanza, il destinatario visualizza l’attività della bozza non appena si verifica.

Per i proprietari e i creatori di bozze, l’avviso e-mail Decisioni funziona meglio per i flussi di lavoro di bozza a più fasi, mentre Decisione finale funziona meglio per i flussi di lavoro a fase singola. In genere, tutti gli altri possono essere impostati su Disabilitato, a meno che non desiderino essere informati se altri utenti inseriscono commenti o decisioni (nel qual caso, una delle opzioni di e-mail di riepilogo potrebbe essere più utile).
