---
title: Inserisci i dettagli del progetto
description: Scopri quali 12 campi di dettagli del progetto [!DNL  Workfront] consiglia di compilare il modulo durante la creazione di un progetto.
feature: Work Management
thumbnail: fill-in-the-project-details.jpeg
type: Tutorial
role: User
level: Intermediate
kt: 10140
exl-id: a62b9421-627a-4f23-ab66-da1f29114225
source-git-commit: 27e8f0aada77488bd6cfc2e786b997f759fd0a17
workflow-type: tm+mt
source-wordcount: '1226'
ht-degree: 1%

---

# Inserisci i dettagli del progetto

Non preoccuparti ... non devi compilare tutti i campi e le caselle di controllo nei dettagli del progetto con ogni progetto creato in [!DNL  Workfront]. Utilizza i modelli per precompilare le informazioni, quindi fai attenzione ai 12 campi più importanti per i dettagli del progetto elencati di seguito.

1. **Nome**

   Un nome descrittivo del progetto aiuta tutti a identificare lo scopo del progetto. Accertati di seguire la convenzione per la denominazione dei progetti della tua organizzazione, che potrebbe richiedere l’inclusione di determinate informazioni nel nome del progetto (ad esempio un numero di riferimento, un nome di reparto o un indicatore di categoria).

1. **Descrizione**

   Quando più persone lavorano su un progetto, in qualità di project manager dovrai accertarti che tutti siano al passo con lo scopo e le aspettative del progetto.

   A tale scopo, inserisci una descrizione del progetto che fornisce informazioni di base, risponde alle domande e consente al team di progetto di proseguire il proprio lavoro. Ad esempio, &quot;Una campagna mirata ad aumentare del 50% i ricavi che generano lavoro&quot; o &quot;Nuovo aggiornamento del sistema per migliorare l&#39;efficienza in tutto il dipartimento&quot;.

   Alcuni clienti Workfront includono un esempio di come dovrebbe essere una descrizione del progetto nei loro modelli di progetto.

1. **Stato**

   Lo stato viene utilizzato in Workfront per indicare la posizione o la fase del flusso di lavoro in cui si trova un progetto. Lo stato viene utilizzato in molti rapporti di Workfront per monitorare l’avanzamento del lavoro.

   Workfront consiglia di impostare lo stato su Planning durante la compilazione e la finalizzazione del piano di progetto. Lo stato Planning indica che le notifiche di Workfront non vengono inviate agli assegnatari delle attività relative al progetto mentre si trova in questo stato.

   Quindi, quando il progetto è pronto per essere live, cambia lo stato in Corrente. Questo accade quando Workfront invia notifiche alle persone appropriate sulle attività a cui sono state assegnate.

   >[!TIP]
   >
   >  Quando si apportano modifiche al progetto, ad esempio se si modificano le date di scadenza, è possibile riportare lo stato su Planning oppure disattivare la funzione di salvataggio automatico per impedire che le notifiche vengano inviate fino al completamento delle modifiche.

   L&#39;amministratore di sistema può impostare lo stato Planning come predefinito globale di Workfront.

1. **Modalità Schedule**

   I progetti Workfront possono essere pianificati a partire da una data di inizio o da una data di completamento. Tale selezione importante determina il modo in cui vengono calcolate le date pianificate di ciascuna attività.

   L’opzione Data inizio considera la data di inizio del progetto, immessa dall’utente, nonché la durata e i predecessori di ogni attività per calcolare la data di fine del progetto. Workfront consiglia di utilizzare questa opzione, in quanto è la più comune e semplifica la pianificazione delle date del progetto.

   Tuttavia, puoi utilizzare una data di completamento. Workfront esamina la data di fine (inserita dall’utente) e il lavoro da eseguire (in base a durate e predecessori), quindi lavora all’indietro per calcolare la data di inizio del progetto. Workfront consiglia di attendere la data di completamento dopo aver stabilito un certo livello di competenza in Workfront.

   A prescindere dall’opzione scelta, non dimenticare di selezionare una data dal calendario a comparsa.

   L’opzione Modalità pianificazione può essere impostata nel modello.

1. **Gruppo**

   Un gruppo è un’unità organizzativa Workfront che spesso si allinea a un reparto. Questo campo può essere impostato sul modello di progetto. Se non lo è, il campo viene impostato automaticamente sul Gruppo Home della persona che crea il progetto. È possibile modificare il gruppo in base alle esigenze.

   In generale, la maggior parte delle persone che lavorano al progetto provengono da questo gruppo. Ma questo non limita le persone da altri gruppi a cui viene assegnato il lavoro nel progetto.

   Il gruppo del progetto determina inoltre quale progetto, attività ed emette le preferenze che il progetto utilizzerà. Queste preferenze, ad esempio lo stato personalizzato di un gruppo specifico, vengono impostate dall’amministratore di sistema o da un amministratore di gruppo.

   L&#39;impostazione di gruppo è un modo conveniente, attraverso il reporting, per mostrare tutti i progetti su cui un reparto sta lavorando.

