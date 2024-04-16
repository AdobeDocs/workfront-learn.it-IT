---
title: Compilare i dettagli del progetto
description: Scopri quali 12 campi dei dettagli del progetto  [!DNL  Workfront]  consiglia di compilare durante la creazione di un progetto.
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: fill-in-the-project-details.jpeg
type: Tutorial
role: User
level: Beginner
recommendations: noDisplay,noCatalog
jira: KT-10140
exl-id: a62b9421-627a-4f23-ab66-da1f29114225
source-git-commit: c2ba2ddfbbc642398a0136ecbf7c3613208080c4
workflow-type: tm+mt
source-wordcount: '1252'
ht-degree: 97%

---

# Compilare i dettagli del progetto

Non preoccuparti ... non devi compilare tutti i campi e le caselle di controllo nei dettagli del progetto con ogni progetto creato in [!DNL  Workfront]. Utilizza i modelli per precompilare le informazioni, quindi rivolgi la tua attenzione ai 12 campi più importanti dei dettagli del progetto elencati di seguito.

1. **Nome**

   Un nome del progetto descrittivo consente a tutti di identificare lo scopo del progetto. Assicurati di seguire la convenzione di denominazione dei progetti dell’organizzazione, che potrebbe richiedere l’inclusione di determinate informazioni nel nome del progetto (ad esempio un numero di riferimento, il nome del reparto o un indicatore di categoria).


1. **Descrizione**

   Quando più persone lavorano a un progetto, tu, in qualità di project manager, devi assicurarti che tutti siano al corrente dello scopo e delle aspettative del progetto.

   A tale scopo, utilizza una descrizione del progetto che fornisca informazioni di base, risponda alle domande e consenta al team di progetto di proseguire il proprio lavoro. Ad esempio, “Campagna mirata ad aumentare del 50% il lavoro che genera entrate” o “Nuovo aggiornamento del sistema per migliorare l’efficienza in tutto il reparto”.

   Alcuni clienti di Workfront includono un esempio di descrizione di un progetto nei loro modelli di progetto.

1. **Stato**

   Lo stato viene utilizzato in Workfront per indicare dove o in quale fase del flusso di lavoro si trova un progetto. Lo stato viene utilizzato in molti rapporti di Workfront per monitorare l’avanzamento del lavoro.

   Workfront consiglia di impostare lo stato su Pianificazione durante la definizione e la finalizzazione del piano del progetto. L’aspetto fondamentale dello stato Pianificazione è che quando il progetto si trova in questo stato le notifiche di Workfront non vengono inviate agli assegnatari dell’attività sul progetto.

   Quindi, una volta che il progetto è pronto per essere avviato, modifica lo stato su Corrente. Questo consente a Workfront di inviare notifiche alle persone sulle nuove attività a cui sono assegnate, ma non invierà notifiche agli utenti per le attività a cui sono stati assegnati mentre il progetto era in stato Pianificazione.

   >[!TIP]
   >
   >  Quando si apportano modifiche al progetto, ad esempio la modifica delle date di scadenza, è possibile ripristinare lo stato su Pianificazione oppure disattivare la funzione Salvataggio automatico per evitare che le notifiche vengano inviate prima del completamento delle modifiche.

   L’amministratore di sistema può impostare lo stato Pianificazione come impostazione predefinita globale di Workfront per i nuovi progetti.

1. **Modalità pianificazione**

   I progetti Workfront possono essere pianificati da una data di inizio o una data di completamento. Questa selezione importante determina il modo in cui vengono calcolate le date pianificate di ogni attività.

   L’opzione Data inizio considera la data di inizio del progetto, da te inserita, nonché la durata e i predecessori di ogni attività, per calcolare quando terminerà il progetto. Workfront consiglia di utilizzare questa opzione, in quanto è la più comune e semplifica la pianificazione delle date dei progetti.

   Tuttavia, puoi utilizzare una data di completamento. Workfront esamina la data di fine (da te inserita) e il lavoro da eseguire (in base alle durate e ai predecessori), quindi lavora a ritroso per calcolare la data di inizio del progetto. Workfront consiglia di aspettare a utilizzare la data di completamento fino a quando non si è raggiunto un determinato livello di esperienza in Workfront.

   Indipendentemente dall’opzione scelta, non dimenticare di selezionare una data dal calendario popup.

   L’opzione Modalità di pianificazione può essere impostata nel modello.

1. **Gruppo**

   Un gruppo è un’unità organizzativa di Workfront che spesso si allinea a un reparto. Questo campo può essere impostato sul modello del progetto. In caso contrario, il campo viene impostato automaticamente sul Gruppo Home della persona che crea il progetto. È possibile modificare il gruppo in base alle esigenze.

   Generalmente, la maggior parte delle persone che lavorano al progetto provengono da questo gruppo. Ma questo non impedisce che vengano assegnati lavori nel progetto a persone di altri gruppi.

   Il gruppo del progetto determina anche le preferenze di progetto, attività e problema che il progetto utilizzerà. Queste preferenze, ad esempio uno stato personalizzato per un gruppo specifico, vengono impostate dall’amministratore di sistema o da un amministratore di gruppo.

   L’impostazione del gruppo è un modo pratico, attraverso il reporting, per mostrare tutti i progetti su cui un reparto sta lavorando.

