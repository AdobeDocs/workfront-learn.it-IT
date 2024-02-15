---
title: Risposte alle domande più comuni sulle code di richieste
description: Ottieni risposte alle domande più comuni sulle code di richieste in [!DNL  Workfront].
feature: Work Management
type: Tutorial
role: Admin, User
level: Beginner
last-substantial-update: 2023-07-18T00:00:00Z
jira: KT-10101
exl-id: bfa3ae5f-9618-444c-9eb8-5d82db9a77c7
source-git-commit: ec82cd0aafb89df7b3c46eb716faf3a25cd438a2
workflow-type: ht
source-wordcount: '406'
ht-degree: 100%

---

# Risposte alle domande più comuni sulle code di richieste

**Perché vedo una coda di richieste, ma il mio utente non la vede?**

Nella scheda [!UICONTROL Dettagli coda] della tua coda di richieste o nel tuo progetto, assicurati che l’utente soddisfi i criteri del campo “Chi può aggiungere richieste a questa coda?” .

**Ho concesso agli utenti l’accesso alla coda, ma ora possono vedere anche il progetto della coda delle richieste. Perché?**

Dipende dal modo in cui hai concesso loro l’accesso alla coda delle richieste.

Se hai utilizzato lo strumento [!UICONTROL Condivisione] dalla pagina di destinazione del progetto della coda delle richieste, allora hai concesso loro anche la possibilità di vedere il progetto nell’elenco dei progetti.

Se invece desideri concedere loro l’accesso solo per inviare una richiesta alla coda, vai su Configurazione coda e seleziona l’opzione appropriata in “Chi può aggiungere richieste a questo progetto?”.

**Posso trasformare una richiesta in un progetto?**

Sì. Puoi convertire i problemi in attività o progetti in base alle necessità.

per ulteriori informazioni, consulta questo articolo: [Convertire i problemi](https://experienceleague.adobe.com/docs/workfront/using/manage-work/issues/convert-issues/convert-issues-overview.html?lang=it).

**Dove trovo una coda di richieste per apportarvi modifiche?**

Puoi usare il campo [!UICONTROL Ricerca] nella barra di navigazione opure puoi trovarla elencata nell’area [!UICONTROL Progetti].

Se apri una richiesta dalla coda delle richieste puoi fare clic sul nome del progetto nell’area delle breadcrumb.

**Posso trasferire le informazioni da un modulo personalizzato di una richiesta a un modulo personalizzato di un progetto?**

Sì. Quando crei un modulo personalizzato, seleziona [!UICONTROL Progetto] e [!UICONTROL Problema] come tipi di oggetto. Allega il modulo personalizzato alla richiesta. Quando converti la richiesta in un progetto, il modulo personalizzato verrà automaticamente allegato al nuovo progetto e i valori contenuti in tutti i campi verranno visualizzati sia nella richiesta che nei moduli personalizzati del progetto.

**Sto guardando un progetto o un rapporto di attività. Come posso capire da quale richiesta proviene questo oggetto?**

Per aggiungere tali informazioni ai rapporti di progetto e attività, puoi accedere ai campi nelle origini campo **[!UICONTROL Problema convertito]** e il **[!UICONTROL Referente problema convertito]**.

**Qual è il modo migliore per filtrare le code di richieste in un rapporto?**

Se il filtro del progetto include **Coda>>È pubblico>>Uguale a>>Nessuno** il rapporto mostrerà solo i progetti che **NON** sono code di richieste.

Se il filtro del progetto include **Coda>>È pubblico>>Non uguale a>>Nessuno** il rapporto mostrerà solo i progetti che **SONO** code di richieste.
