---
title: Best practice - Stati
description: Esplora le best practice consigliate dagli esperti Adobe Workfront in merito all’impostazione, alla gestione e all’utilizzo degli stati di Workfront.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
jira: KT-10926
exl-id: c3a4fe42-339c-4063-ad67-045868bbc6b1
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '584'
ht-degree: 0%

---

# Best practice - Stati

## Cos’è una &quot;best practice&quot; di Adobe Workfront?

Le best practice sono linee guida che rappresentano una linea di condotta efficace ed efficiente, sono facilmente adottabili da te e dagli utenti della tua azienda e possono essere replicate correttamente all’interno dell’organizzazione.

Mentre esamini questi consigli, tieni presente che alcune best practice di Workfront sono universali, mentre altre potrebbero essere più specifiche per l’argomento. Utilizza queste best practice come framework per guidare le impostazioni e l’utilizzo del sistema Workfront.

## Navigazione in questa pagina

Scorrendo questa pagina, troverai innanzitutto un elenco di alto livello di tutte le best practice per l’argomento. Questo ti consente di rivedere i consigli senza immergerti nei dettagli di &quot;perché&quot;.

La sezione &quot;Perché sono queste best practice?&quot; , disponibile dopo l’elenco di alto livello, fornisce maggiori dettagli su alcune delle best practice e sul perché sono considerate un processo, uno strumento, ecc., è consigliabile implementarle con l’istanza di Workfront.

</br>
</br>

## Best practice per gli stati

* Quando rinomini gli stati predefiniti di Workfront, mantieni lo scopo originale dello stato.

* Se crei uno stato di progetto personalizzato per Annullato, imposta lo stato su Inattivo.

* Mantieni al minimo gli stati personalizzati globali.

* Non utilizzare gli stati del progetto invece delle attività per indicare la progressione di un progetto.


</br>
</br>



## Perché si tratta di procedure ottimali?

**Best practice**

Quando rinomini gli stati predefiniti di Workfront, mantieni lo scopo originale dello stato.



**Ecco perché**

Alcune azioni in Workfront vengono attivate dagli stati predefiniti del sistema. La modifica dell’intento di uno stato può influire sul comportamento di Workfront in determinate situazioni, influire sulla generazione di rapporti, ecc.



Ad esempio, lo stato predefinito dell&#39;attività Completo indica a Workfront di impostare su 100% la percentuale di completamento di un&#39;attività. Lo stato Completo consente inoltre a Workfront di sapere che può iniziare il lavoro sulle attività dipendenti. Se hai cambiato il nome dello stato in In attesa, per indicare che un lavoro su un’attività è in pausa, Workfront penserà che l’attività sia terminata e avvierà i passaggi successivi del progetto.

</br>
</br>



**Best practice**

Se crei uno stato di progetto personalizzato per Annullato, imposta lo stato su Inattivo.



**Ecco perché**

Se si associa Annullato a Completo, non è possibile utilizzare lo stato per annullare un progetto a meno che tutte le attività non siano contrassegnate come completate e tutti i problemi siano chiusi. Tuttavia, se si associa Annullato a Inattivo, è possibile annullare il progetto senza modificare nulla nel record cronologico.


</br>
</br>

**Best practice**

Mantieni al minimo gli stati personalizzati globali.



**Ecco perché**

Meno è di più. Oltre a creare una manutenzione non necessaria, troppi stati personalizzati creano confusione, soprattutto quando si lavora su progetti cross-functional. Rendi invece specifici i gruppi di stati personalizzati. In questo modo l&#39;ambiente Workfront sarà più pulito e posizionato meglio per l&#39;espansione futura ad altri gruppi. Collabora con il tuo comitato di governance/supervisione e le parti interessate per identificare gli stati che i gruppi della tua organizzazione devono utilizzare.


</br>
</br>

**Best practice**

Non utilizzare gli stati del progetto invece delle attività per indicare la progressione di un progetto.



**Ecco perché**

Mantenere semplici gli stati del progetto per indicare le fasi di avanzamento di alto livello, come Pianificazione, Corrente, Completa, ecc. Le attività, gli stati delle attività e la percentuale di completamento delle attività indicano lo stato complessivo del lavoro del progetto. Questi indicatori a livello di attività vengono aggregati nella percentuale di completamento del progetto, nella condizione del progetto e nello stato di avanzamento del progetto, tutti indicatori migliori e più precisi dell&#39;avanzamento del progetto rispetto allo stato del progetto. Inoltre, queste informazioni a livello di attività forniscono una migliore generazione di rapporti sui progetti.
