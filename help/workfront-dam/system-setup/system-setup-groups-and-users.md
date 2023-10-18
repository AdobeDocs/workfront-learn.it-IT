---
title: Configurare gruppi e utenti
description: Scopri come creare cartelle, gruppi e utenti in [!UICONTROL DAM WORKFRONT]. Comprendere i tipi di ruolo utente e concedere autorizzazioni alle cartelle.
activity: use
feature: Digital Content and Documents
type: Tutorial
role: Admin
level: Intermediate
team: Technical Marketing
jira: KT-8967
exl-id: 4ebf675c-b72d-447e-b131-a89acb449e15
doc-type: video
source-git-commit: 6c31f8d2e98ad8cd1880cd03ec0b0e6c0fd9ec09
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 0%

---

# Configurare gruppi e utenti

Questo video illustra come:

* Comprendere come le impostazioni di gruppo influiscono sull’accesso alle risorse
* Creare cartelle, gruppi e utenti in un ordine specifico
* Comprendere i tipi di ruolo utente
* Concedere autorizzazioni alle cartelle
* Creare e modificare i gruppi
* Aggiungere e modificare gli utenti

>[!VIDEO](https://video.tv.adobe.com/v/335230/?quality=12&learn=on)

## Revisione di gruppi e utenti

Durante la configurazione [!UICONTROL DAM WORKFRONT] è importante considerare il ruolo degli utenti e dei gruppi nel quadro generale.

I gruppi controllano l’accesso alle cartelle di risorse in [!UICONTROL DAM WORKFRONT]. Le impostazioni del gruppo controllano anche le operazioni che gli utenti possono eseguire con le risorse (visualizzazione, download, modifica, ecc.) hanno l&#39;autorizzazione di accesso.

Durante la creazione di gruppi, è fondamentale tenere presente le cartelle di risorse a cui i membri di quel gruppo dovranno accedere in [!UICONTROL DAM WORKFRONT].

Gli utenti sono gli utenti che hanno effettuato l’accesso a [!UICONTROL DAM WORKFRONT]. Un utente non può accedere a nulla in [!UICONTROL DAM WORKFRONT] a meno che non siano assegnati a un gruppo. Gli utenti possono appartenere a più gruppi, a seconda delle loro esigenze.

## Gruppi predefiniti

Esistono due gruppi predefiniti forniti con [!UICONTROL DAM WORKFRONT]. Tutti gli utenti appartengono automaticamente a questi gruppi, a seconda che abbiano [!UICONTROL DAM WORKFRONT] credenziali di accesso. Non è possibile aggiungere o rimuovere utenti da questi gruppi:

* **Gruppo ospite**- Utilizzato per controllare l&#39;accesso per un utente anonimo. Potrebbe trattarsi di un utente senza credenziali di accesso o di un utente non attualmente connesso.
* **Accesso effettuato**-In gruppo—Tutti gli utenti che hanno eseguito l&#39;accesso appartengono a questo gruppo.

Per impostazione predefinita, esistono anche il gruppo Amministratore e le relative impostazioni. È possibile aggiungere utenti a questo gruppo, ma non modificare le impostazioni.

## Tipi di ruolo

Man mano che i gruppi vengono creati, viene loro assegnato un tipo di ruolo. Il tipo di ruolo determina quale parte del [!UICONTROL DAM WORKFRONT] gli utenti del sistema ricevono all&#39;accesso — [!UICONTROL DAM WORKFRONT] stesso o [!UICONTROL Brand Connect].

Sono disponibili tre tipi di ruolo con [!UICONTROL DAM WORKFRONT] licenze:

* **[!UICONTROL Brand Portal]**- Questi utenti hanno accesso solo a [!UICONTROL Brand Connect], che consente loro di visualizzare e scaricare le risorse approvate.
* **[!UICONTROL Collaboratore]**: questi utenti possono accedere a [!UICONTROL DAM WORKFRONT] e [!UICONTROL Brand Connect]. Possiedono i diritti di accesso completo alle risorse e alle cartelle, ossia visualizzarle, scaricarle, caricarle, modificarle, spostarle ed eliminarle.
* **[!UICONTROL Amministratore]**: gli amministratori di sistema hanno accesso a tutte le funzioni di [!UICONTROL Brand Connect] e [!UICONTROL DAM WORKFRONT], oltre alla possibilità di stabilire le impostazioni di sistema globali per ciascuno di essi. Inoltre, possono accedere alle risorse scadute o impostate come inattive.

<!-- 
Learn more graphic & documentation article link, below
* Understanding the difference between Workfront licenses and Workfront DAM role types
* -->
