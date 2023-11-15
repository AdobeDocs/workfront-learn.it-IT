---
title: Inserisci i dettagli del progetto
description: Scopri quali 12 campi dei dettagli del progetto [!DNL  Workfront] consiglia di compilare durante la creazione di un progetto.
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: fill-in-the-project-details.jpeg
type: Tutorial
role: User
level: Beginner
jira: KT-10140
exl-id: a62b9421-627a-4f23-ab66-da1f29114225
source-git-commit: ec82cd0aafb89df7b3c46eb716faf3a25cd438a2
workflow-type: tm+mt
source-wordcount: '1219'
ht-degree: 1%

---

# Inserisci i dettagli del progetto

Non preoccuparti ... non devi compilare ogni campo e casella di controllo nei dettagli del progetto con ogni progetto creato in [!DNL  Workfront]. Utilizza i modelli per precompilare le informazioni, quindi rivolgi la tua attenzione ai 12 campi più importanti dei dettagli del progetto elencati di seguito.

1. **Nome**

   Un nome descrittivo del progetto consente a tutti di identificare lo scopo del progetto. Assicurati di seguire la convenzione di denominazione dei progetti della tua organizzazione, che potrebbe richiedere l’inclusione di determinate informazioni nel nome del progetto (ad esempio un numero di riferimento, il nome del reparto o un indicatore di categoria).


1. **Descrizione**

   Quando più persone lavorano a un progetto, tu, in qualità di project manager, devi assicurarti che tutti siano al corrente dello scopo e delle aspettative del progetto.

   A tale scopo, utilizzare una descrizione del progetto che fornisca informazioni di base, risponda alle domande e consenta al team di progetto di proseguire il proprio lavoro. Ad esempio, &quot;Una campagna mirata ad aumentare del 50% il lavoro generatore di ricavi&quot; o &quot;Un nuovo aggiornamento del sistema per migliorare l&#39;efficienza in tutto il reparto&quot;.

   Alcuni clienti di Workfront includono un esempio di descrizione di un progetto nei loro modelli di progetto.

1. **Stato**

   Lo stato viene utilizzato in Workfront per indicare dove o in quale fase del flusso di lavoro si trova un progetto. Lo stato viene utilizzato in molti rapporti di Workfront per monitorare l’avanzamento del lavoro.

   Workfront consiglia di impostare lo stato su Planning durante la definizione e la finalizzazione del piano di progetto. L&#39;elemento chiave con lo stato Pianificazione è che le notifiche di Workfront non vengono inviate agli assegnatari dell&#39;attività sul progetto mentre si trova in questo stato.

   Quindi, una volta che il progetto è pronto per andare live, modifica lo stato su Corrente. Questo consente a Workfront di inviare notifiche alle persone sulle nuove attività a cui sono assegnate, ma non invierà notifiche agli utenti per le attività a cui sono state assegnate mentre il progetto era in stato Pianificazione.

   >[!TIP]
   >
   >  Quando si apportano modifiche al progetto, ad esempio la modifica delle date di scadenza, è possibile ripristinare lo stato su Planning oppure disattivare la funzione Salvataggio automatico per impedire che le notifiche vengano inviate fino al completamento delle modifiche.

   L&#39;amministratore di sistema può impostare lo stato Pianificazione come predefinito globale di Workfront per i nuovi progetti.

1. **Modalità pianificazione**

   I progetti Workfront possono essere programmati da una data di inizio o una data di completamento. Questa selezione importante determina il modo in cui vengono calcolate le date pianificate di ogni attività.

   L&#39;opzione Data inizio consente di calcolare la data di inizio del progetto, inserita dall&#39;utente, nonché la durata e i predecessori di ogni attività. Workfront consiglia di utilizzare questa opzione, in quanto è la più comune e semplifica la pianificazione delle date dei progetti.

   Tuttavia, puoi utilizzare una data di completamento. Workfront esamina la data di fine (inserita dall’utente) e il lavoro da eseguire (in base alle durate e ai predecessori), quindi lavora all’indietro per calcolare la data di inizio del progetto. Workfront consiglia di attendere la data di completamento dopo aver stabilito un determinato livello di esperienza in Workfront.

   Indipendentemente dall&#39;opzione scelta, non dimenticare di selezionare una data dal calendario popup.

   L&#39;opzione Modalità di pianificazione può essere impostata nel modello.

