---
title: Comprendere più tariffe di fatturazione
description: Scopri come sostituire le tariffe di fatturazione di sistema all’interno di un progetto.
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: understand-multiple-billing-rates.png
type: Tutorial
role: User
level: Intermediate
jira: KT-10048
hide: true
exl-id: 5b1ae2c4-43bd-4382-900f-078ef84408a5
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-05T19:00:23.025Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 438
ht-degree: 93%

---

# Comprendere più tariffe di fatturazione

In [!DNL Workfront], un project manager ha la possibilità di sostituire le tariffe di fatturazione di sistema all’interno di un progetto specifico. In precedenza, quando la nuova tariffa di fatturazione veniva applicata al progetto, non influenzava solo le ore future, ma anche le ore già registrate sul progetto.

Con la nuova funzionalità di fatturazione multipla di [!DNL Workfront], il project manager è in grado di decidere il periodo di tempo in cui applicare una tariffa di fatturazione. In questo modo, se una tariffa è stata negoziata o modificata, il project manager può determinare quando tale tariffa dovrebbe diventare effettiva.

## Modificare la tariffa di fatturazione

1. Vai alla pagina di destinazione del progetto. Seleziona **[!UICONTROL Tariffe di fatturazione]** dal pannello a sinistra.

   ![Immagine della selezione [!UICONTROL Tariffe di fatturazione] in [!DNL Workfront]](assets/project-finances-1.png)

1. Dalla scheda **[!UICONTROL Tariffe di fatturazione]**, fai clic sul pulsante **[!UICONTROL Aggiungi tariffa di fatturazione]**. Seleziona **[!UICONTROL Nuova tariffa di fatturazione]** dal menu a discesa.

   ![Immagine della selezione [!UICONTROL Nuova tariffa di fatturazione] in [!DNL Workfront]](assets/project-finances-2.png)

1. Viene visualizzata la finestra di dialogo [!UICONTROL Nuova tariffa di fatturazione]. Dal menu a discesa **[!UICONTROL Mansione]**, seleziona la mansione a cui verrà applicata la nuova tariffa di fatturazione.

   ![Immagine della selezione delle mansioni in una nuova tariffa di fatturazione in [!DNL Workfront]](assets/project-finances-3.png)

1. Una volta selezionata la mansione, vengono visualizzati la [!UICONTROL Tariffa di fatturazione predefinita] e il campo [!UICONTROL Tariffa di fatturazione 1]. Inserisci la nuova tariffa di fatturazione nel campo [!UICONTROL Tariffa di fatturazione 1]. Se la tariffa di fatturazione si applica all’intero progetto (ore passate, presenti e future registrate), fai clic sul pulsante **[!UICONTROL Salva]**.

   ![Immagine che mostra come salvare una nuova tariffa di fatturazione applicabile all’intero progetto in [!DNL Workfront]](assets/project-finances-5.png)

1. Se la nuova tariffa di fatturazione si applica solo per un determinato periodo di tempo, fai clic sul pulsante **[!UICONTROL Aggiungi tariffa]**. Vengono visualizzati i campi [!UICONTROL Data di fine della tariffa di fatturazione 1] e [!UICONTROL Tariffa di fatturazione 2]. Inserisci la data di fine per la [!UICONTROL Tariffa di fatturazione 1]. Non è possibile immettere una data di inizio per la [!UICONTROL Tariffa di fatturazione 1] perché il sistema presuppone che sia stata avviata all’inizio del progetto.

   ![Immagine che mostra la creazione di una nuova tariffa di fatturazione per un determinato periodo di tempo, a partire dall’inizio del progetto in [!DNL Workfront]](assets/project-finances-6.png)

1. In caso contrario:

   * inserisci la tariffa di fatturazione predefinita per la [!UICONTROL Tariffa di fatturazione 1].
   * Seleziona la data di fine per la [!UICONTROL Tariffa di fatturazione 1] ([!UICONTROL Tariffa di fatturazione predefinita]).
   * La data di inizio per la [!UICONTROL Tariffa di fatturazione 2] verrà impostata automaticamente nel giorno successivo al termine della [!UICONTROL Tariffa di fatturazione 1].
   * Inserisci la tariffa di fatturazione desiderata nella sezione [!UICONTROL Tariffa di fatturazione 2].
   * Continua ad aggiungere tariffe di fatturazione, in base alle esigenze, facendo clic sul pulsante **[!UICONTROL Aggiungi tariffa]**.
   * Al termine, fai clic su **[!UICONTROL Salva]**.
   * Tutte le tariffe di fatturazione saranno visualizzate nella scheda [!UICONTROL Tariffe di fatturazione] nel progetto.

   ![Immagine della creazione di nuove tariffe di fatturazione che si applicano ai diversi periodi di tempo in [!DNL Workfront]](assets/project-finances-7.png)
