---
title: Copiare un obiettivo esistente
description: Scopri come copiare un obiettivo esistente in [!DNL Workfront Goals].
feature: Workfront Goals
type: Tutorial
role: User
level: Beginner
kt: 10121
exl-id: bf9ac10a-8419-458b-b4e8-bedb0ad3b98f
source-git-commit: 27e8f0aada77488bd6cfc2e786b997f759fd0a17
workflow-type: tm+mt
source-wordcount: '525'
ht-degree: 0%

---

# Copiare un obiettivo esistente

Supponiamo che sia la fine di un trimestre e desideri ricreare un obiettivo esistente per il prossimo periodo. O forse non hai completato l&#39;obiettivo e devi estenderlo al periodo di tempo successivo. Qual è l&#39;opzione migliore per creare quell&#39;obiettivo? Sarà necessario copiare e modificare un obiettivo esistente.

Copiare un obiettivo esistente è utile anche se più membri del team hanno obiettivi simili e devi creare un obiettivo per ciascuno di essi.

<!--
Pro-tips graphic
-->

Di seguito sono riportati alcuni aspetti da considerare prima di copiare gli obiettivi:

* Tutte le informazioni dell&#39;obiettivo originale verranno copiate, ad eccezione del periodo di obiettivo (perché è nel passato).
* Puoi copiare i risultati di un obiettivo esistente e questi verranno trasferiti al nuovo obiettivo.
* Per impostazione predefinita, i risultati copiati vengono assegnati allo stesso proprietario.
* Non è possibile copiare l&#39;avanzamento dell&#39;obiettivo esistente in un nuovo obiettivo.
* Non puoi copiare le attività di un obiettivo quando copi un obiettivo.

## Come copiare un obiettivo

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
