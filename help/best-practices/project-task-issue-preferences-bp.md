---
title: Best practice - Preferenze per progetti, attività e problemi
description: Esplora le best practice consigliate dagli esperti di Adobe Workfront in merito all’impostazione, alla gestione e all’utilizzo delle preferenze per progetti, attività e problemi di Workfront.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
jira: KT-10918
exl-id: 321af897-3791-4b06-a9dd-241b5246b2a0
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '702'
ht-degree: 100%

---

# Best practice - Preferenze per progetti, attività e problemi

## Che cos’è una “best practice” di Adobe Workfront?

Le best practice sono linee guida che rappresentano una linea d’azione efficace ed efficiente; sono facilmente adottabili da te e dagli utenti della tua azienda; e possono essere replicate con successo in tutta l’organizzazione.

Mentre esamini questi consigli, tieni presente che alcune best practice di Workfront sono universali mentre altre potrebbero essere più specifiche per un dato argomento. Utilizza queste best practice come una base comune per le impostazioni e l’utilizzo del sistema Workfront.

## Esplorazione di questa pagina

Mentre scorri questa pagina, troverai innanzitutto un elenco di alto livello di tutte le best practice per questo argomento. Questo ti consente di rivedere i consigli senza entrare nei dettagli del “perché”.

La sezione “Perché queste sono best practice?”, che si trova dopo l’elenco di alto livello, fornisce maggiori dettagli su alcune delle best practice e sul motivo per cui sono considerate un processo, uno strumento ecc. da implementare con la tua istanza di Workfront.

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

Uno stato corrente indica che un progetto è in esecuzione e il lavoro viene svolto attivamente. È raro che un progetto debba trovarsi in questo stato al momento della creazione. Anche se utilizzi un modello di progetto, è necessaria una certa “pianificazione” per ottenere le assegnazioni delle attività, modificare la data di completamento pianificata del progetto, ecc. Lo stato Pianificazione elimina inoltre le notifiche agli assegnatari dell’attività e ai membri del team del progetto. Ricevere notifiche prima che il progetto sia in esecuzione può confondere gli interessati.

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
