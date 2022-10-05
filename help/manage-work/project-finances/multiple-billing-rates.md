---
title: Comprendere i tassi di fatturazione multipli
description: In Workfront, un project manager può ignorare le tariffe di fatturazione del sistema all'interno di un progetto specifico.
feature: Work Management
thumbnail: understand-multiple-billing-rates.png
type: Tutorial
role: User
level: Intermediate
kt: 10048
exl-id: bda562b9-f8da-49c9-bea7-0440fdc4c24c
source-git-commit: d0c842ad8bf6f52161f003a62237fbcd35d23176
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 0%

---

# Comprendere i tassi di fatturazione multipli

Within [!DNL Workfront], un project manager può ignorare le tariffe di fatturazione del sistema all’interno di un progetto specifico. Precedentemente, quando il nuovo tasso di fatturazione veniva applicato al progetto, non solo influenzava le ore future, ma le ore già registrate sul progetto.

Con [!DNL Workfront]La nuova funzionalità di tasso di fatturazione multiplo, il project manager è in grado di decidere quale periodo di tempo applicare un tasso di fatturazione. In questo modo, se un tasso è stato negoziato o modificato, il project manager può determinare quando tale tasso dovrebbe avere effetto.

## Modificare il tasso di fatturazione

1. Vai alla pagina di destinazione del progetto. Seleziona **[!UICONTROL Tassi di fatturazione]** dal pannello a sinistra.

   ![Immagine di selezione [!UICONTROL Tassi di fatturazione] in [!DNL Workfront]](assets/project-finances-1.png)

1. Da **[!UICONTROL Tassi di fatturazione]** fai clic sulla scheda **[!UICONTROL Aggiungi tasso di fatturazione]** pulsante . Seleziona **[!UICONTROL Nuovo tasso di fatturazione]** dal menu a discesa .

   ![Immagine di selezione [!UICONTROL Nuovo tasso di fatturazione] in [!DNL Workfront]](assets/project-finances-2.png)

1. La [!UICONTROL Nuovo tasso di fatturazione] viene visualizzata la finestra di dialogo. Da **[!UICONTROL Ruolo]** a discesa, seleziona il ruolo del processo a cui verrà applicato il nuovo tasso di fatturazione.

   ![Immagine della selezione di ruoli di lavoro in un nuovo tasso di fatturazione in [!DNL Workfront]](assets/project-finances-3.png)

1. Una volta selezionato il ruolo di lavoro, il [!UICONTROL Tasso di fatturazione predefinito] e [!UICONTROL Tasso di fatturazione 1] viene visualizzato il campo . Inserisci il nuovo tasso di fatturazione nel [!UICONTROL Tasso di fatturazione 1] campo . Se il tasso di fatturazione è applicabile all&#39;intero progetto (ore passate, presenti e future registrate), fai clic sul pulsante **[!UICONTROL Salva]** pulsante .

   ![Immagine del salvataggio di un nuovo tasso di fatturazione applicabile all&#39;intero progetto in [!DNL Workfront]](assets/project-finances-5.png)

1. Se il nuovo tasso di fatturazione si applica solo per un determinato periodo di tempo, fai clic sul pulsante **[!UICONTROL Aggiungi tasso]** pulsante . La [!UICONTROL Data di fine tasso di fatturazione 1] e [!UICONTROL Tasso di fatturazione 2] vengono visualizzati i campi. Immettere la data di fine per [!UICONTROL Tasso di fatturazione 1]. Non è possibile inserire una data di inizio per [!UICONTROL Tasso di fatturazione 1] poiché il sistema presuppone che sia stato avviato all’inizio del progetto.

   ![Immagine della creazione di un nuovo tasso di fatturazione applicabile a un determinato periodo di tempo, a partire dall&#39;inizio del progetto in [!DNL Workfront]](assets/project-finances-6.png)

1. In caso contrario:

   * Immettere il tasso di fatturazione predefinito per [!UICONTROL Tasso di fatturazione 1].
   * Selezionare la data di fine per [!UICONTROL Tasso di fatturazione 1] ([!UICONTROL Tasso di fatturazione predefinito]).
   * Data di inizio per [!UICONTROL Tasso di fatturazione 2] viene automaticamente impostato sul giorno successivo a [!UICONTROL Tasso di fatturazione 1] termina.
   * Inserisci il tasso di fatturazione desiderato nel [!UICONTROL Tasso di fatturazione 2] sezione .
   * Continua ad aggiungere le tariffe di fatturazione, se necessario, facendo clic sul pulsante **[!UICONTROL Aggiungi tasso]** pulsante .
   * Al termine, fai clic su **[!UICONTROL Salva]**.
   * Tutte le tariffe di fatturazione verranno visualizzate nella [!UICONTROL Tassi di fatturazione] nel progetto.
   ![Immagine della creazione di nuovi tassi di fatturazione applicabili ai diversi periodi di tempo in [!DNL Workfront]](assets/project-finances-7.png)
