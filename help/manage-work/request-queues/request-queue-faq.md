---
title: Risposte alle domande comuni sulle code di richieste
description: Risposte alle domande comuni sulle code di richieste in [!DNL  Workfront].
feature: Work Management
type: Tutorial
role: Admin, User
level: Beginner, Intermediate
last-substantial-update: 2023-07-18T00:00:00Z
jira: KT-10101
exl-id: bfa3ae5f-9618-444c-9eb8-5d82db9a77c7
source-git-commit: ce2aad1cd0ecb7d568ed9a01d97147cbd126ca05
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 0%

---

# Domande comuni sulle code di richieste

**Perché è possibile visualizzare una coda di richieste, ma l&#39;utente non è in grado di visualizzarle?**

In [!UICONTROL Dettagli coda] della coda/del progetto della richiesta, verificare che l&#39;utente soddisfi i criteri del messaggio &quot;Chi può aggiungere richieste a questa coda?&quot; campo.

**Ho dato agli utenti l’accesso alla coda, ma ora possono anche vedere il progetto della coda richieste. Perché?**

Ciò ha a che fare con il modo in cui hai dato loro l’accesso alla coda delle richieste.

Se è stato utilizzato il [!UICONTROL Condivisione] dalla pagina di destinazione del progetto della coda richieste, hai dato a tali utenti l’accesso per visualizzare il progetto nell’elenco dei progetti.

Tuttavia, se desideri consentire loro di accedere solo per inviare una richiesta alla coda, passa a Configurazione coda e seleziona l’opzione appropriata in &quot;Chi può aggiungere richieste a questo progetto&quot;.

**Posso trasformare una richiesta in un progetto?**

Sì. Puoi convertire i problemi in attività o progetti a seconda di ciò che è necessario.

Consulta questo articolo per ulteriori informazioni: [Converti i problemi](https://experienceleague.adobe.com/docs/workfront/using/manage-work/issues/convert-issues/convert-issues-overview.html?lang=en).

**Dove si trova una coda di richieste per apportare modifiche?**

È possibile utilizzare [!UICONTROL Ricerca] nella barra di navigazione o trovarlo elencato nella [!UICONTROL Progetti] area.

Se apri una richiesta dalla coda di richieste, puoi fare clic sul nome del progetto nell’area delle breadcrumb.

**Posso trasferire le informazioni da un modulo personalizzato di richiesta a un modulo personalizzato di progetto?**

Sì. Quando crei un modulo personalizzato, seleziona entrambi [!UICONTROL Progetto] e [!UICONTROL Problema] come tipi di oggetto. Allega il modulo personalizzato alla richiesta. Quando si converte la richiesta in un progetto, il modulo personalizzato viene automaticamente allegato al nuovo progetto e i valori contenuti in qualsiasi campo vengono visualizzati sia nella richiesta che nel modulo personalizzato del progetto.

**Visualizzazione di un report di progetto o attività. Come posso trovare la richiesta da cui ha avuto origine questo oggetto?**

Puoi accedere ai campi nella sezione **[!UICONTROL Problema convertito]** e **[!UICONTROL Iniziatore problema convertito]** origini dei campi per aggiungere tali informazioni ai report di progetto e attività.

**Qual è il modo migliore per filtrare le code di richieste in un rapporto?**

Se il filtro del progetto include **Coda>>È pubblico>>Uguale a>>Nessuno** il report mostrerà solo i progetti che sono **NOT** code di richieste.

Se il filtro del progetto include **Queue>>È pubblico>>Non uguale a>>Nessuno** il report mostrerà solo i progetti che **SONO** code di richieste.
