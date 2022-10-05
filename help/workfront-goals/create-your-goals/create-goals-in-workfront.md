---
title: Creare obiettivi in Workfront
description: Scopri come creare obiettivi in [!DNL Workfront Goals] utilizzando tre opzioni diverse.
activity: use
feature: Workfront Goals
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
kt: 10122
exl-id: 784b353f-cc6b-4a4b-9935-9e5d25c532b4
source-git-commit: d1f5c4a558f737cb8188e209a16b91b67d32285c
workflow-type: tm+mt
source-wordcount: '923'
ht-degree: 0%

---

# Creare obiettivi in Workfront

In [!DNL Workfront Goals], dirigenti e team di direzione aziendale possono vedere i progressi dell&#39;intera organizzazione ad ogni livello, fino all&#39;individuo. [!DNL Workfront Goals] offre la visibilità necessaria per ottenere informazioni utili per portare avanti le priorità più importanti, identificare gli obiettivi a rischio, diagnosticare i problemi in tempo reale e correggere in modo proattivo il corso.

[!DNL Workfront Goals] consente anche ai singoli collaboratori di vedere in che modo il loro lavoro contribuisce al quadro generale. Il lavoro è più significativo quando gli individui possono vedere dove il loro lavoro conta.

Ci sono 3 modi per creare obiettivi con [!DNL Workfront]:

## Creare un obiettivo da zero

Di seguito sono riportati alcuni aspetti da considerare durante la creazione di obiettivi da zero:

* Non puoi creare obiettivi con date di fine passate.
* Quando si creano obiettivi o obiettivi simili allineati, tutti nell’organizzazione devono selezionare gli stessi intervalli di tempo.
* Le date personalizzate sono vincolate dalla data iniziale selezionata. Ciò significa che se selezioni &quot;trimestre&quot; e quindi una data personalizzata, la data personalizzata non può andare oltre il trimestre.
* Lo stato del nuovo obiettivo è sempre Bozza finché non lo attivi aggiungendo un’attività o un risultato.

Questo video illustra come:

* Passa alla [!UICONTROL Elenco obiettivi] per aggiungere un nuovo obiettivo

