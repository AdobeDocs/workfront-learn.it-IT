---
title: Imposta i ruoli bozza predefiniti
description: Scopri come impostare il ruolo bozza predefinito assegnato quando vengono creati nuovi utenti o viene aperta una bozza.
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
thumbnail: set-default-proof-roles.png
jira: KT-10235
last-substantial-update: 2024-01-23T00:00:00Z
exl-id: 77dfb9f1-3242-47ca-a0ce-203b535af156
source-git-commit: 731005176bc02e3a4d26d00373931fa7444afeea
workflow-type: tm+mt
source-wordcount: '359'
ht-degree: 0%

---

# Imposta i ruoli bozza predefiniti



La prima impostazione predefinita da completare consiste nel determinare un ruolo di bozza predefinito che verrà assegnato quando vengono creati nuovi utenti o si apre una bozza.

I ruoli di bozza determinano ciò che un utente è in grado di fare con una bozza: basta guardarla, fare commenti, approvarla, ecc. [!DNL Workfront] consiglia di impostare le impostazioni predefinite del ruolo bozza per tutti gli utenti, in modo da velocizzare e semplificare l’aggiunta di destinatari alle bozze e la configurazione dei flussi di lavoro.

![È possibile selezionare i ruoli della bozza durante il caricamento della bozza](assets/proof-system-setups-proof-role-example.png)

Tuttavia, questo ruolo di bozza predefinito può essere modificato durante il caricamento delle singole bozze, affinché tutti possano svolgere il ruolo richiesto nel processo di revisione e approvazione.


## Imposta i ruoli bozza predefiniti

1. Seleziona **Configurazione** dal [!UICONTROL Menu principale].
1. Seleziona **Revisione e approvazione** dal menu a sinistra.
1. Fai clic sul pulsante accanto al ruolo di bozza predefinito desiderato per entrambe le nuove [!DNL Workfront] utenti e utenti di bozze guest per &quot;destinatari designati&quot;: tutti gli utenti che vengono aggiunti al flusso di lavoro della bozza, manualmente o tramite un modello di flusso di lavoro.
1. Fai clic sul pulsante accanto al ruolo di bozza predefinito desiderato per entrambe le nuove [!DNL Workfront] utenti e utenti di prova ospiti per utenti &quot;non destinatari&quot;. Questi sono generalmente [!DNL Workfront] utenti che hanno accesso a una bozza ma non sono tra le persone assegnate al flusso di lavoro.
1. Salva le modifiche.

![Impostazioni di revisione e approvazione in Workfront](assets/proof-system-setups-workfront-defaults.png)

Considera cosa dovrebbero fare la maggior parte degli utenti e degli ospiti quando vengono aggiunti a un flusso di lavoro di verifica. Questo dovrebbe essere il tuo valore predefinito.

## Best practice

| Best practice | Ecco perché |
|---|---|
| Utilizzare solo Read Only o Reviewer per l&#39;impostazione &quot;Roles for non-recipients that open a document proof&quot; (Ruoli per non destinatari che aprono una bozza di documento) in Workfront. | Tutte le altre opzioni per questa impostazione richiedono una decisione di bozza, che può far deragliare il flusso di lavoro di bozza. In genere, gli utenti che non vengono aggiunti al flusso di lavoro della bozza devono solo visualizzarla o aggiungere commenti, non approvare la bozza, pertanto le opzioni Sola lettura o Revisore sono la scelta migliore. <br> <br>Nota: questa impostazione si trova nel menu principale di Workfront > Impostazione > Revisione e approvazione. |
