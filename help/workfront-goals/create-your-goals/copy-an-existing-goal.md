---
title: Copiare un obiettivo esistente
description: Scopri come copiare un obiettivo esistente in  [!DNL Workfront Goals].
activity: use
team: Technical Marketing
feature: Workfront Goals
type: Tutorial
role: User
level: Beginner
jira: KT-10121
exl-id: bf9ac10a-8419-458b-b4e8-bedb0ad3b98f
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: ht
source-wordcount: '525'
ht-degree: 100%

---

# Copiare un obiettivo esistente

Supponiamo che sia la fine di un trimestre e che desideri ricreare un obiettivo esistente per il periodo successivo. O magari non hai completato l’obiettivo e devi estenderlo al periodo di tempo successivo. Qual è l’opzione migliore per creare tale obiettivo? Desideri copiare e modificare un obiettivo esistente.

Copiare un obiettivo esistente è utile anche se più membri del team hanno obiettivi simili ed è necessario creare un obiettivo per ciascuno di essi.

<!--
Pro-tips graphic
-->

Di seguito sono riportati alcuni aspetti da considerare prima di copiare gli obiettivi:

* Tutte le informazioni dell’obiettivo originale vengono copiate, ad eccezione del periodo dell’obiettivo (perché è nel passato).
* Puoi copiare i risultati di un obiettivo esistente che verranno trasferiti nel nuovo obiettivo.
* Per impostazione predefinita, i risultati copiati vengono assegnati allo stesso proprietario.
* Non è possibile copiare l’avanzamento dell’obiettivo esistente in un nuovo obiettivo.
* Non è possibile copiare le attività di un obiettivo durante l’operazione di copia.

## Come copiare un obiettivo

1. Fai clic sul nome di un obiettivo per aprire il pannello **[!UICONTROL Dettagli obiettivo]**.
1. Fai clic sull’icona con tre punti, quindi seleziona **[!UICONTROL Copia]**.
1. Aggiorna una delle seguenti informazioni per l’obiettivo copiato:
   * **Nuovo obiettivo:** è il nome del nuovo obiettivo. Il valore predefinito è il nome dell’obiettivo originale.
   * **Periodo:** il periodo di tempo durante il quale desideri raggiungere l’obiettivo. Seleziona un periodo di tempo dal menu a discesa o fai clic su Definisci date personalizzate per indicare un periodo di tempo personalizzato. Il periodo predefinito è sempre il trimestre corrente.
   * **Proprietario:** il proprietario dell’obiettivo. Può trattarsi di un utente, un team, un gruppo o un’azienda. L’impostazione predefinita è il proprietario dell’obiettivo originale.
   * **Descrizione:** informazioni aggiuntive inerenti l’obiettivo.

1. Controlla la casella **[!UICONTROL Copia risultati]** per verificare l’aggiunta di risultati all’obiettivo originale e desideri copiarli nel nuovo obiettivo. I risultati dell&#39;obiettivo copiato hanno lo stesso proprietario, nomi e valori misurati dei risultati dell’obiettivo originale.

1. Fai clic su **[!UICONTROL Salva]**. L’obiettivo copiato viene salvato con lo stato Bozza.

   ![Immagine del pannello [!UICONTROL Dettagli obiettivo] in [!DNL Workfront Goals] con l’opzione [!UICONTROL Copia] ](assets/03-workfront-goals-copy-a-goal.png)

1. Fai clic su **[!UICONTROL Attiva]**, in modo da aggiornare lo stato dell’obiettivo in Attivo. L’obiettivo deve avere un’attività o un risultato associato per poter essere “da attivare”.

1. Fai clic sulla **X** in alto a destra del pannello [!UICONTROL Dettagli obiettivo] per chiuderlo.

Se hai copiato un obiettivo che non era stato completato in un periodo di tempo precedente e desideri continuare a lavorarci nel periodo di tempo seguente, effettua le seguenti operazioni:

1. Passa all’obiettivo originale nella sezione **[!UICONTROL Elenco degli obiettivi]**,**[!UICONTROL Check-in]** o nella sezione **[!UICONTROL Pulse]**.
1. Commenta l’obiettivo per indicare che è stato copiato ed è stato creato un obiettivo più attuale.
1. Chiudi l’obiettivo originale per preservare i progressi compiuti durante il periodo di tempo originale. Fai clic sull’icona con i tre punti nel pannello **[!UICONTROL Dettagli obiettivo]** e seleziona **[!UICONTROL Chiudi]** dal menù.
1. Aggiorna il valore [!UICONTROL Iniziale] del nuovo risultato corrispondente al valore **[!UICONTROL Target]** del risultato precedente, in modo che l’avanzamento del nuovo obiettivo inizi a essere calcolato dal punto raggiunto nel periodo precedente.
