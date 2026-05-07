---
title: Best practice - Preferenze per progetti, attività e problemi
description: Esplora le best practice consigliate dagli esperti di Adobe Workfront in merito all’impostazione, alla gestione e all’utilizzo delle preferenze per progetti, attività e problemi di Workfront.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
jira: KT-10918
exl-id: 321af897-3791-4b06-a9dd-241b5246b2a0
TQID: https://experienceleague.adobe.com/2Nc0Sj-3xZ-H8ir2OvXLhRJFEEKZu0DM8jIbFvizqlM
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bdid: f8a45b24-4be7-4f1b-909b-60d06b483a20
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 36674ed53c8645f556862bb2d99f3bfd6c993c1e
workflow-type: tm+mt
source-wordcount: 704
ht-degree: 89%

---

# Best practice - Preferenze per progetti, attività e problemi

## Che cos’è una “best practice” di Adobe Workfront?

Le best practice sono linee guida che rappresentano una linea d’azione efficace ed efficiente; sono facilmente adottabili da te e dagli utenti della tua azienda; e possono essere replicate con successo in tutta l’organizzazione.

Mentre esamini questi consigli, tieni presente che alcune best practice di Workfront sono universali mentre altre potrebbero essere più specifiche per un dato argomento. Utilizza queste best practice come una base comune per le impostazioni e l’utilizzo del sistema Workfront.

## Esplorazione di questa pagina

Mentre scorri questa pagina, troverai innanzitutto un elenco di alto livello di tutte le best practice per questo argomento. Questo ti consente di rivedere i consigli senza entrare nei dettagli del “perché”.

L’area &quot;Perché queste best practice?&quot;, che si trova dopo l’elenco di alto livello, fornisce maggiori dettagli su alcune delle best practice e sul perché vengono considerate un processo, uno strumento, ecc., è consigliabile implementarle con l’istanza di Workfront.

</br>
</br>

## Best practice per progetti, attività e problemi

* Imposta il tipo di durata predefinita dell’attività su Semplice.

* Imposta la preferenza per lo stato di un nuovo progetto su Pianificazione o Idea, non su Corrente.

* Abilita Crea baseline automaticamente nelle preferenze globali del progetto.

* Seleziona tutte le opzioni nella sezione Casi di business delle preferenze del progetto del sistema.

* Nelle preferenze relative ai problemi, verifica l’opzione Aggiorna automaticamente lo stato dei problemi risolvibili quando lo stato dell’oggetto di risoluzione cambia.

</br>
</br>


## Perché queste sono best practice?

**Best practice**

Imposta il tipo di durata predefinita dell’attività su Semplice.

**Ecco perché**

I tipi di durata definiscono la relazione tra la durata dell’attività, le ore pianificate e il numero di persone assegnate all’attività.

Con Semplice come impostazione predefinita per il sistema globale, tutte le attività create manualmente hanno questo tipo di durata. Le ore pianificate vengono divise equamente tra gli assegnatari dell’attività per tutta la durata. Il tipo di durata Semplice può semplificare la pianificazione del progetto, in quanto consente di apportare modifiche agli assegnatari dell’attività e alle ore pianificate senza influire sulla durata dell’attività, sulla data di inizio pianificata o sulla data di completamento pianificata.

</br>
</br>

**Best practice**

Imposta la preferenza per lo stato di un nuovo progetto su Pianificazione o Idea, non su Corrente.

**Ecco perché**

Uno stato corrente indica che un progetto è in esecuzione e il lavoro viene svolto attivamente. È raro che un progetto debba trovarsi in questo stato al momento della creazione. Anche se si utilizza un modello di progetto, è necessaria una certa &quot;pianificazione&quot; per ottenere assegnazioni di attività, regolare la data di completamento pianificata del progetto e così via. Lo stato Pianificazione sopprime inoltre le notifiche agli assegnatari dei task e ai membri del team di progetto. Ricevere notifiche prima che il progetto sia in esecuzione può confondere gli interessati.

</br>
</br>

**Best practice**

Abilita Crea baseline automaticamente nelle preferenze globali del progetto.

**Ecco perché**

Ogni volta che modifichi lo stato di un progetto in Corrente, Workfront registra automaticamente una baseline del progetto. Questa “istantanea” del progetto fornisce informazioni storiche su come il piano del progetto è cambiato nel tempo. Ad esempio, è possibile confrontare il piano del progetto originale con il piano corrente per mostrare alla leadership il modo in cui lo spostamento delle priorità o la deviazione dall’ambito del progetto ha influito sulle scadenze.

</br>
</br>

**Best practice**

Seleziona tutte le opzioni nella sezione Casi di business delle preferenze del progetto del sistema.

**Ecco perché**

Abilita tutte le cinque opzioni per consentire a project manager, responsabili della pianificazione e altri di includere una qualsiasi di queste sezioni nel caso di business di un progetto. Se le opzioni non sono abilitate, non verranno visualizzate nella finestra del caso di business. Gli utenti possono lasciare vuoti i campi se questi non sono necessari per quel particolare progetto, ma non possono abilitare un campo a livello di progetto. Queste opzioni possono essere abilitate solo a livello globale in Configurazione.

</br>
</br>

**Best practice**

Nelle preferenze relative ai problemi, verifica l’opzione Aggiorna automaticamente lo stato dei problemi risolvibili quando lo stato dell’oggetto di risoluzione cambia.

**Ecco perché**

Quando un problema viene convertito in un progetto, questa impostazione di preferenza “collega” gli stati dei due elementi. L’aggiornamento dello stato del progetto (l’oggetto di risoluzione) aggiornerà automaticamente lo stato del problema. Ciò significa che il richiedente può visualizzare l’avanzamento della propria richiesta, anche se non dispone delle autorizzazioni necessarie per visualizzare l’intero progetto in Workfront.
