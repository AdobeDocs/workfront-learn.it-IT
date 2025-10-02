---
title: Configurare gruppi e utenti
description: Scopri come creare cartelle, gruppi e utenti in [!UICONTROL Workfront DAM]. Informazioni sui tipi di ruolo utente e concessioni delle autorizzazioni alle cartelle.
activity: use
feature: Digital Content and Documents
type: Tutorial
role: Admin
level: Intermediate
team: Technical Marketing
jira: KT-8967
exl-id: 4ebf675c-b72d-447e-b131-a89acb449e15
doc-type: video
source-git-commit: bbdf99c6bc1be714077fd94fc3f8325394de36b3
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 95%

---

# Configurare gruppi e utenti

In questo video scoprirai come:

* le impostazioni di gruppo influiscono sull’accesso alle risorse
* Creare cartelle, gruppi e utenti in un ordine specifico
* Comprendere i tipi di ruolo utente
* Concedere autorizzazioni alle cartelle
* Creare e modificare gruppi
* Aggiungere e modificare utenti

>[!VIDEO](https://video.tv.adobe.com/v/335230/?quality=12&learn=on&enablevpops=1)

## Revisione di gruppi e utenti

Durante la configurazione del sistema [!UICONTROL Workfront DAM] è importante considerare il ruolo che gli utenti e i gruppi svolgono nel quadro generale.

I gruppi controllano l’accesso alle cartelle delle risorse in [!UICONTROL Workfront DAM]. Le impostazioni del gruppo controllano anche le operazioni che gli utenti possono eseguire con le risorse (visualizzazione, download, modifica, ecc.) a cui dispongono dell’autorizzazione di accesso.

Durante la creazione di gruppi, è fondamentale tenere presente a quali cartelle di risorse i membri di un gruppo avranno necessità di accedere in [!UICONTROL Workfront DAM].

Gli utenti sono le persone che hanno effettuato l’accesso a [!UICONTROL Workfront DAM]. Un utente non può accedere a nessuna funzione di [!UICONTROL Workfront DAM], a meno che non sia stato assegnato a un gruppo. Gli utenti possono appartenere a più gruppi, a seconda delle loro esigenze.

## Gruppi predefiniti

In [!UICONTROL Workfront DAM] sono disponibili due gruppi predefiniti. Tutti gli utenti appartengono automaticamente a questi gruppi, a condizione che dispongano delle credenziali di accesso a [!UICONTROL Workfront DAM]. Non è possibile aggiungere o rimuovere utenti da questi gruppi:

* **Gruppo ospiti:** utilizzato per controllare l’accesso di un utente anonimo. Potrebbe trattarsi di un utente senza credenziali di accesso o di un utente non attualmente connesso.
* **Gruppo con accesso:** tutti gli utenti che hanno effettuato l’accesso appartengono a questo gruppo.

Per impostazione predefinita, esistono anche il gruppo Amministratore e le relative impostazioni. È possibile aggiungere utenti a questo gruppo, ma non modificarne le impostazioni.

## Tipi di ruolo

Man mano che i gruppi vengono creati, viene loro assegnato un tipo di ruolo. Il tipo di ruolo determina quale parte del sistema [!UICONTROL Workfront DAM] ottengono gli utenti al momento della connessione: [!UICONTROL Workfront DAM] o [!UICONTROL Brand Connect].

Le licenze [!UICONTROL Workfront DAM] prevedono tre tipi di ruolo:

* **[!UICONTROL Brand Portal:]** questi utenti hanno accesso solo a [!UICONTROL Brand Connect], che consente loro di visualizzare e scaricare le risorse approvate.
* **[!UICONTROL Collaboratore:]** questi utenti possono accedere a [!UICONTROL Workfront DAM] e a [!UICONTROL  Brand Connect]. Possiedono i diritti di accesso completo alle risorse e alle cartelle, ossia visualizzarle, scaricarle, caricarle, modificarle, spostarle ed eliminarle.
* **[!UICONTROL Amministratore:]** gli amministratori di sistema hanno accesso a tutte le funzioni di [!UICONTROL Brand Connect] e [!UICONTROL Workfront DAM], oltre ad avere la possibilità di stabilire le impostazioni di sistema globali per ciascuno di essi. Inoltre, possono accedere alle risorse scadute o impostate come inattive.

<!-- 
Learn more graphic & documentation article link, below
* Understanding the difference between Workfront licenses and Workfront DAM role types
* -->
