---
title: Configurare le preferenze globali predefinite per i problemi
description: Scopri come impostare le preferenze del problema per i problemi convertiti, le date effettive e l’accesso al problema.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
jira: KT-10018
exl-id: 9924e479-c300-47b4-8e40-241ebb2435cf
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '885'
ht-degree: 0%

---

# Configurare le preferenze globali dei problemi predefiniti

Diverse impostazioni a livello di sistema stabiliscono valori predefiniti per il comportamento dei problemi in determinate circostanze in [!DNL Workfront].

Si consiglia di lasciare invariati i valori predefiniti globali e consentire ai project manager di apportare le modifiche necessarie a livello di progetto o nei modelli di progetto.

È possibile regolare le preferenze relative al problema globale, ma si consiglia di e [!DNL Workfront] i consulenti illustrano le impostazioni necessarie per i flussi di lavoro, i processi e le esigenze di reporting della tua organizzazione. Il tuo consulente può anche aiutarti a capire cosa succederà se alcune impostazioni vengono modificate.

Le preferenze problema consentono agli amministratori di sistema di controllare le opzioni quando i problemi vengono convertiti in attività o progetti, il modo in cui vengono calcolate le date effettive e chi ottiene l’accesso al progetto quando vengono assegnati i problemi. Vediamo dove si trovano queste impostazioni [!DNL Workfront].

## Preferenze problema convertito

Queste impostazioni controllano cosa accade a un problema quando viene convertito in un’attività o in un progetto in [!DNL Workfront].

![[!UICONTROL Attività e problemi] finestra preferenze con [!UICONTROL Problemi] sezione evidenziata](assets/admin-fund-issue-prefs-converting.png)

1. Clic **[!UICONTROL Configurazione]** nel **[!UICONTROL Menu principale]**.
1. Espandi **[!UICONTROL Preferenze progetto]** nel pannello del menu a sinistra.
1. Seleziona **[!UICONTROL Attività e problemi]**.
1. Scorri fino a **[!UICONTROL Problemi]** sezione.
1. Fai clic sulle opzioni desiderate.
1. Al termine, salva.

Esaminiamo le opzioni disponibili in questa sezione per consentirti di scegliere quelle appropriate per la tua organizzazione.

