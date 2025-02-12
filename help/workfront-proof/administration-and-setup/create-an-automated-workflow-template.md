---
title: Creare un modello di flusso di lavoro automatizzato
description: Scopri come creare un modello di flusso di lavoro automatizzato assegnando i destinatari di bozza e impostando le scadenze della bozza. Quindi condividi il modello con altri utenti.
activity: use
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
team: Technical Marketing
thumbnail: 335130.png
jira: KT-8830
last-substantial-update: 2024-01-24T00:00:00Z
exl-id: eac89e40-d3ea-4376-82a2-16bec550d131
doc-type: video
source-git-commit: d17df7162ccaab6b62db34209f50131927c0a532
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 100%

---

# Creare un modello di flusso di lavoro automatizzato

In questo video scoprirai come:

* creare un modello di flusso di lavoro automatizzato per la bozza [!DNL  Workfront]
* Assegnare destinatari di bozza
* Impostare una scadenza per il processo di revisione e approvazione
* Condividere il modello di flusso di lavoro automatizzato con altri utenti

>[!VIDEO](https://video.tv.adobe.com/v/335130/?quality=12&learn=on&enablevpops)

## Opzioni aggiuntive di attivazione della fase

Raramente, se non mai, per determinare quando dare inizio a una fase del flusso di lavoro di bozza, vengono utilizzate due opzioni: [!UICONTROL Data e ora] e l’opzione “[!UICONTROL Quando la scadenza della fase precedente viene superata]”.

La seconda opzione funziona solo in scenari in cui un ampio gruppo di persone effettua una revisione e non desideri aspettare tutti. È una sorta di opzione: “Avrai un certo periodo di tempo per completare la tua revisione e poi perderai la tua occasione”. Ma anche questo può rallentare il processo di revisione.

Se utilizzi “[!UICONTROL Scadenza fase precedente oltrepassata]”, è importante ricordare che è possibile attivare manualmente una fase in qualsiasi momento, se non si desidera attendere il superamento di una scadenza.

## Best Practice

| Best Practice | Ecco perché |
|---|---|
| Imposta il ruolo bozza del Creatore della bozza su Revisore. | Il ruolo bozza Revisore consente al creatore della bozza di inserire commenti e accedere ai commenti lasciati da altri utenti. Nella maggior parte dei casi, il creatore della bozza non è tenuto a prendere una decisione su una bozza caricata. I ruoli bozza Approvatore, Revisore e Approvatore, Autore o Moderatore richiedono tutti di prendere una decisione. Se al creatore della bozza viene assegnato uno di questi ruoli bozza ma non prende mai decisioni, ciò può influire negativamente sulle scadenze della bozza. |
| Evita di utilizzare il ruolo bozza Approvatore. | Il ruolo bozza Approvatore non consente all’utente di aggiungere commenti alla bozza. Questo potrebbe comportare il rifiuto della bozza da parte di un utente senza alcuna spiegazione, in quanto l’utente non è in grado di aggiungere commenti. Utilizza invece il ruolo bozza Revisore e Approvatore in modo che l’utente possa fornire un feedback. |
| Evita l’opzione di avviso e-mail “Tutte le attività di bozza”. | Questa opzione invia una notifica e-mail relativa alla bozza ogni volta che si verifica un evento relativo a essa: viene inserito un commento, viene inviata una risposta, viene presa una decisione, ecc. In sostanza, il destinatario visualizza l’attività della bozza non appena si verifica.<br><br>Per i proprietari e i creatori di bozze, l’avviso e-mail Decisioni funziona meglio per i flussi di lavoro di bozza a più fasi, mentre Decisione finale funziona meglio per i flussi di lavoro a fase singola. In genere, tutti gli altri possono essere impostati su Disabilitato, a meno che non desiderino essere informati se altri utenti inseriscono commenti o decisioni (nel qual caso, una delle opzioni di e-mail di riepilogo potrebbe essere più utile). |