1. **Proprietario progetto**

   Proprietario del progetto è il termine utilizzato da Workfront per riferirsi al project manager. Si tratta della persona responsabile della pianificazione e/o della gestione del progetto.

   Affinché il proprietario del progetto possa disporre delle autorizzazioni di gestione complete per il progetto, deve disporre di una licenza Pianificazione.

   Normalmente questo campo viene lasciato vuoto nel modello e viene compilato automaticamente con il nome della persona che crea il progetto. Se nel modello viene immesso un nome, si tratta del proprietario predefinito del progetto.

1. **Sponsor Progetto**

   Lo sponsor del progetto non è obbligatorio, ma quando viene utilizzato è generalmente la persona che ha richiesto il progetto. Si tratta spesso di uno stakeholder interno, come un manager o un dirigente, con responsabilità generale del progetto.

   Lo sponsor riceve automaticamente le autorizzazioni di visualizzazione per il progetto e deve essere un utente con licenza Workfront.

   Lo sponsor del progetto può essere impostato nel modello.

1. **Responsabile risorse**

   Gli utenti di Workfront elencati in questo campo possono utilizzare gli strumenti di gestione e pianificazione delle risorse di Workfront per i progetti specifici in cui sono elencati. Nel campo Manager risorse è possibile elencare fino a 30 nomi, ognuno dei quali deve disporre di una licenza Pianificazione.

   Il campo Manager risorse può essere impostato nel modello.

1. **Moduli personalizzati**

   In Workfront sono disponibili campi nativi per elementi quali il nome del progetto e la data di inizio. Tuttavia, sono necessarie ulteriori informazioni in qualità di project manager o per il team del progetto. I dati univoci sono ugualmente importanti e possono essere facilmente archiviati in questi moduli. Dettagli come date di pubblicazione, dimensioni delle risorse di stampa, canali di consegna, ecc.

   I moduli personalizzati possono acquisire queste informazioni ed essere inclusi in elenchi e report in Workfront, semplificandone la visualizzazione e la modifica.

   I moduli personalizzati possono essere allegati ai modelli in anticipo.

1. **Pianificazione**

   Il lavoro si svolge 24 ore su 24, dato che molte aziende hanno dipendenti in tutto il mondo.

   Workfront consente di applicare ai progetti una pianificazione comune. Le pianificazioni comuni vengono create dall’amministratore di sistema. Le pianificazioni riflettono i giorni e le ore lavorative dei team, più i giorni in cui i dipendenti non saranno al lavoro (come le festività).

   Durante la pianificazione, assicurati di applicare quella corretta al progetto corretto. Le impostazioni della pianificazione influiscono sui calcoli della timeline, tenendo conto delle ferie e dei fusi orari.

   La pianificazione assegnata al progetto deve essere quella che si applica alla maggior parte degli assegnatari dell’attività. Se non è stata specificata alcuna pianificazione per il progetto, verrà utilizzata la pianificazione contrassegnata come Predefinita.

   La pianificazione può essere impostata nel modello.

1. **Gruppi di risorse**

   I pool di risorse sono insiemi di utenti Workfront necessari contemporaneamente per il completamento dei progetti all’interno dell’organizzazione. Un pool di risorse può essere assegnato a più progetti, il che significa che si dispone di progetti in competizione per le risorse.

   L’assegnazione di pool di risorse a un progetto è un prerequisito per l’utilizzo della Pianificazione risorse e di altri strumenti di gestione delle risorse in Workfront.

   È possibile impostare un pool di risorse predefinito nel modello.

1. **Accesso al progetto per utenti e collaboratori**

   Quando a un utente viene concesso l’accesso a un progetto tramite Condividi, è possibile assegnare tre livelli di autorizzazione: Visualizza, Contribuisci e Gestisci. Ogni livello di autorizzazione consente all’utente di visualizzare ed eseguire determinate operazioni con il progetto.

   Ad esempio, ci sono persone che potrebbero avere accesso al progetto ma non dovrebbero vedere le informazioni finanziarie. Per questo motivo è possibile disattivare l’opzione Visualizza dati finanziari.

   Le impostazioni di accesso possono essere impostate nel modello.

## Tutorial consigliati su questo argomento

* [Creazione di un progetto di base](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/manage-work/projects/understand-basic-project-creation)
* [Passare alla pagina del progetto](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/manage-work/projects/navigate-the-project-page)
* [Scopri quattro modi per creare un progetto](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/manage-work/projects/understand-other-ways-to-create-projects)
* [Inizia a pianificare un progetto](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/manage-work/projects/getting-started-plan-a-project)
