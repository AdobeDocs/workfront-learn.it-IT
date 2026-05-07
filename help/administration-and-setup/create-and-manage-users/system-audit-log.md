---
title: Informazioni sul registro di controllo del sistema
description: Scopri come utilizzare il registro di controllo del sistema per rivedere quando sono state apportate modifiche e quando queste sono state apportate agli elementi.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Beginner, Intermediate
thumbnail: 10040.jpeg
jira: KT-10040
exl-id: 9de6fd40-10fb-47a6-b186-3a38c411f1ac
TQID: https://experienceleague.adobe.com/xMxWQ53TUXVjS-H8EuK3nf7jt8v4vUgKoZVsmApc-JM
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2: id: d095671a-1355-40aa-8b5f-06c33c68080bid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 36674ed53c8645f556862bb2d99f3bfd6c993c1e
workflow-type: tm+mt
source-wordcount: 267
ht-degree: 100%

---

# Informazioni sul registro di controllo del sistema

Il registro di controllo del sistema è il modo migliore a disposizione dell’amministratore di sistema per tenere d’occhio cosa sta succedendo in [!DNL Workfront]. Considera il registro come fonte attendibili per controllare chi ha apportato delle modifiche e quando.

Accedi al registro di controllo andando nella sezione [!UICONTROL Preferenze] nell’area [!UICONTROL Configurazione]. Per impostazione predefinita, vengono visualizzati i dati degli ultimi sette giorni. Modifica i criteri di filtro per visualizzare i dati in intervalli di date differenti.

Quando un utente esegue determinate azioni, [!UICONTROL Workfront] le registra nella sezione [!UICONTROL Registri di controllo] dell’area [!UICONTROL Configurazione].

Menu a discesa ![[!UICONTROL Tipo di registro] nella pagina [!UICONTROL Registri di controllo] in [!UICONTROL Configurazione]](assets/admin-fund-audit-log-1.png)

Ogni azione registrata o a cui è stato effettuato l’accesso mostra:

* data e ora della modifica
* Tipo di registro
* Nome dell’utente che ha completato l’azione
* Oggetto
* Qualsiasi dettaglio associato all’azione
* Indirizzo IP

Elenco del ![[!UICONTROL Registro di controllo]](assets/admin-fund-audit-log-2.JPG)

## Esportare il registro di controllo

L’esportazione dei dati del registro di controllo consente agli amministratori di sistema di condividere le informazioni con revisori interni/esterni o specialisti della sicurezza. Alcune organizzazioni richiedono che determinati registri vengano conservati per conformarsi alle normative sulla sicurezza informatica. Altre hanno bisogno delle informazioni importate in un sistema di sicurezza per l’analisi.

I registri di controllo possono essere esportati in un file CSV (valori separati da virgole), che può essere aperto in un’applicazione per fogli di calcolo o in un editor di testo normale. L’esportazione è limitata a 50.000 righe alla volta. Pertanto, se il totale supera le 50.000 righe, restringi l’elenco utilizzando i filtri.

Pulsante ![[!UICONTROL Esporta] nella pagina [!UICONTROL Registri di controllo]](assets/admin-fund-audit-log-3.png)

<!--
learn more URLs
Audit logs
Managing audit logs
-->
