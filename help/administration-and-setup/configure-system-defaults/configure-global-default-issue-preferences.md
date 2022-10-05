---
title: Configurare le preferenze per i problemi predefiniti globali
description: Scopri come impostare le preferenze dei problemi per i problemi convertiti, le date effettive e l’accesso ai problemi.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
kt: 10018
exl-id: 9924e479-c300-47b4-8e40-241ebb2435cf
source-git-commit: 3ded3fe9d8b97b1c11cb382f8088930842399c98
workflow-type: tm+mt
source-wordcount: '885'
ht-degree: 0%

---

# Configurare le preferenze predefinite globali dei problemi

Diverse impostazioni a livello di sistema determinano le impostazioni predefinite per il comportamento dei problemi in determinate circostanze [!DNL Workfront].

La procedura consigliata consiste nel lasciare invariati i valori predefiniti globali e nel consentire ai project manager di apportare le modifiche necessarie a livello di progetto o nei modelli di progetto.

È possibile regolare le preferenze relative al problema globale, ma si consiglia di [!DNL Workfront] consulta le impostazioni necessarie per i flussi di lavoro, i processi e le esigenze di reporting della tua organizzazione. Il tuo consulente può anche aiutarti a capire cosa succederà se vengono modificate alcune impostazioni.

Le preferenze relative ai problemi consentono agli amministratori di sistema di controllare le opzioni quando i problemi vengono convertiti in attività o progetti, come vengono calcolate le date effettive e chi ottiene l’accesso al progetto quando i problemi vengono assegnati. Diamo un&#39;occhiata a dove si trovano queste impostazioni [!DNL Workfront].

## Preferenze dei problemi convertiti

Queste impostazioni controllano cosa accade a un problema quando viene convertito in un&#39;attività o in un progetto in [!DNL Workfront].

![[!UICONTROL Attività e problemi] finestra delle preferenze con [!UICONTROL Problemi] sezione evidenziata](assets/admin-fund-issue-prefs-converting.png)

1. Fai clic su **[!UICONTROL Configurazione]** in **[!UICONTROL Menu principale]**.
1. Espandi la **[!UICONTROL Preferenze del progetto]** nel pannello del menu a sinistra.
1. Seleziona **[!UICONTROL Attività e problemi]**.
1. Scorri fino a **[!UICONTROL Problemi]** sezione .
1. Fai clic sulle opzioni desiderate.
1. Al termine, salva.

Diamo un’occhiata alle opzioni presenti in questa sezione, in modo da poter scegliere le opzioni appropriate per la tua organizzazione.