1. **Gruppo**

   Un gruppo è un&#39;unità organizzativa di Workfront che spesso si allinea a un reparto. Questo campo può essere impostato sul modello di progetto. In caso contrario, il campo viene impostato automaticamente sul Gruppo predefinito della persona che crea il progetto. È possibile modificare il gruppo in base alle esigenze.

   Generalmente, la maggior parte delle persone che lavorano al progetto provengono da questo gruppo. Ma questo non limita le persone di altri gruppi a cui viene assegnato il lavoro nel progetto.

   Il Gruppo del progetto determina anche le preferenze di progetto, attività e problema che il progetto utilizzerà. Queste preferenze, ad esempio uno stato personalizzato per un gruppo specifico, vengono impostate dall&#39;amministratore di sistema o da un amministratore di gruppo.

   L&#39;impostazione del gruppo è un modo pratico, attraverso la generazione di rapporti, per mostrare tutti i progetti su cui un reparto sta lavorando.

1. **Proprietario progetto**

   Proprietario del progetto è il termine utilizzato da Workfront per project manager. Si tratta della persona responsabile della pianificazione e/o della gestione del progetto.

   Affinché il proprietario del progetto possa disporre delle autorizzazioni di gestione complete per il progetto, deve disporre di una licenza Pianificazione.

   Normalmente questo campo viene lasciato vuoto nel modello e viene compilato automaticamente con il nome della persona che ha creato il progetto. Se nel modello viene immesso un nome, si tratta del proprietario predefinito del progetto.

1. **Sponsor Progetto**

   Lo sponsor del progetto non è obbligatorio, ma quando viene utilizzato è generalmente la persona che ha richiesto il progetto. Si tratta spesso di un soggetto interessato interno, come un manager o un dirigente, con responsabilità generale per il progetto.

   Lo sponsor riceve automaticamente le autorizzazioni di visualizzazione per il progetto e deve essere un utente con licenza Workfront.

   Lo sponsor del progetto può essere impostato nel modello.

1. **Responsabile risorse**

   Gli utenti di Workfront elencati in questo campo possono utilizzare gli strumenti di gestione e pianificazione delle risorse di Workfront per i progetti specifici in cui sono elencati. Nel campo Responsabile risorse è possibile elencare fino a 30 nomi, ognuno dei quali deve disporre di una licenza Pianificazione.

   Il campo Responsabile risorse può essere impostato nel modello.

1. **Moduli personalizzati**

   In Workfront sono disponibili campi nativi per elementi quali il nome del progetto e la data di inizio. Tuttavia, sono necessarie ulteriori informazioni in qualità di project manager o per il team del progetto. I dati univoci sono ugualmente importanti e possono essere facilmente archiviati in questi moduli. Dettagli come date di pubblicazione, dimensioni delle risorse di stampa, canali di consegna, ecc.

   I moduli personalizzati possono acquisire queste informazioni e possono essere inclusi in elenchi e report in Workfront, semplificandone la visualizzazione e la modifica.

   I moduli personalizzati possono essere allegati in anticipo ai modelli.

1. **Pianificazione**

   Il lavoro è ininterrotto, dato che molte aziende hanno dipendenti in tutto il mondo.

   Workfront consente di applicare ai progetti una pianificazione comune. Vengono create dall&#39;amministratore di sistema. Le pianificazioni riflettono i giorni e le ore lavorative dei team, più i giorni in cui i dipendenti non saranno al lavoro (come le ferie).

   In qualità di planner, assicurati di applicare la pianificazione corretta al progetto corretto. Le impostazioni della pianificazione influiscono sui calcoli della sequenza temporale, tenendo conto del tempo libero e dei fusi orari.

   La pianificazione assegnata al progetto deve essere quella che si applica alla maggior parte degli assegnatari dell&#39;attività. Se non è stata specificata alcuna pianificazione per il progetto, verrà utilizzata la pianificazione contrassegnata come Predefinita.

   La pianificazione può essere impostata nel modello.

1. **Gruppi di risorse**

   I gruppi di risorse sono insiemi di utenti Workfront necessari contemporaneamente per il completamento dei progetti all’interno dell’organizzazione. Un pool di risorse può essere assegnato a più progetti, il che significa che si dispone di progetti in competizione per le risorse.

   L’assegnazione di pool di risorse a un progetto è un prerequisito per l’utilizzo della pianificazione delle risorse e di altri strumenti di gestione delle risorse in Workfront.

   È possibile impostare un pool di risorse predefinito nel modello.

1. **Accesso al progetto per visualizzatori e collaboratori**

   Quando a un utente viene concesso l&#39;accesso a un progetto tramite Condividi, è possibile assegnare tre livelli di autorizzazione: Visualizza, Contribuisci e Gestisci. Ogni livello di autorizzazione consente all’utente di visualizzare ed eseguire determinate operazioni con il progetto.

   Ad esempio, ci sono persone che potrebbero avere accesso al progetto ma non dovrebbero vedere le informazioni finanziarie. In questo modo è possibile disattivare l&#39;opzione Visualizza contabilità.

   Le impostazioni di accesso possono essere impostate nel modello.
