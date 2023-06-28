---
title: Copia un obiettivo esistente
description: Scopri come copiare un obiettivo esistente in [!DNL Workfront Goals].
activity: use
team: Technical Marketing
feature: Workfront Goals
type: Tutorial
role: User
level: Beginner
jira: KT-10121
exl-id: bf9ac10a-8419-458b-b4e8-bedb0ad3b98f
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '525'
ht-degree: 0%

---

# Copia un obiettivo esistente

Supponiamo che sia la fine di un trimestre e desideri ricreare un obiettivo esistente per il periodo successivo. O forse non hai completato l’obiettivo e devi estenderlo al periodo di tempo successivo. Qual è l’opzione migliore per creare tale obiettivo? Si desidera copiare e modificare un obiettivo esistente.

Copiare un obiettivo esistente è utile anche se più membri del gruppo hanno obiettivi simili e devi creare un obiettivo per ciascuno di essi.

<!--
Pro-tips graphic
-->

Di seguito sono riportati alcuni aspetti da considerare prima di copiare gli obiettivi:

* Tutte le informazioni dell’obiettivo originale vengono copiate, ad eccezione del periodo dell’obiettivo (perché è nel passato).
* Puoi copiare i risultati di un obiettivo esistente e trasferirli nel nuovo obiettivo.
* Per impostazione predefinita, i risultati copiati vengono assegnati allo stesso proprietario.
* Non è possibile copiare l’avanzamento dell’obiettivo esistente in un nuovo obiettivo.
* Non è possibile copiare le attività di un obiettivo quando si copia un obiettivo.

## Come copiare un obiettivo

1. Fai clic sul nome di un obiettivo per aprire **[!UICONTROL Dettagli obiettivo]** pannello.
1. Fai clic sull’icona a 3 punti, quindi seleziona **[!UICONTROL Copia]**.
1. Aggiorna una delle seguenti informazioni per l&#39;obiettivo copiato:
   * **Nuovo obiettivo**- Nome del nuovo obiettivo. L&#39;impostazione predefinita è il nome dell&#39;obiettivo originale.
   * **Periodo**- Periodo di tempo durante il quale si desidera raggiungere l&#39;obiettivo. Seleziona un periodo di tempo dal menu a discesa o fai clic su Definisci date personalizzate per indicare un periodo di tempo personalizzato. Il periodo predefinito è sempre il trimestre corrente.
   * **Proprietario**- Il proprietario dell&#39;obiettivo. Può essere un utente, un team, un gruppo o un’azienda. L&#39;impostazione predefinita è il proprietario dell&#39;obiettivo originale.
   * **Descrizione**- Informazioni aggiuntive sull&#39;obiettivo.

1. Controlla la **[!UICONTROL Copia risultati]** casella se all&#39;obiettivo originale sono stati aggiunti risultati e si desidera copiarli nel nuovo obiettivo. I risultati dell&#39;obiettivo copiato hanno lo stesso proprietario, gli stessi nomi e gli stessi valori misurati dei risultati dell&#39;obiettivo originale.

1. Fai clic su **[!UICONTROL Salva]**. L&#39;obiettivo copiato viene salvato con lo stato Bozza.

   ![Un&#39;immagine del [!UICONTROL Dettagli obiettivo] pannello in [!DNL Workfront Goals] con [!UICONTROL Copia] opzione](assets/03-workfront-goals-copy-a-goal.png)

1. Clic **[!UICONTROL Attiva]**, che aggiorna lo stato dell’obiettivo su Attivo. Per poter &quot;attivare&quot; l&#39;obiettivo deve avere un&#39;attività o un risultato associato.

1. Fai clic su **X** in alto a destra nella [!UICONTROL Dettagli obiettivo] per chiuderlo.

Se hai copiato un obiettivo che non era stato completato in un periodo di tempo precedente e desideri continuare a lavorarci nel periodo di tempo seguente, effettua le seguenti operazioni:

1. Vai all’obiettivo originale in **[!UICONTROL Elenco obiettivi]**, **[!UICONTROL Check-in]** sezione, oppure **[!UICONTROL Pulse]** sezione.
1. Commento sull&#39;obiettivo per indicare che è stato copiato ed è stato creato un obiettivo più corrente.
1. Chiudere l&#39;obiettivo originale per mantenere l&#39;avanzamento effettuato durante il periodo di tempo originale. Fai clic sull’icona a tre punti in **[!UICONTROL Dettagli obiettivo]** e seleziona **[!UICONTROL Chiudi]** dal menu.
1. Aggiornare il [!UICONTROL Iniziale] valore del nuovo risultato corrispondente al **[!UICONTROL Target]** valore del risultato precedente, in modo che l’avanzamento del nuovo obiettivo inizi a essere calcolato dal punto raggiunto nel periodo precedente.
