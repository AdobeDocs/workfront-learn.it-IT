---
title: Comprendere l’accesso finanziario
description: Scopri come i diritti di accesso finanziario consentono agli amministratori di controllare chi può visualizzare e modificare le informazioni finanziarie tracciate in Workfront.
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: understand-financial-access.png
type: Tutorial
role: User
level: Intermediate
jira: KT-10067
exl-id: 1c3d724a-8ff0-466f-9416-cff3da59c8ea
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 5%

---

# Comprendere l’accesso finanziario

Se l’organizzazione acquisisce dati finanziari con [!DNL Workfront]In qualità di amministratore di sistema, è tua responsabilità proteggere e gestire gli utenti che hanno accesso alla visualizzazione e alla modifica di tali informazioni.

Per consentire a un utente di visualizzare o modificare le informazioni finanziarie sono necessari due elementi:

1. I diritti di accesso devono essere abilitati in [!UICONTROL Livello d&#39;Accesso].
2. L’autorizzazione a utilizzare tali diritti di accesso deve essere concessa oggetto per oggetto.

Ad esempio, a un utente possono essere concessi i diritti per visualizzare i dati finanziari nel proprio livello di accesso, ma può visualizzare solo i dati finanziari su un’attività condivisa con lui e la visualizzazione finanziaria è abilitata nella condivisione di tale attività.

Quindi è possibile per un utente con [!UICONTROL Livello d&#39;Accesso] diritti di visualizzare i dati finanziari per poter visualizzare i dati finanziari su alcuni oggetti e non su altri, a seconda delle singole opzioni di condivisione di tali oggetti. Tuttavia, nessun utente può visualizzare i dati finanziari su qualsiasi oggetto a meno che non abbia il diritto dato loro nel [!UICONTROL Livello d&#39;Accesso].

## [!UICONTROL Livello d&#39;Accesso] impostazioni

L&#39;accesso generale ai dati finanziari è concesso in primo luogo da [!DNL Workfront] tipo di licenza.

**[!UICONTROL Piano] Le licenze possono:**

* Gestisci record fatturazione
* Gestire e visualizzare la fatturazione dei ruoli e i tassi di costo
* Gestire e visualizzare la fatturazione utente e le tariffe di costo
* Gestione spese
* Visualizza e modifica dati finanziari

**[!UICONTROL Lavoro] Le licenze possono:**

* Gestione spese
* Visualizza dati finanziari

**[!UICONTROL Revisione] Le licenze possono:**

* Visualizza dati finanziari

**Le autorizzazioni possono essere modificate da [!UICONTROL Livello d&#39;Accesso]. Le tre opzioni per l’accesso ai dati finanziari sono:**

* [!UICONTROL Nessun accesso] — L&#39;utente non sarà in grado di visualizzare le informazioni finanziarie.
* [!UICONTROL Visualizza] — L&#39;utente può esaminare e condividere le informazioni.
* [!UICONTROL Modifica] — L&#39;utente può creare, modificare, eliminare e condividere le informazioni. Disponibile solo per una licenza Full.

![Immagine che mostra le opzioni generali di Financial Data in un livello di accesso](assets/setting-up-finances-8.png)

È importante notare che il [!UICONTROL Visualizza] e [!UICONTROL Modifica] opzioni hanno impostazioni aggiuntive per un [!UICONTROL Piano] licenza. Fai clic sull’ingranaggio nella [!UICONTROL Visualizza] per queste opzioni:

**[!UICONTROL Visualizza]**

* Visualizza fatturazione mansione e tassi di costo
* Visualizza fatturazione utente e tassi di costo

![Immagine che mostra le opzioni della visualizzazione Dati finanziari in un livello di accesso](assets/setting-up-finances-9.png)

**[!UICONTROL Modifica]**

Queste due opzioni sono disponibili nel [!UICONTROL Modifica] , insieme a:

* Modifica fatturazione mansione e tassi di costo
* Modifica fatturazione utente e tassi di costo

![Immagine che mostra le opzioni di modifica dei dati finanziari in un livello di accesso](assets/setting-up-finances-10.png)

>[!NOTE]
>
>Un utente con accesso per aggiungere spese può anche visualizzare le spese che aggiunge, così come le spese aggiunte dai suoi referenti diretti.