* **[!UICONTROL Aggiorna automaticamente lo stato del problema risolvibile quando lo stato dell&#39;oggetto di risoluzione cambia]**

   Questa impostazione consente di correlare la risoluzione del problema originale alla risoluzione del nuovo oggetto (attività o progetto).

   Con questa impostazione abilitata (selezionata), puoi creare stati di problemi personalizzati con la stessa chiave di stato di un&#39;attività o di uno stato di progetto. Quando l&#39;attività o il progetto (l&#39;oggetto risolvibile) è impostato sullo stato personalizzato, la modifica viene visualizzata anche sullo stato del problema.

   Se disabilitata, lo stato dell’oggetto di risoluzione viene impostato automaticamente sullo stato predefinito, anziché su quello personalizzato.

   Affinché questa impostazione abbia effetto, il &quot;[!UICONTROL Mantenere il problema originale e legarne la risoluzione all&#39;attività]&quot; deve essere selezionata.

* **[!UICONTROL Mantieni il problema originale e il tempo è la risoluzione all&#39;attività/progetto]**

   Quando il problema viene convertito, questo indica [!DNL Workfront] per mantenere i problemi originali. Lo stato del problema cambia quando cambia lo stato dell&#39;attività o del progetto. Una volta che l&#39;attività o il progetto è contrassegnato come completato, il problema viene contrassegnato come risolto.

   Se questa opzione non è selezionata, il problema originale viene eliminato e rimane solo l&#39;attività o il progetto convertiti.

   Questa impostazione influisce sul reporting dei problemi originariamente connessi a un progetto o che provengono da un [!DNL Workfront] coda richieste.

* **[!UICONTROL Consenti accesso al contatto primario per l&#39;attività o il progetto]**

   Questo consente alla persona che ha creato il problema originale di accedere all’attività o al progetto creato durante la conversione. Possono rivedere il lavoro, apportare aggiornamenti e rimanere informati dei suoi progressi.

* **[!UICONTROL Consenti la modifica delle impostazioni durante la conversione]**

   Se selezionata, questa opzione indica le impostazioni predefinite per &quot;[!UICONTROL Mantieni problema originale]&quot; e &quot;[!UICONTROL Consenti contatto primario]&quot; può essere modificato dall&#39;utente che converte il problema. Se desideri che le impostazioni predefinite rimangano invariate, deseleziona questa opzione.

<!---
learn more URLs
Configure system-wide task and issue preferences
Issue statuses
Create and customize system-wide statuses
--->

## Preferenze date effettive

Esistono diversi tipi di date utilizzati in [!DNL Workfront]. Le date effettive sono una &quot;marca temporale&quot; che [!DNL Workfront] genera quando si verificano determinate modifiche dello stato.

La [!UICONTROL Data di inizio effettiva] la marca temporale viene creata quando lo stato del problema cambia da Nuovo a un altro stato. La [!UICONTROL Data completamento effettivo] la marca temporale si verifica quando lo stato del problema cambia in uno stato che indica che è chiuso.

È importante notare che questa preferenza controlla le impostazioni di data effettive sia per le attività che per i problemi.

![[!UICONTROL Attività e problemi] finestra delle preferenze con [!UICONTROL Date effettive] sezione evidenziata](assets/admin-fund-issue-prefs-actual-dates.png)

1. Fai clic su **[!UICONTROL Configurazione]** in **[!UICONTROL Menu principale]**.
1. Espandi la **[!UICONTROL Preferenze del progetto]** nel pannello del menu a sinistra.
1. Seleziona **[!UICONTROL Attività e problemi]**.
1. Scorri fino a **[!UICONTROL Date effettive]** sezione .
1. Seleziona l’opzione desiderata per la **[!UICONTROL Data di inizio effettiva]** — [!UICONTROL Ora] (data e ora correnti) oppure [!UICONTROL Data di inizio prevista] (2) [!UICONTROL Data di inizio effettiva] corrisponde alla data di inizio impostata nei dettagli del problema).
1. Ora seleziona l’opzione per la **[!UICONTROL Data completamento effettivo]** — [!UICONTROL Ora] (data e ora correnti) oppure [!UICONTROL Data di completamento pianificata] (2) [!UICONTROL Data di inizio effettiva] corrisponde alla data impostata nei dettagli del problema).
1. Al termine, salva.


<!---
learn more URLs
Definitions for the project, task, and issue dates within Workfront
Configure system-wide task and issue preferences
--->

## Accesso al problema

La [!UICONTROL Accesso] le impostazioni per i problemi controllano l’accesso concesso a un utente quando gli viene assegnato un problema in Workfront. Queste impostazioni controllano l&#39;accesso al problema stesso, oltre all&#39;accesso al progetto a cui è associato il problema.

Prima di modificare queste impostazioni, discuti qualsiasi esigenza di flusso di lavoro o di processo con il tuo [!DNL Workfront] consulenti e il team di governance interno.

![[!UICONTROL Attività e problemi] finestra delle preferenze con [!UICONTROL Quando qualcuno viene assegnato a un problema] sezione evidenziata](assets/admin-fund-issue-prefs-access-1.png)

1. Fai clic su **[!UICONTROL Configurazione]** in **[!UICONTROL Menu principale]**.
1. Espandi la **[!UICONTROL Preferenze del progetto]** nel pannello del menu a sinistra.
1. Seleziona **[!UICONTROL Attività e problemi]**.
1. Scorri fino a **[!UICONTROL Accesso]** e trova la sezione &quot;[!UICONTROL Quando qualcuno viene assegnato a un problema]&quot; opzione.
1. Impostare l&#39;accesso condiviso per il problema stesso — [!UICONTROL Visualizza], [!UICONTROL Collaborare]oppure [!UICONTROL Gestisci]. [!DNL Workfront] consiglia di lasciare invariate le opzioni avanzate.
1. Seleziona la casella se anche l’assegnatario del problema deve avere accesso al progetto
1. Quindi seleziona l&#39;accesso condiviso per il progetto — [!UICONTROL Visualizza], [!UICONTROL Collaborare]oppure [!UICONTROL Gestisci]. Quando imposti [!UICONTROL Opzioni avanzate], ricorda i flussi di lavoro e le esigenze di accesso della tua organizzazione.
1. Al termine, salva.

![[!UICONTROL Accesso] finestra [!UICONTROL Collaborare] options](assets/admin-fund-issue-prefs-access-2.png)

<!---
learn more URLs
Configure system-wide task and issue preferences
Grant access to issues
--->
