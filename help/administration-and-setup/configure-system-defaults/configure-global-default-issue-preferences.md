---
title: Configurare le preferenze globali dei problemi predefiniti
description: Scopri come impostare le preferenze del problema per i problemi convertiti, le date effettive e l’accesso al problema.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
jira: KT-10018
exl-id: 9924e479-c300-47b4-8e40-241ebb2435cf
source-git-commit: 4568e4e47b719e2dee35357d42674613112a9c43
workflow-type: tm+mt
source-wordcount: '885'
ht-degree: 75%

---

# Configurare le preferenze globali dei problemi predefiniti

Diverse impostazioni a livello di sistema stabiliscono valori predefiniti per il comportamento dei problemi in determinate circostanze in [!DNL Workfront].

Le best practice suggeriscono di lasciare invariati i valori predefiniti globali e consentire ai project manager di apportare le modifiche necessarie a livello di progetto o nei modelli di progetto.

È possibile regolare le preferenze relative ai problemi globali, ma si consiglia di discutere con il consulente [!DNL Workfront] le impostazioni necessarie per i flussi di lavoro, i processi e le esigenze di reporting della propria organizzazione. Il consulente può anche aiutarti a capire cosa succederà se alcune impostazioni vengono modificate.

Le preferenze dei problemi consentono agli amministratori di sistema di controllare le opzioni dei problemi convertiti in attività o progetti, come vengono calcolate le date effettive e chi ottiene l’accesso al progetto quando i problemi vengono assegnati. Vediamo dove si trovano queste impostazioni in [!DNL Workfront].

## Preferenze problema convertito

Queste impostazioni controllano cosa accade a un problema quando viene convertito in un&#39;attività o in un progetto in [!DNL Workfront].

Finestra delle preferenze ![[!UICONTROL Attività e problemi] con evidenziata la sezione [!UICONTROL Problemi]](assets/admin-fund-issue-prefs-converting.png)

1. Fai clic su **[!UICONTROL Configurazione]** nel **[!UICONTROL Menu principale]**.
1. Espandi la sezione **[!UICONTROL Preferenze progetto]** nel pannello del menu a sinistra.
1. Seleziona **[!UICONTROL Attività e problemi]**.
1. Scorri fino alla sezione **[!UICONTROL Problemi]**.
1. Fai clic sulle opzioni desiderate.
1. Al termine, salva.

Esaminiamo ora le opzioni disponibili in questa sezione per consentirti di scegliere quelle appropriate per la tua organizzazione.

* **[!UICONTROL Aggiorna automaticamente lo stato del problema risolvibile quando lo stato dell’oggetto di risoluzione cambia]**

  Questa impostazione consente di correlare la risoluzione del problema originale alla risoluzione del nuovo oggetto (attività o progetto).

  Con questa impostazione abilitata (selezionata), puoi creare stati di problema personalizzati che hanno la stessa chiave di stato di un’attività o di un progetto. Quando l’attività o il progetto (l’oggetto risolvibile) è impostato sullo stato personalizzato, la modifica viene visualizzata anche sullo stato del problema.

  Se l’opzione è disattivata, lo stato dell’oggetto di risoluzione viene impostato automaticamente sullo stato predefinito, anziché su quello personalizzato.

  Affinché questa impostazione abbia effetto, è necessario selezionare l&#39;opzione &quot;[!UICONTROL Mantieni il problema originale e collegane la risoluzione all&#39;attività]&quot;.

* **[!UICONTROL Mantieni il problema originale e collegane la risoluzione all’attività/progetto]**

  Quando il problema viene convertito, questo fa sì che [!DNL Workfront] mantenga i problemi originali. Lo stato del problema cambia man mano che cambia lo stato dell’attività o del progetto. Dopo aver contrassegnato l’attività o il progetto come completato, il problema viene contrassegnato come risolto.

  Se questa opzione non è selezionata, il problema originale viene eliminato e rimane solo l’attività o il progetto convertito.

  Questa impostazione influisce sulla generazione di rapporti sui problemi originariamente registrati in un progetto o che derivano da una coda richieste di [!DNL Workfront].

* **[!UICONTROL Consenti al contatto principale di accedere all’attività/progetto]**

  Ciò fornisce alla persona che ha creato il problema originale l’accesso all’attività o al progetto creato durante la conversione. In questo modo, chi ha creato il progetto può rivedere il lavoro, apportare aggiornamenti e avere informazioni sui suoi progressi.