* **[!UICONTROL Aggiorna automaticamente lo stato del problema risolvibile quando lo stato dell&#39;oggetto risolutivo cambia]**

  Consente di correlare la risoluzione del problema originale alla risoluzione del nuovo oggetto (attività o progetto).

  Se questa impostazione è abilitata (selezionata), puoi creare stati di problemi personalizzati con la stessa chiave di stato di un’attività o di un progetto. Quando l’attività o il progetto (l’oggetto risolvibile) è impostato sullo stato personalizzato, la modifica viene visualizzata anche sullo stato del problema.

  Se l&#39;opzione è disattivata, lo stato dell&#39;oggetto di risoluzione viene impostato automaticamente sullo stato predefinito, anziché su quello personalizzato.

  Affinché questa impostazione abbia effetto, il comando &quot;[!UICONTROL Mantieni il problema originale e collegane la risoluzione all&#39;attività]&quot; deve essere selezionata.

* **[!UICONTROL Mantieni il problema originale e collegalo alla risoluzione dell’attività/progetto]**

  Quando il problema viene convertito, indica [!DNL Workfront] per mantenere i problemi originali. Lo stato del problema cambia quando cambia lo stato dell’attività o del progetto. Dopo aver contrassegnato l&#39;attività o il progetto come completato, il problema viene contrassegnato come risolto.

  Se questa opzione non è selezionata, il problema originale viene eliminato e rimane solo l&#39;attività o il progetto convertito.

  Questa impostazione influisce sulla generazione di rapporti sui problemi originariamente registrati in un progetto o che derivano da un [!DNL Workfront] coda richieste.

* **[!UICONTROL Consenti al contatto principale di accedere all&#39;attività o al progetto]**

  In questo modo l’utente che ha creato il problema originale ha accesso all’attività o al progetto creato durante la conversione. Possono rivedere il lavoro, apportare aggiornamenti e rimanere informati sui suoi progressi.

* **[!UICONTROL Consenti la modifica delle impostazioni durante la conversione]**

  Se selezionata, questa opzione indica le impostazioni predefinite per &quot;[!UICONTROL Mantieni problema originale]&quot; e &quot;[!UICONTROL Consenti contatto principale]&quot; possono essere modificate dall’utente che converte il problema. Se desiderate che le impostazioni predefinite rimangano invariate, deselezionate questa opzione.

<!---
learn more URLs
Configure system-wide task and issue preferences
Issue statuses
Create and customize system-wide statuses
--->

## Preferenze date effettive

In sono utilizzati più tipi di date [!DNL Workfront]. Le date effettive sono una &quot;marca temporale&quot; che [!DNL Workfront] genera quando si verificano determinate modifiche di stato.

Il [!UICONTROL Data d&#39;Inizio Reale] La marca temporale viene creata quando lo stato del problema cambia da Nuovo a un altro stato. Il [!UICONTROL Data di completamento effettiva] il timestamp si verifica quando lo stato del problema cambia in uno stato che indica che è chiuso.

È importante notare che questa preferenza controlla le impostazioni effettive della data sia per le attività che per i problemi.

![[!UICONTROL Attività e problemi] finestra preferenze con [!UICONTROL Date effettive] sezione evidenziata](assets/admin-fund-issue-prefs-actual-dates.png)

1. Clic **[!UICONTROL Configurazione]** nel **[!UICONTROL Menu principale]**.
1. Espandi **[!UICONTROL Preferenze progetto]** nel pannello del menu a sinistra.
1. Seleziona **[!UICONTROL Attività e problemi]**.
1. Scorri fino a **[!UICONTROL Date effettive]** sezione.
1. Seleziona l’opzione desiderata per il **[!UICONTROL Data d&#39;Inizio Reale]** — [!UICONTROL Ora] (la data e l’ora correnti) oppure [!UICONTROL La data di inizio pianificata] (il [!UICONTROL Data d&#39;Inizio Reale] corrisponde alla data di inizio impostata nei dettagli del problema).
1. Ora seleziona l’opzione per **[!UICONTROL Data di completamento effettiva]** — [!UICONTROL Ora] (la data e l’ora correnti) oppure [!UICONTROL La data di completamento pianificata] (il [!UICONTROL Data d&#39;Inizio Reale] corrisponde alla data impostata nei dettagli del problema).
1. Al termine, salva.


<!---
learn more URLs
Definitions for the project, task, and issue dates within Workfront
Configure system-wide task and issue preferences
--->

## Accesso problema

Il [!UICONTROL Accesso] le impostazioni per i problemi controllano l’accesso concesso a un utente quando viene assegnato un problema in Workfront. Queste impostazioni controllano l’accesso al problema stesso, oltre all’accesso al progetto a cui è associato il problema.

Prima di modificare queste impostazioni, discuti con il tuo account di qualsiasi flusso di lavoro o processo necessario [!DNL Workfront] consulenti e il team di governance interno.

![[!UICONTROL Attività e problemi] finestra preferenze con [!UICONTROL Quando a un utente viene assegnato un PROBLEMA] sezione evidenziata](assets/admin-fund-issue-prefs-access-1.png)

1. Clic **[!UICONTROL Configurazione]** nel **[!UICONTROL Menu principale]**.
1. Espandi **[!UICONTROL Preferenze progetto]** nel pannello del menu a sinistra.
1. Seleziona **[!UICONTROL Attività e problemi]**.
1. Scorri fino a **[!UICONTROL Accesso]** e trovare la sezione &quot;[!UICONTROL Quando a un utente viene assegnato un PROBLEMA]&quot;.
1. Impostare l&#39;accesso alla condivisione per il problema stesso — [!UICONTROL Visualizza], [!UICONTROL Contribuisci], o [!UICONTROL Gestisci]. [!DNL Workfront] consiglia di lasciare invariate le opzioni avanzate.
1. Seleziona la casella se anche l’assegnatario del problema deve avere accesso al progetto
1. Selezionare quindi l&#39;accesso condiviso per il progetto. [!UICONTROL Visualizza], [!UICONTROL Contribuisci], o [!UICONTROL Gestisci]. Quando si imposta [!UICONTROL Opzioni avanzate], tieni presenti i flussi di lavoro dell’organizzazione e le esigenze di accesso.
1. Al termine, salva.

![[!UICONTROL Accesso] visualizzazione della finestra [!UICONTROL Contribuisci] opzioni](assets/admin-fund-issue-prefs-access-2.png)

<!---
learn more URLs
Configure system-wide task and issue preferences
Grant access to issues
--->
