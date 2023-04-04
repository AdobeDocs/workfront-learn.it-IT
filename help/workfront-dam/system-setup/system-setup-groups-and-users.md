---
title: Comprendere i gruppi e gli utenti in [!UICONTROL Workfront DAM]
description: Scopri come creare cartelle, gruppi e utenti in [!UICONTROL Workfront DAM]. Comprendere i tipi di ruolo utente e concedere autorizzazioni alle cartelle.
activity: use
feature: Digital Content and Documents
type: Tutorial
role: Admin
level: Intermediate
team: Technical Marketing
kt: 8967
exl-id: 4ebf675c-b72d-447e-b131-a89acb449e15
doc-type: video
source-git-commit: 650e4d346e1792863930dcebafacab4c88f2a8bc
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# Configurazione del sistema: gruppi e utenti

Questo video illustra come:

* Comprendere in che modo le impostazioni del gruppo influiscono sull’accesso alle risorse
* Creare cartelle, gruppi e utenti in un ordine specifico
* Comprendere i tipi di ruolo utente
* Concedere autorizzazioni alle cartelle
* Creare e modificare gruppi
* Aggiungere e modificare gli utenti

>[!VIDEO](https://video.tv.adobe.com/v/335230/?quality=12&learn=on)

## Revisione di gruppi e utenti

Quando configuri [!UICONTROL Workfront DAM] è importante considerare i ruoli che gli utenti e i gruppi svolgono nel quadro generale.

I gruppi controllano l’accesso alle cartelle di risorse in [!UICONTROL Workfront DAM]. Le impostazioni del gruppo controllano anche le operazioni che gli utenti possono eseguire con le risorse (visualizzazione, download, modifica, ecc.) hanno il permesso di accedere.

Durante la creazione di gruppi, è fondamentale tenere presente a quali cartelle di risorse i membri di quel gruppo avranno bisogno di accedere in [!UICONTROL Workfront DAM].

Gli utenti sono gli utenti che hanno accesso a [!UICONTROL Workfront DAM]. Un utente non può accedere a nulla in [!UICONTROL Workfront DAM] a meno che non siano assegnati a un gruppo. Gli utenti possono appartenere a più gruppi, a seconda delle loro esigenze.

## Gruppi predefiniti

Sono disponibili due gruppi predefiniti [!UICONTROL Workfront DAM]. Tutti gli utenti appartengono automaticamente a questi gruppi, a seconda che abbiano o meno [!UICONTROL Workfront DAM] credenziali di accesso. Non è possibile aggiungere o rimuovere utenti dai gruppi seguenti:

* **Gruppo di ospiti**- Utilizzato per controllare l&#39;accesso di un utente anonimo. Potrebbe trattarsi di un utente senza credenziali di accesso o che al momento non ha effettuato l&#39;accesso.
* **Registrato**-In gruppo - Tutti gli utenti che hanno effettuato l&#39;accesso appartengono a questo gruppo.

Per impostazione predefinita esistono anche il gruppo Amministratore e le relative impostazioni. È possibile aggiungere utenti a questo gruppo ma non è possibile modificare le impostazioni.

## Tipi di ruolo

Al momento della creazione dei gruppi, gli viene assegnato un tipo di ruolo. Il tipo di ruolo determina la parte del [!UICONTROL Workfront DAM] gli utenti del sistema ottengono quando effettuano l&#39;accesso — [!UICONTROL Workfront DAM] o [!UICONTROL Brand Connect].

Sono disponibili tre tipi di ruolo con [!UICONTROL Workfront DAM] licenze:

* **[!UICONTROL Brand Portal]**—Questi utenti hanno accesso solo a [!UICONTROL Brand Connect], che è il luogo in cui possono visualizzare e scaricare le risorse approvate.
* **[!UICONTROL Collaboratore]**—Questi utenti possono accedere a [!UICONTROL Workfront DAM] e [!UICONTROL Brand Connect]. Hanno diritti di accesso completi a risorse e cartelle: visualizza, scarica, carica, modifica, sposta ed elimina.
* **[!UICONTROL Amministratore]**- Gli amministratori di sistema possono accedere a tutto ciò che è [!UICONTROL Brand Connect] e [!UICONTROL Workfront DAM], oltre alla possibilità di definire le impostazioni di sistema globali per ciascuna di esse. Possono inoltre accedere alle risorse scadute o impostate come inattive.

<!-- 
Learn more graphic & documentation article link, below
* Understanding the difference between Workfront licenses and Workfront DAM role types
* -->
