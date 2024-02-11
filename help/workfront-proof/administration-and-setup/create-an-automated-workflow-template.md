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
source-git-commit: 30748311c14fb8aa6b10c03a74e83f46bdb5dfbf
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 56%

---

# Creare un modello di flusso di lavoro automatizzato

In questo video scoprirai come:

* creare un modello di flusso di lavoro automatizzato per la bozza [!DNL  Workfront]
* Assegnare destinatari di bozza
* Impostare una scadenza per il processo di revisione e approvazione
* Condividere il modello di flusso di lavoro automatizzato con altri utenti

>[!VIDEO](https://video.tv.adobe.com/v/335130/?quality=12&learn=on)

## Opzioni aggiuntive di attivazione della fase

Due opzioni per determinare quando deve iniziare una fase del flusso di lavoro di correzione sono utilizzate raramente, se non mai: [!UICONTROL Data e ora] e il pulsante &quot;[!UICONTROL Quando la scadenza della fase precedente viene superata]&quot;.

La seconda opzione funziona solo in scenari in cui un ampio gruppo di persone rivede e non si desidera aspettare tutti. È una specie di opzione &quot;Ti darò un certo periodo di tempo per completare la tua recensione e poi perderai la tua occasione&quot;. Ma anche questo può rallentare il processo di revisione.

Se utilizzi effettivamente &quot;[!UICONTROL quando la scadenza della fase precedente viene superata],&quot; è importante ricordare che è possibile attivare manualmente una fase in qualsiasi momento se non si desidera attendere il superamento di una scadenza.

## Best practice

| Best practice | Ecco perché |
|---|---|
| Imposta il ruolo di bozza del creatore della bozza su Revisore. | Il ruolo bozza Revisore consente al creatore della bozza di inserire commenti e accedere ai commenti lasciati da altri utenti. Nella maggior parte dei casi, il creatore della bozza non è tenuto a prendere una decisione in merito a una bozza caricata. I ruoli bozza Approvatore, Revisore e Approvatore, Autore o Moderatore richiedono tutti di prendere una decisione. Se al creatore della bozza viene assegnato uno di questi ruoli bozza ma non prende mai decisioni, ciò può influire negativamente sulle scadenze della bozza. |
| Evita di utilizzare il ruolo bozza Approvatore. | Il ruolo bozza Approvatore non consente all’utente di aggiungere commenti alla bozza. Questo poteva comportare il rifiuto della bozza da parte di un utente, senza alcuna spiegazione, in quanto l’utente non era in grado di aggiungere commenti. Utilizza invece il ruolo bozza Revisore e Approvatore in modo che l’utente possa fornire un feedback. |
| Evita l’opzione di avviso e-mail “Tutte le attività di bozza”. | Questa opzione invia una notifica e-mail relativa alla bozza ogni volta che si verifica un evento relativo a essa: viene inserito un commento, viene inviata una risposta, viene presa una decisione, ecc. In sostanza, il destinatario visualizza l’attività della bozza non appena si verifica.<br><br>Per i proprietari e i creatori di bozze, l’avviso e-mail per le decisioni funziona meglio per i flussi di lavoro a bozza multipla e Final Decision (Decisione finale) funziona meglio per i flussi di lavoro a fase singola. In genere, tutti gli altri possono essere impostati su Disabilitato, a meno che non desiderino essere informati se altri utenti inseriscono commenti o decisioni (nel qual caso, una delle opzioni di e-mail di riepilogo potrebbe essere più utile). |
