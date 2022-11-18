---
title: Comprendere l'accesso finanziario
description: Scopri come i diritti di accesso finanziario consentono agli amministratori di controllare chi può visualizzare e modificare le informazioni finanziarie tracciate in Workfront.
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: understand-financial-access.png
type: Tutorial
role: User
level: Intermediate
kt: 10067
exl-id: 1c3d724a-8ff0-466f-9416-cff3da59c8ea
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 5%

---

# Comprendere l&#39;accesso finanziario

Se la tua organizzazione acquisisce dati finanziari con [!DNL Workfront], in qualità di amministratore di sistema, è tua responsabilità proteggere e gestire gli utenti che hanno accesso per visualizzare e modificare tali informazioni.

Sono necessari due elementi per consentire a un utente di visualizzare o modificare le informazioni finanziarie:

1. I diritti di accesso devono essere attivati nella [!UICONTROL Livello di accesso].
2. L&#39;autorizzazione all&#39;utilizzo di tali diritti di accesso deve essere concessa in base all&#39;oggetto.

Ad esempio, a un utente possono essere concessi i diritti per visualizzare i dati finanziari nel loro livello di accesso, ma possono visualizzare solo i dati finanziari su un&#39;attività che è sia condivisa con loro che la visualizzazione finanziaria è abilitata nella condivisione di tale attività.

Quindi è possibile per un utente con [!UICONTROL Livello di accesso] diritti di visualizzare i dati finanziari per poter visualizzare i dati finanziari su alcuni oggetti e non su altri, a seconda delle singole opzioni di condivisione di tali oggetti. Tuttavia, nessun utente può visualizzare i dati finanziari su qualsiasi oggetto a meno che non abbia il diritto loro conferito nel loro [!UICONTROL Livello di accesso].

## [!UICONTROL Livello di accesso] impostazioni

L&#39;accesso generale ai dati finanziari è concesso per primo da [!DNL Workfront] tipo di licenza.

**[!UICONTROL Pianificare] le licenze possono:**

* Gestire i record di fatturazione
* Gestisci e visualizza la fatturazione dei ruoli e le tariffe dei costi
* Gestione e visualizzazione della fatturazione e dei tassi di costo degli utenti
* Gestione delle spese
* Visualizza e modifica le finanze

**[!UICONTROL Lavoro] le licenze possono:**

* Gestione delle spese
* Visualizza finanze

**[!UICONTROL Revisione] le licenze possono:**

* Visualizza finanze

**Le autorizzazioni possono essere modificate dal [!UICONTROL Livello di accesso]. Le tre opzioni per l&#39;accesso ai dati finanziari sono:**

* [!UICONTROL Nessun accesso] — L&#39;utente non sarà in grado di visualizzare informazioni finanziarie.
* [!UICONTROL Visualizza] — L&#39;utente può rivedere e condividere le informazioni.
* [!UICONTROL Modifica] — L’utente può creare, modificare, eliminare e condividere le informazioni. (Disponibile solo per una licenza Plan).

![Immagine che mostra le opzioni generali di Financial Data in un livello di accesso](assets/setting-up-finances-8.png)

È importante notare che la [!UICONTROL Visualizza] e [!UICONTROL Modifica] le opzioni dispongono di impostazioni aggiuntive per [!UICONTROL Pianificare] licenza. Fai clic sull’ingranaggio [!UICONTROL Visualizza] pulsante per le seguenti opzioni:

**[!UICONTROL Visualizza]**

* Visualizza fatturazione mansione e tassi di costo
* Visualizza fatturazione utente e tassi di costo

![Immagine che mostra le opzioni di visualizzazione Dati finanziari in un livello di accesso](assets/setting-up-finances-9.png)

**[!UICONTROL Modifica]**

Queste due opzioni sono disponibili nella sezione [!UICONTROL Modifica] insieme a:

* Modifica fatturazione mansione e tassi di costo
* Modifica fatturazione utente e tassi di costo

![Immagine che mostra le opzioni di modifica dei dati finanziari a livello di accesso](assets/setting-up-finances-10.png)

>[!NOTE]
>
>Un utente con accesso per aggiungere spese può anche visualizzare le spese che aggiungono, così come le spese aggiunte dai loro rapporti diretti.
