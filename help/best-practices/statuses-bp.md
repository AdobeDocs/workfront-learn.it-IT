---
title: Best practice - Stati
description: Esplora le best practice consigliate dagli esperti di Adobe Workfront in merito all’impostazione, alla gestione e all’utilizzo degli stati di Workfront.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
jira: KT-10926
exl-id: c3a4fe42-339c-4063-ad67-045868bbc6b1
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 100%

---

# Best practice - Stati

## Che cos’è una “best practice” di Adobe Workfront?

Le best practice sono linee guida che rappresentano una linea d’azione efficace ed efficiente; sono facilmente adottabili da te e dagli utenti della tua azienda; e possono essere replicate con successo in tutta l’organizzazione.

Mentre esamini questi consigli, tieni presente che alcune best practice di Workfront sono universali mentre altre potrebbero essere più specifiche per un dato argomento. Utilizza queste best practice come una base comune per le impostazioni e l’utilizzo del sistema Workfront.

## Esplorazione di questa pagina

Mentre scorri questa pagina, troverai innanzitutto un elenco di alto livello di tutte le best practice per questo argomento. Questo ti consente di rivedere i consigli senza entrare nei dettagli del “perché”.

La sezione “Perché queste sono best practice?”, che si trova dopo l’elenco di alto livello, fornisce maggiori dettagli su alcune delle best practice e sul motivo per cui sono considerate un processo, uno strumento ecc. da implementare con la tua istanza di Workfront.

</br>
</br>

## Best practice per gli stati

* Quando rinomini gli stati predefiniti di Workfront, mantieni lo scopo originale dello stato.

* Ad esempio, se crei uno stato di progetto personalizzato per Annullato, impostalo come equivalente di Inattivo.

* Mantieni al minimo gli stati personalizzati globali.

* Non utilizzare gli stati del progetto invece delle attività per indicare l’avanzamento di un progetto.


</br>
</br>



## Perché queste sono best practice?

**Best practice**

Quando rinomini gli stati predefiniti di Workfront, mantieni lo scopo originale dello stato.



**Ecco perché**

Alcune azioni in Workfront vengono attivate dagli stati predefiniti del sistema. Se si cambia l’intento di uno stato, questo può influire sul comportamento di Workfront in determinate situazioni, sulla generazione di rapporti, ecc.



Ad esempio, lo stato predefinito Completato per le attività indica a Workfront di impostare su 100% la percentuale di completamento di un’attività. Lo stato Completato consente inoltre a Workfront di sapere quando può avere inizio il lavoro sulle attività dipendenti. Se cambi il nome di questo stato in “In attesa”, per indicare che un lavoro su un’attività è in pausa, Workfront penserà comunque che l’attività sia terminata e avvierà i passaggi successivi del progetto.

</br>
</br>



**Best practice**

Ad esempio, se crei uno stato di progetto personalizzato per Annullato, impostalo come equivalente di Inattivo.



**Ecco perché**

Se associ Annullato a Completato, non potrai utilizzare lo stato per annullare un progetto a meno che tutte le attività non siano contrassegnate come completate e tutti i problemi non siano stati chiusi. Se invece associ Annullato a Inattivo, potrai annullare il progetto senza modificare nulla nel record cronologico.


</br>
</br>

**Best practice**

Mantieni al minimo gli stati personalizzati globali.



**Ecco perché**

Meno è meglio. Oltre a richiedere più manutenzione, troppi stati personalizzati creano confusione, soprattutto quando si lavora su progetti cross-functional. Piuttosto, crea stati personalizzati per specifici gruppi. In questo modo l’ambiente Workfront sarà più pulito e sarà più facile estenderlo in futuro ad altri gruppi. Collabora con il tuo comitato di governance/supervisione e le parti interessate per individuare gli stati che dovranno essere utilizzati dai gruppi della tua organizzazione.


</br>
</br>

**Best practice**

Non utilizzare gli stati del progetto invece delle attività per indicare l’avanzamento di un progetto.



**Ecco perché**

Usa gli stati del progetto per indicare semplicemente le fasi di avanzamento di alto livello, come Pianificazione, Corrente, Completato, ecc. Usa invece le attività, gli stati delle attività e la percentuale di completamento delle attività per conoscere l’avanzamento complessivo del lavoro del progetto. Questi indicatori a livello di attività vengono aggregati nella percentuale di completamento del progetto, nella condizione del progetto e nello stato di avanzamento del progetto, tutti indicatori migliori e più precisi dell’avanzamento del progetto rispetto allo stato del progetto. Inoltre, queste informazioni a livello di attività forniscono rapporti migliori sui progetti.
