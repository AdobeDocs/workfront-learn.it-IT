---
title: Procedure consigliate - Stati
description: Scopri le best practice consigliate dagli esperti di Adobe Workfront sull’impostazione, la gestione e l’utilizzo degli stati di Workfront.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
kt: 10926
exl-id: c3a4fe42-339c-4063-ad67-045868bbc6b1
source-git-commit: 444f059d3cc26d8e3074a7145bc5419407c786cf
workflow-type: tm+mt
source-wordcount: '584'
ht-degree: 0%

---

# Procedure consigliate - Stati

## Qual è una &quot;best practice&quot; di Adobe Workfront?

Le migliori pratiche sono linee guida che rappresentano un&#39;azione efficace ed efficiente; sono facilmente adottati da te e dagli utenti della tua azienda; e può essere replicato correttamente in tutta l’organizzazione.

Quando si esaminano queste raccomandazioni, tenere presente che alcune best practice di Workfront sono universali, mentre altre potrebbero essere più specifiche per l’argomento. Utilizza queste best practice come framework per guidare le impostazioni e l’utilizzo del sistema Workfront.

## Navigazione in questa pagina

Scorrendo questa pagina, troverai innanzitutto un elenco di alto livello contenente tutte le best practice per l’argomento. Questo ti consente di rivedere le raccomandazioni senza immergerti nei dettagli del &quot;perché&quot;.

Perché queste best practice? area, disponibile dopo l’elenco di alto livello, fornisce maggiori dettagli su alcune delle best practice e sui motivi per cui vengono considerate un processo, uno strumento, ecc., dovresti considerare l’implementazione con la tua istanza Workfront.

</br>
</br>

## Best practice per lo stato

* Quando si rinominano gli stati predefiniti di Workfront, mantenere lo scopo originale dello stato invariato.

* Se crei uno stato di progetto personalizzato per Annullato, equipara lo stato a Morto.

* Mantenere al minimo gli stati personalizzati globali.

* Non utilizzare gli stati del progetto al posto delle attività per indicare l’avanzamento di un progetto.


</br>
</br>



## Perché queste best practice sono?

**Best practice**

Quando si rinominano gli stati predefiniti di Workfront, mantenere lo scopo originale dello stato invariato.



**Ecco perché**

Alcune azioni in Workfront vengono attivate dagli stati predefiniti del sistema. La modifica dell’intento di uno stato può influire sul comportamento di Workfront in determinate situazioni, sulla generazione di rapporti, ecc.



Ad esempio, lo stato predefinito dell’attività Completa indica a Workfront di modificare la percentuale di completamento di un’attività al 100%. Lo stato Completa consente inoltre a Workfront di sapere che il lavoro sulle attività dipendenti può iniziare. Se hai modificato il nome dello stato in Attesa, per indicare che un lavoro su un&#39;attività è in pausa, Workfront penserà che l&#39;attività sia stata completata e avvierà i passaggi successivi nel progetto.

</br>
</br>



**Best practice**

Se crei uno stato di progetto personalizzato per Annullato, equipara lo stato a Morto.



**Ecco perché**

Se si paragona Annullato con Completo, non è possibile utilizzare lo stato per annullare un progetto a meno che tutte le attività siano contrassegnate come completate e tutti i problemi siano chiusi. Ma se si paragona Cancelled con Dead, è possibile annullare il progetto senza modificare nulla nel record storico.


</br>
</br>

**Best practice**

Mantenere al minimo gli stati personalizzati globali.



**Ecco perché**

Meno è di più. Oltre a creare una manutenzione non necessaria, troppi stati personalizzati creano confusione, soprattutto quando si lavora a progetti interfunzionali. Imposta invece gli stati personalizzati specifici per un gruppo. In questo modo l&#39;ambiente Workfront è più pulito e più adatto per l&#39;espansione verso altri gruppi in futuro. Collabora con il tuo comitato di governance/sorveglianza e con le parti interessate per identificare gli stati che i gruppi della tua organizzazione devono utilizzare.


</br>
</br>

**Best practice**

Non utilizzare gli stati del progetto al posto delle attività per indicare l’avanzamento di un progetto.



**Ecco perché**

Mantenere gli stati del progetto semplici per indicare fasi di avanzamento di alto livello, come Planning, Current, Complete, ecc. Lasciare che le attività, gli stati delle attività e la percentuale di completamento dell&#39;attività indichino come procede il lavoro complessivo sul progetto. Questi indicatori a livello di attività vengono aggregati in percentuale di completamento del progetto, condizione del progetto e stato di avanzamento del progetto, tutti indicatori di avanzamento del progetto migliori e più precisi rispetto allo stato del progetto. Inoltre, queste informazioni a livello di attività forniscono una migliore generazione di rapporti sui progetti.
