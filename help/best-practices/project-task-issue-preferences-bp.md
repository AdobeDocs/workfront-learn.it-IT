---
title: 'Best practice: preferenze per progetto, attività e problema'
description: Esplora le best practice consigliate dagli esperti di Adobe Workfront in merito all’impostazione, alla gestione e all’utilizzo delle preferenze per progetti, attività e problemi di Workfront.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
jira: KT-10918
exl-id: 321af897-3791-4b06-a9dd-241b5246b2a0
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '702'
ht-degree: 0%

---

# Best practice: preferenze per progetto, attività e problema

## Cos’è una &quot;best practice&quot; di Adobe Workfront?

Le best practice sono linee guida che rappresentano una linea di condotta efficace ed efficiente, sono facilmente adottabili da te e dagli utenti della tua azienda e possono essere replicate correttamente all’interno dell’organizzazione.

Mentre esamini questi consigli, tieni presente che alcune best practice di Workfront sono universali, mentre altre potrebbero essere più specifiche per l’argomento. Utilizza queste best practice come framework per guidare le impostazioni e l’utilizzo del sistema Workfront.

## Navigazione in questa pagina

Scorrendo questa pagina, troverai innanzitutto un elenco di alto livello di tutte le best practice per l’argomento. Questo ti consente di rivedere i consigli senza immergerti nei dettagli di &quot;perché&quot;.

La sezione &quot;Perché sono queste best practice?&quot; , disponibile dopo l’elenco di alto livello, fornisce maggiori dettagli su alcune delle best practice e sul perché sono considerate un processo, uno strumento, ecc., è consigliabile implementarle con l’istanza di Workfront.

</br>
</br>

## Best practice per progetti, attività e problemi

* Impostare il tipo di durata predefinita dell&#39;attività su Semplice.

* Impostare la preferenza per lo stato di un nuovo progetto su Pianificazione o Idea, non su Corrente.

* Abilita Crea baseline automaticamente nelle preferenze globali del progetto.

* Seleziona tutte le opzioni nella sezione Casi aziendali delle preferenze di progetto del sistema.

* Nelle preferenze relative ai problemi, selezionare l&#39;opzione Aggiorna automaticamente lo stato dei problemi risolvibili quando lo stato dell&#39;oggetto risolutivo cambia.

</br>
</br>


## Perché si tratta di procedure ottimali?

**Best practice**

Impostare il tipo di durata predefinita dell&#39;attività su Semplice.

**Ecco perché**

I tipi di durata definiscono la relazione tra la durata dell&#39;attività, le ore pianificate e il numero di persone assegnate all&#39;attività.

Con l&#39;impostazione predefinita del sistema globale Semplice, tutte le attività create manualmente hanno questa durata. Le ore pianificate vengono suddivise in modo uniforme tra gli assegnatari dell&#39;attività per l&#39;intera durata. Il tipo di durata semplice può semplificare la pianificazione del progetto, in quanto consente di apportare modifiche agli assegnatari dell&#39;attività e alle ore pianificate senza influire sulla durata dell&#39;attività, sulla data di inizio pianificata o sulla data di completamento pianificata.

</br>
</br>

**Best practice**

Impostare la preferenza per lo stato di un nuovo progetto su Pianificazione o Idea, non su Corrente.

**Ecco perché**

Lo stato Attuale indica che un progetto è attivo e che il lavoro è in corso. È raro che un progetto debba trovarsi in questo stato al momento della creazione. Anche se si utilizza un modello di progetto, è necessaria una certa &quot;pianificazione&quot; per ottenere assegnazioni di attività, regolare la data di completamento pianificata del progetto e così via. Lo stato Pianificazione sopprime inoltre le notifiche agli assegnatari dei task e ai membri del team di progetto. Ricevere notifiche prima che il progetto sia in esecuzione può confondere gli interessati.

</br>
</br>

**Best practice**

Abilita Crea baseline automaticamente nelle preferenze globali del progetto.

**Ecco perché**

Ogni volta che si modifica lo stato di un progetto su Corrente, Workfront registra automaticamente una previsione del progetto. Questa &quot;istantanea&quot; del progetto fornisce informazioni cronologiche sulle modifiche apportate nel tempo al piano del progetto. Ad esempio, è possibile confrontare il piano di progetto originale con il piano corrente quando si mostra alla leadership il modo in cui lo spostamento delle priorità o lo scorrimento dell&#39;ambito ha influito sulle scadenze del progetto.

</br>
</br>

**Best practice**

Seleziona tutte le opzioni nella sezione Casi aziendali delle preferenze di progetto del sistema.

**Ecco perché**

Abilitare tutte e cinque le opzioni per consentire ai project manager, ai planner e ad altri di includere una qualsiasi di queste sezioni nel business case di un progetto. Se le opzioni non sono abilitate, non vengono visualizzate nella finestra del caso di business. Gli utenti possono lasciare vuoto uno qualsiasi dei campi se non è necessario per quel particolare progetto, ma non possono abilitare un campo a livello di progetto. Queste opzioni possono essere abilitate solo a livello globale in Configurazione.

</br>
</br>

**Best practice**

Nelle preferenze relative ai problemi, selezionare l&#39;opzione Aggiorna automaticamente lo stato dei problemi risolvibili quando lo stato dell&#39;oggetto risolutivo cambia.

**Ecco perché**

Quando un problema viene convertito in un progetto, questa preferenza &quot;collega&quot; gli stati dei due elementi. L’aggiornamento dello stato del progetto (l’oggetto di risoluzione) aggiornerà automaticamente lo stato del problema. Ciò significa che il richiedente può visualizzare l’avanzamento della propria richiesta, anche se non dispone delle autorizzazioni necessarie per visualizzare l’intero progetto in Workfront.