* **[!UICONTROL Consenti la modifica delle impostazioni durante la conversione]**

  Se selezionata, l&#39;utente che converte il problema potrà modificare le impostazioni predefinite per &quot;[!UICONTROL Mantieni problema originale]&quot; e &quot;[!UICONTROL Consenti contatto principale]&quot;. Se desideri che le impostazioni predefinite rimangano invariate, deseleziona questa opzione.

<!--
learn more URLs
Configure system-wide task and issue preferences
Issue statuses
Create and customize system-wide statuses
-->

## Preferenze date effettive

Ci sono diverse tipologie di date utilizzate in tutto il processo [!DNL Workfront]. Le date effettive sono una &quot;marca temporale&quot; generata da [!DNL Workfront] quando si verificano determinate modifiche di stato.

La marca temporale [!UICONTROL Data di inizio effettiva] viene creata quando lo stato del problema cambia da Nuovo a un altro stato. La marca temporale [!UICONTROL Data di completamento effettiva] si verifica quando lo stato del problema cambia in uno stato che indica che è chiuso.

È importante notare che questa preferenza controlla le impostazioni effettive della data sia per le attività che per i problemi.

Finestra delle preferenze di ![[!UICONTROL Attività e problemi] con la sezione [!UICONTROL Date effettive] evidenziata](assets/admin-fund-issue-prefs-actual-dates.png)

1. Fai clic su **[!UICONTROL Configurazione]** nel **[!UICONTROL Menu principale]**.
1. Espandi la sezione **[!UICONTROL Preferenze progetto]** nel pannello del menu a sinistra.
1. Seleziona **[!UICONTROL Attività e problemi]**.
1. Scorri fino alla sezione **[!UICONTROL Date effettive]**.
1. Seleziona l’opzione desiderata per la **[!UICONTROL Data d’inizio effettiva]**: [!UICONTROL Ora] (data e ora correnti) oppure [!UICONTROL Data d’inizio pianificata] (la [!UICONTROL Data d’inizio effettiva] corrisponde alla data di inizio impostata nei dettagli del problema).
1. Ora seleziona l’opzione per la **[!UICONTROL Data di completamento effettiva]**: [!UICONTROL Ora] (data e ora correnti) oppure [!UICONTROL Data di completamento pianificata] (la [!UICONTROL Data d’inizio effettiva] corrisponde alla data impostata nei dettagli del problema).
1. Al termine, salva.


<!--
learn more URLs
Definitions for the project, task, and issue dates within Workfront
Configure system-wide task and issue preferences
-->

## Accesso al problema

Le impostazioni di [!UICONTROL Accesso] per i problemi controllano l&#39;accesso concesso a un utente quando gli viene assegnato un problema in Workfront. Queste impostazioni controllano l’accesso al problema stesso, oltre all’accesso al progetto a cui è associato il problema.

Prima di modificare queste impostazioni, discuti di qualsiasi flusso di lavoro o processo necessario con i tuoi consulenti di [!DNL Workfront] e il tuo team di governance interno.

Finestra delle preferenze ![[!UICONTROL Attività e problemi] con la sezione [!UICONTROL Quando a un utente viene assegnato un PROBLEMA] evidenziata](assets/admin-fund-issue-prefs-access-1.png)

1. Fai clic su **[!UICONTROL Configurazione]** nel **[!UICONTROL Menu principale]**.
1. Espandi la sezione **[!UICONTROL Preferenze progetto]** nel pannello del menu a sinistra.
1. Seleziona **[!UICONTROL Attività e problemi]**.
1. Scorri fino alla sezione **[!UICONTROL Access]** e individua l&#39;opzione &quot;[!UICONTROL Quando qualcuno è assegnato a un PROBLEMA]&quot;.
1. Imposta l’accesso di condivisione per il problema stesso: [!UICONTROL Visualizza],[!UICONTROL  Contribuisci], o [!UICONTROL Gestisci]. [!DNL Workfront] consiglia di lasciare invariate le opzioni avanzate.
1. Seleziona la casella se anche l’assegnatario del problema deve avere accesso al progetto
1. Quindi seleziona l’accesso di condivisione per il progetto: [!UICONTROL Visualizza],[!UICONTROL  Contribuisci], o [!UICONTROL Gestisci]. Quando imposti le [!UICONTROL Opzioni avanzate], tieni presenti i flussi di lavoro della tua organizzazione e le esigenze di accesso.
1. Al termine, salva.

Finestra ![[!UICONTROL Accesso] che mostra le opzioni [!UICONTROL Contribuisci]](assets/admin-fund-issue-prefs-access-2.png)

<!--
learn more URLs
Configure system-wide task and issue preferences
Grant access to issues
-->
