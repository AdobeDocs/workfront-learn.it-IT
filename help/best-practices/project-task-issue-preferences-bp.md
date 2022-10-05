---
title: Procedure consigliate - Preferenze per progetti, attività ed problemi
description: Scopri le best practice consigliate dagli esperti di Adobe Workfront sull’impostazione, la gestione e l’utilizzo di progetti, attività e preferenze per i problemi di Workfront.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
kt: 10918
exl-id: 321af897-3791-4b06-a9dd-241b5246b2a0
source-git-commit: 444f059d3cc26d8e3074a7145bc5419407c786cf
workflow-type: tm+mt
source-wordcount: '702'
ht-degree: 0%

---

# Procedure consigliate - Preferenze per progetti, attività ed problemi

## Qual è una &quot;best practice&quot; di Adobe Workfront?

Le migliori pratiche sono linee guida che rappresentano un&#39;azione efficace ed efficiente; sono facilmente adottati da te e dagli utenti della tua azienda; e può essere replicato correttamente in tutta l’organizzazione.

Quando si esaminano queste raccomandazioni, tenere presente che alcune best practice di Workfront sono universali, mentre altre potrebbero essere più specifiche per l’argomento. Utilizza queste best practice come framework per guidare le impostazioni e l’utilizzo del sistema Workfront.

## Navigazione in questa pagina

Scorrendo questa pagina, troverai innanzitutto un elenco di alto livello contenente tutte le best practice per l’argomento. Questo ti consente di rivedere le raccomandazioni senza immergerti nei dettagli del &quot;perché&quot;.

Perché queste best practice? area, disponibile dopo l’elenco di alto livello, fornisce maggiori dettagli su alcune delle best practice e sui motivi per cui vengono considerate un processo, uno strumento, ecc., dovresti considerare l’implementazione con la tua istanza Workfront.

</br>
</br>

## Best practice relative a progetti, attività e problemi delle preferenze

* Impostare il tipo di durata predefinito dell&#39;attività su Semplice.

* Impostare la preferenza per lo stato di un nuovo progetto su Planning o Idea, non Corrente.

* Abilita Crea automaticamente linee di base nelle preferenze del progetto globale.

* Controlla tutte le opzioni nella sezione Casi aziendali delle preferenze del progetto di sistema.

* Nelle preferenze relative ai problemi, selezionare l&#39;opzione Aggiorna automaticamente lo stato del problema risolvibile quando cambia lo stato dell&#39;oggetto di risoluzione.

</br>
</br>


## Perché queste best practice sono?

**Best practice**

Impostare il tipo di durata predefinito dell&#39;attività su Semplice.

**Ecco perché**

I tipi di durata definiscono la relazione tra la durata dell&#39;attività, le ore pianificate e il numero di persone assegnate all&#39;attività.

Con Semplice come impostazione predefinita del sistema globale, tutte le attività create manualmente hanno questo tipo di durata. Le ore pianificate sono suddivise in modo uniforme tra gli assegnatari dell&#39;attività per tutta la durata. Il tipo di durata semplice consente di semplificare la pianificazione del progetto, in quanto consente di apportare modifiche agli assegnatari dell’attività e alle ore pianificate senza influire sulla durata dell’attività, sulla data di inizio pianificata o sulla data di completamento pianificato.

</br>
</br>

**Best practice**

Impostare la preferenza per lo stato di un nuovo progetto su Planning o Idea, non Corrente.

**Ecco perché**

Lo stato Corrente indica che un progetto è attivo e che il lavoro è in corso. È raro che un progetto debba trovarsi in questo stato al momento della creazione. Anche se si utilizza un modello di progetto, è necessaria una certa &quot;pianificazione&quot; per ottenere assegnazioni di attività, per regolare la data di completamento pianificato del progetto, ecc. Lo stato Planning inoltre sopprime le notifiche agli assegnatari delle attività e ai membri del team di progetto. La ricezione delle notifiche prima che il progetto sia attivo può creare confusione per i soggetti coinvolti.

</br>
</br>

**Best practice**

Abilita Crea automaticamente linee di base nelle preferenze del progetto globale.

**Ecco perché**

Ogni volta che lo stato di un progetto viene modificato in Corrente, Workfront registra automaticamente una linea di base del progetto. Questa &quot;istantanea&quot; del progetto fornisce informazioni storiche su come il piano del progetto è cambiato nel tempo. Ad esempio, è possibile confrontare il piano di progetto originale con il piano corrente quando si mostra come lo spostamento delle priorità o l&#39;aumento dell&#39;ambito abbiano inciso sulle scadenze del progetto.

</br>
</br>

**Best practice**

Controlla tutte le opzioni nella sezione Casi aziendali delle preferenze del progetto di sistema.

**Ecco perché**

Abilita tutte e cinque le opzioni per consentire ai project manager, ai pianificatori e agli altri di includere una di queste sezioni nel business case su un progetto. Se le opzioni non sono abilitate, non vengono visualizzate nella finestra del business case. Gli utenti possono lasciare vuoti uno qualsiasi dei campi se non è necessario per quel particolare progetto, ma non possono abilitare un campo a livello di progetto. Queste opzioni possono essere abilitate solo a livello globale in Configurazione.

</br>
</br>

**Best practice**

Nelle preferenze relative ai problemi, selezionare l&#39;opzione Aggiorna automaticamente lo stato del problema risolvibile quando cambia lo stato dell&#39;oggetto di risoluzione.

**Ecco perché**

Quando un problema viene convertito in un progetto, questa impostazione di preferenza &quot;collega&quot; gli stati dei due elementi. L’aggiornamento dello stato del progetto (l’oggetto di risoluzione) aggiorna automaticamente lo stato del problema. Ciò significa che il richiedente può vedere l’avanzamento della richiesta, anche se non dispone delle autorizzazioni necessarie per visualizzare l’intero progetto in Workfront.