>[!VIDEO](https://video.tv.adobe.com/v/335191/?quality=12)

## Copiare un obiettivo esistente

Supponiamo che sia la fine di un trimestre e desideri ricreare un obiettivo esistente per il prossimo periodo. O forse non hai completato l&#39;obiettivo e devi estenderlo al periodo di tempo successivo. Qual è l&#39;opzione migliore per creare quell&#39;obiettivo? Sarà necessario copiare e modificare un obiettivo esistente.

Copiare un obiettivo esistente è utile anche se più membri del team hanno obiettivi simili e devi creare un obiettivo per ciascuno di essi.

Di seguito sono riportati alcuni aspetti da considerare prima di copiare gli obiettivi:

* Tutte le informazioni dell&#39;obiettivo originale verranno copiate, ad eccezione del periodo di obiettivo (perché è nel passato).
* Puoi copiare i risultati di un obiettivo esistente e questi verranno trasferiti al nuovo obiettivo.
* Per impostazione predefinita, i risultati copiati vengono assegnati allo stesso proprietario.
* Non è possibile copiare l&#39;avanzamento dell&#39;obiettivo esistente in un nuovo obiettivo.
* Non puoi copiare le attività di un obiettivo quando copi un obiettivo.

### Come copiare un obiettivo

1. Fai clic sul nome di un obiettivo per aprire **[!UICONTROL Dettagli obiettivo]** pannello.
1. Fai clic sull’icona a 3 punti, quindi seleziona **[!UICONTROL Copia]**.
1. Aggiorna una delle seguenti informazioni per l&#39;obiettivo copiato:
   * **Nuovo obiettivo**- Questo è il nome del nuovo obiettivo. Il valore predefinito è il nome dell&#39;obiettivo originale.
   * **Punto**- Il periodo di tempo durante il quale si desidera raggiungere l&#39;obiettivo. Seleziona un periodo di tempo dal menu a discesa o fai clic su Definisci date personalizzate per indicare un periodo di tempo personalizzato. Il periodo predefinito è sempre il trimestre corrente.
   * **Proprietario**- Il proprietario dell&#39;obiettivo. Può essere un utente, un team, un gruppo o un&#39;azienda. Il valore predefinito è il proprietario dell&#39;obiettivo originale.
   * **Descrizione**- Informazioni aggiuntive sull&#39;obiettivo.

1. Controlla la **[!UICONTROL Copia risultati]** Se all&#39;obiettivo originale sono stati aggiunti dei risultati e si desidera copiarli nel nuovo obiettivo. I risultati dell&#39;obiettivo copiato hanno gli stessi proprietari, nomi e valori misurati dei risultati dell&#39;obiettivo originale.

1. Fai clic su **[!UICONTROL Salva]**. L&#39;obiettivo copiato viene salvato con lo stato Bozza.

   ![Un&#39;immagine del [!UICONTROL Dettagli obiettivo] pannello in [!DNL Workfront Goals] con [!UICONTROL Copia] opzione](assets/03-workfront-goals-copy-a-goal.png)

1. Fai clic su **[!UICONTROL Attiva]**, che aggiorna lo stato dell’obiettivo su Attivo. L’obiettivo deve avere un’attività associata o un risultato per poter &quot;attivare&quot;.

1. Fai clic sul pulsante **X** in alto a destra del [!UICONTROL Dettagli obiettivo] per chiuderlo.

Se hai copiato un obiettivo che non è stato completato in un periodo di tempo precedente e desideri continuare a utilizzarlo nel periodo di tempo seguente, procedi come segue:

1. Vai all&#39;obiettivo originale nel **[!UICONTROL Elenco obiettivi]**, **[!UICONTROL Check-in]** sezione, oppure **[!UICONTROL Impulso]** sezione .
1. Commenta l’obiettivo per indicare che è stato copiato e che è stato creato un obiettivo più corrente.
1. Chiudere l&#39;obiettivo originale per mantenere i progressi compiuti durante il periodo di tempo originale. Fai clic sull’icona a 3 punti nel **[!UICONTROL Dettagli obiettivo]** e seleziona **[!UICONTROL Chiudi]** dal menu.
1. Aggiorna [!UICONTROL Iniziale] valore del nuovo risultato che corrisponde al **[!UICONTROL Target]** valore del risultato precedente, in modo che l&#39;avanzamento del nuovo obiettivo inizi a essere calcolato dal punto raggiunto nel periodo precedente.

## Convertire un risultato o un’attività in un obiettivo

L’opzione finale per la creazione degli obiettivi in [!DNL Workfront Goals] è mediante la conversione dei risultati e/o delle attività di un obiettivo esistente in un altro obiettivo. Il risultato/attività convertito diventa un obiettivo secondario rispetto all’obiettivo originale.

Puoi eseguire questa operazione quando un risultato/attività ha un ambito più ampio del previsto e sarebbe utile convertire il risultato/attività in un obiettivo effettivo stesso. Pensate a questo come ad un approccio dal basso verso l&#39;alto per allineare gli obiettivi.

Di seguito sono riportati alcuni aspetti da tenere a mente prima di convertire un risultato o un’attività in un obiettivo:

* Il risultato o l’attività convertiti può diventare l’obiettivo secondario dell’obiettivo originale. I due obiettivi si allineano.
* Il risultato o l’attività convertito può essere rimosso dall’obiettivo originale e aggiunto come risultato o attività all’obiettivo appena creato.
* L&#39;obiettivo appena creato diventa l&#39;unico indicatore di avanzamento per l&#39;obiettivo originale, se non ci sono ulteriori risultati o attività sull&#39;obiettivo originale.

Questo video illustra come:

* Convertire un’attività in un obiettivo allineato

>[!VIDEO](https://video.tv.adobe.com/v/335192/?quality=12)

Ora che hai esplorato i tre modi per creare obiettivi in [!DNL Workfront Goals]Lavoriamo all&#39;attivazione di questi obiettivi.
