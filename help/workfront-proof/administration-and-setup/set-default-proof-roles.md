---
title: Impostare ruoli di bozza predefiniti
description: Scopri come impostare il ruolo di bozza predefinito assegnato quando vengono creati nuovi utenti o viene aperta una bozza.
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
thumbnail: set-default-proof-roles.png
jira: KT-10235
last-substantial-update: '2024-01-24T00:00:00.000Z'
exl-id: 77dfb9f1-3242-47ca-a0ce-203b535af156
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2: id: b18b693b-6d59-4359-95fd-a386b7a615fe
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-05T20:03:40.797Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 362
ht-degree: 87%

---

# Impostare ruoli di bozza predefiniti



La prima impostazione predefinita da completare consiste nel determinare un ruolo di bozza predefinito che verrà assegnato quando vengono creati nuovi utenti o si apre una bozza.

I ruoli di bozza determinano ciò che un utente è in grado di fare con una bozza: basta guardarla, fare commenti, approvarla, ecc. [!DNL Workfront] consiglia di impostare le impostazioni predefinite del ruolo di bozza per tutti gli utenti, per rendere più rapida e semplice l&#39;aggiunta di destinatari alle bozze e l&#39;impostazione di flussi di lavoro.

![È possibile selezionare i ruoli di bozza durante il caricamento della bozza](assets/proof-system-setups-proof-role-example.png)

Tuttavia, questo ruolo di bozza predefinito può essere modificato durante il caricamento delle singole bozze, affinché tutti possano svolgere il ruolo richiesto nel processo di revisione e approvazione.


## Impostare ruoli di bozza predefiniti

1. Seleziona **Configurazione** dal [!UICONTROL Menu principale].
1. Seleziona **Revisione e approvazione** dal menu a sinistra.
1. Fai clic sul pulsante accanto al ruolo di bozza predefinito desiderato sia per i nuovi utenti di [!DNL Workfront] che per gli utenti di bozze guest per “destinatari designati”: tutti gli utenti che vengono aggiunti al flusso di lavoro di bozza, manualmente o tramite un modello di flusso di lavoro.
1. Fai clic sul pulsante accanto al ruolo di bozza predefinito desiderato sia per i nuovi utenti di [!DNL Workfront] che per gli utenti di bozze guest per gli utenti “non destinatari”. Questi sono generalmente utenti di [!DNL Workfront] che hanno accesso a una bozza ma non sono una delle persone assegnate al flusso di lavoro.
1. Salva le modifiche.

![Impostazioni di revisione e approvazione in Workfront](assets/proof-system-setups-workfront-defaults.png)

Considera cosa dovrà fare la maggior parte dei tuoi utenti e guest quando verranno aggiunti a un flusso di lavoro di bozza. Questo dovrebbe essere il tuo valore predefinito.

## Best Practice

| Best Practice | Ecco perché |
|---|---|
| Utilizza esclusivamente l’impostazione di Workfront Solo lettura o Revisore per “Ruoli non destinatari che aprono la bozza di un documento”. | Le altre opzioni per questa impostazione richiedono tutte una Decisione bozza, che può ostacolare il flusso di lavoro di bozza. In genere, le persone non aggiunte al flusso di lavoro di bozza devono solo visualizzarla o aggiungere commenti, non devono approvarla, pertanto le opzioni Sola lettura o Revisore sono la scelta migliore.<br> <br>Nota: questa impostazione si trova nel menu principale di Workfront > Configurazione > Revisione e approvazione. |
