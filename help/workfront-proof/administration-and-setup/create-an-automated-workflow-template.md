---
title: Creare un modello di flusso di lavoro automatizzato
description: Scopri come creare un modello di flusso di lavoro automatizzato assegnando i destinatari della bozza e impostando le scadenze della bozza. Quindi condividi il modello con altri utenti.
activity: use
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
team: Technical Marketing
thumbnail: 335130.png
jira: KT-8830
last-substantial-update: 2024-01-23T00:00:00Z
exl-id: eac89e40-d3ea-4376-82a2-16bec550d131
doc-type: video
source-git-commit: 731005176bc02e3a4d26d00373931fa7444afeea
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 0%

---

# Creare un modello di flusso di lavoro automatizzato

Questo video illustra come:

* Crea un modello di flusso di lavoro automatizzato per [!DNL  Workfront] prova
* Assegna destinatari bozza
* Impostare una scadenza per il processo di revisione e approvazione
* Condividere il modello di workflow automatizzato con altri utenti

>[!VIDEO](https://video.tv.adobe.com/v/335130/?quality=12&learn=on)

## Opzioni aggiuntive di attivazione della fase

Due opzioni per determinare quando deve iniziare una fase del flusso di lavoro di correzione sono utilizzate raramente, se non mai: [!UICONTROL Data e ora] e il pulsante &quot;[!UICONTROL Quando la scadenza della fase precedente viene superata]&quot;.

La seconda opzione funziona solo in scenari in cui un ampio gruppo di persone rivede e non si desidera aspettare tutti. È una specie di opzione &quot;Ti darò un certo periodo di tempo per completare la tua recensione e poi perderai la tua occasione&quot;. Ma anche questo può rallentare il processo di revisione.

Se utilizzi effettivamente &quot;[!UICONTROL quando la scadenza della fase precedente viene superata],&quot; è importante ricordare che è possibile attivare manualmente una fase in qualsiasi momento se non si desidera attendere il superamento di una scadenza.

## Best practice

| Best practice | Ecco perché |
|---|---|
| Imposta il ruolo di bozza del creatore della bozza su Revisore. | Il ruolo Bozza revisore consente al creatore della bozza di inserire commenti e accedere ai commenti lasciati da altri utenti. Nella maggior parte dei casi, il creatore della bozza non è tenuto a prendere una decisione in merito a una bozza caricata. I ruoli Approvatore, Revisore e Approvatore, Autore o Moderatore della bozza richiedono tutti una decisione. Se al creatore della bozza viene assegnato uno di questi ruoli di bozza ma non prende mai una decisione, ciò può influenzare negativamente le scadenze della bozza. |
| Evita di usare il ruolo di bozza Approvatore. | Il ruolo Bozza approvatore non consente all’utente di aggiungere commenti a questa bozza. Questo poteva comportare il rifiuto della bozza da parte di un utente, senza alcuna spiegazione, in quanto l’utente non era in grado di aggiungere commenti. Utilizza invece il ruolo di bozza Revisore e Approvatore in modo che l’utente possa fornire un feedback. |
| Evita l’opzione di avviso e-mail All Activity proof (Tutte le attività). | Questa opzione invia una notifica e-mail relativa alla bozza ogni volta che si verifica un evento con una bozza: viene inserito un commento, viene inviata una risposta, viene presa una decisione, ecc. In sostanza, il destinatario vede l’attività della bozza così come si verifica.<br><br>Per i proprietari e i creatori di bozze, l’avviso e-mail per le decisioni funziona meglio per i flussi di lavoro a bozza multipla e Final Decision (Decisione finale) funziona meglio per i flussi di lavoro a fase singola. In genere, tutti gli altri possono essere impostati su Disabilitato, a meno che non desiderino essere informati di altri utenti che stanno prendendo commenti o decisioni (nel qual caso, una delle opzioni di riepilogo dell’e-mail potrebbe funzionare meglio). |