1. **Proprietario progetto**

   Il proprietario del progetto è il termine di Workfront per project manager. Responsabile della pianificazione e/o della gestione del progetto.

   Il proprietario del progetto dispone di autorizzazioni di gestione complete per il progetto, pertanto deve disporre di una licenza di piano.

   Normalmente questo campo viene lasciato vuoto nel modello e viene compilato automaticamente con il nome della persona che crea il progetto. Se nel modello viene immesso un nome, è il proprietario predefinito del progetto.

1. **Sponsor Progetto**

   In genere, lo sponsor del progetto è la persona che ha richiesto il progetto. Spesso si tratta di un soggetto interno, come un dirigente o un dirigente, con responsabilità complessiva per il progetto.

   Lo sponsor riceve automaticamente le autorizzazioni di visualizzazione per il progetto e deve essere un utente con licenza Workfront.

   Lo sponsor del progetto può essere impostato nel modello.

1. **Responsabile risorse**

   Gli utenti Workfront elencati in questo campo possono utilizzare gli strumenti di pianificazione e gestione delle risorse in Workfront per i progetti specifici in cui sono elencati. È possibile elencare fino a 30 nomi nel campo Gestione risorse e ciascuno deve disporre di una licenza Piano.

   Il campo Gestione risorse può essere impostato nel modello.

1. **Moduli personalizzati**

   Workfront fornisce campi nativi per elementi quali il nome del progetto e la data di inizio. Tuttavia, è necessario disporre di ulteriori informazioni in qualità di project manager o che il team di progetto avrà bisogno di. I tuoi dati unici sono ugualmente importanti ed è facilmente memorizzabile in questi moduli. Dettagli come date di pubblicazione, dimensioni delle risorse di stampa, canali di consegna e altro ancora.

   I moduli personalizzati possono acquisire queste informazioni e possono essere inclusi negli elenchi e nei rapporti di Workfront, semplificando la visualizzazione e la modifica delle informazioni.

   I moduli personalizzati possono essere allegati ai modelli in anticipo.

1. **Pianificazione**

   Il lavoro avviene 24 ore su 24, come molte aziende hanno dipendenti in tutto il mondo.

   Workfront consente di applicare ai progetti una pianificazione comune. Questi vengono creati dall’amministratore di sistema. Le pianificazioni riflettono i giorni e le ore lavorative dei team, oltre ai giorni in cui i dipendenti non lavoreranno (ad esempio le vacanze).

   In qualità di pianificatore, assicurati di applicare la pianificazione corretta al progetto corretto. Le impostazioni della pianificazione influiscono sul calcolo della timeline, tenendo conto del tempo di inattività e dei fusi orari.

   La pianificazione assegnata al progetto deve essere quella che si applica alla maggior parte degli assegnatari delle attività. Se non è specificata alcuna pianificazione per il progetto, verrà utilizzata la pianificazione contrassegnata come Predefinito.

   La pianificazione può essere impostata nel modello.

1. **Gruppi di risorse**

   I pool di risorse sono raccolte di utenti Workfront che sono necessari allo stesso tempo per il completamento dei progetti nella tua organizzazione. Un pool di risorse può essere assegnato a più progetti, il che significa che i progetti sono in competizione per le risorse.

   L’assegnazione di pool di risorse a un progetto è un prerequisito per l’utilizzo di Resource Planner e di altri strumenti di gestione delle risorse in Workfront.

   Nel modello è possibile impostare un pool di risorse predefinito.

1. **Accesso al progetto per visualizzatori e collaboratori**

   Quando un utente ha accesso a un progetto, possono inizialmente ottenere tre livelli di autorizzazioni: Visualizza, Contribuisce e Gestisci. Ogni livello di autorizzazione consente all’utente di visualizzare e eseguire determinate operazioni con il progetto.

   Ad esempio, ci sono persone che potrebbero avere accesso al progetto ma non dovrebbero visualizzare le informazioni finanziarie. Per disattivare l’opzione Visualizza contabilità per visualizzatori e collaboratori.

   Puoi regolare in modo preciso queste impostazioni delle autorizzazioni per i singoli progetti in qualsiasi momento. Tuttavia, una volta che un progetto è passato dallo stato Planning allo stato attuale, è necessario eseguire regolazioni basate sulle autorizzazioni tramite la condivisione del progetto.

   Le impostazioni di accesso possono essere impostate nel modello.
