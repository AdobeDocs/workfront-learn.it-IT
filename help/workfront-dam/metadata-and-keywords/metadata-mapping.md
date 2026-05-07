---
title: Configurare la mappatura dei metadati
description: Scopri come configurare la mappatura dei metadati per [!UICONTROL Workfront DAM].
activity: use
team: Technical Marketing
feature: Digital Content and Documents
type: Tutorial
role: Admin
level: Intermediate
jira: KT-10088
exl-id: 3869db93-9fbc-4689-b838-0f4400a436c3
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2: id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-05T22:32:59.006Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 276
ht-degree: 100%

---

# Configurare la mappatura dei metadati

Le informazioni relative a[!DNL Workfront]su una risorsa possono essere trasferite da [!DNL Workfront] a [!UICONTROL Workfront DAM] insieme alla risorsa. L’opzione di mappatura dei metadati nell’area [!DNL Workfront] [!UICONTROL Configurazione] consente questo trasferimento di informazioni.

Parla con il tuo consulente di [!DNL Workfront] per ricevere consigli sulle best practice relative alla configurazione della mappatura dei metadati.

Devi essere un amministratore [!DNL Workfront] e un amministratore [!UICONTROL Workfront DAM] per impostare la mappatura dei metadati. Prima di iniziare, è necessario collegare i tuoi account [!DNL Workfront] e [!UICONTROL Workfront DAM].

## Connetti account

1. Accedi a [!DNL Workfront].
1. Apri un progetto, un’attività o un problema e fai clic sulla scheda **[!UICONTROL Documenti]**.
1. Fai clic sul pulsante **[!UICONTROL Aggiungi nuovo]** e seleziona **[!UICONTROL Da Workfront DAM]** dal menu a discesa.
1. Immetti il nome di accesso e la password nella casella di autorizzazione [!UICONTROL Workfront DAM] che viene visualizzata.
1. Quindi, fai clic su **[!UICONTROL Sì]** per dare accesso a [!DNL Workfront] all’account [!UICONTROL Workfront DAM].
1. Se necessario, aggiorna la pagina per aggiornare l’accesso a [!UICONTROL Workfront DAM].

Una volta stabilita questa connessione, puoi iniziare a mappare i metadati tra i due sistemi. Assicurati di aver già creato i campi di metadati necessari in [!UICONTROL Workfront DAM] prima di iniziare la mappatura.

## Configurare la mappatura

1. Accedi a [!DNL Workfront].
1. Seleziona **[!UICONTROL Configurazione]** dal [!UICONTROL Menu principale].
1. Espandi la sezione **[!UICONTROL Documenti]** nel menu del pannello a sinistra.
1. Quindi fai clic su **[!UICONTROL Mappatura metadati]**.
1. Nel campo Workfront, digita l’origine del campo del campo [!DNL Workfront] da mappare.
1. Quindi seleziona il campo di metadati **[!UICONTROL Workfront DAM]** corrispondente o di destinazione.
1. Fai clic sul pulsante **[!UICONTROL Aggiungi mappatura]**.
1. Vedrai il [!UICONTROL campo di origine Workfront] e il [!UICONTROL campo di destinazione Workfront DAM] nel grafico nella parte inferiore della finestra.
1. Ripeti l’operazione per tutti i campi di metadati desiderati.

![Schermata della [!UICONTROL Mappatura dei metadati] in [!DNL Workfront]](assets/01-metadata-mapping.png)
