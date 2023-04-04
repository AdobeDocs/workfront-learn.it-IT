---
title: Comprendere le esecuzioni incomplete
description: Scopri cosa sono le esecuzioni incomplete e come gestire un errore che si traduce in un’esecuzione incompleta in [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 9066
exl-id: 3b7bf669-4736-4ba5-bcec-0d3fe0b2ce74
doc-type: video
source-git-commit: 650e4d346e1792863930dcebafacab4c88f2a8bc
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---

# Comprendere le esecuzioni incomplete

Le esecuzioni incomplete possono essere archiviate in Workfront Fusion, dove possono essere successivamente riviste e risolte. Scopri come sfruttare questa straordinaria funzionalità.

In questo video imparerai:

* Quali esecuzioni incomplete sono
* Come gestire un errore che si traduce in un&#39;esecuzione incompleta

>[!VIDEO](https://video.tv.adobe.com/v/335307/?quality=12&learn=on)

## Errori che determinano esecuzioni incomplete

Ci sono diverse categorie di errori che portano alla memorizzazione di esecuzioni incomplete.

I diversi tipi di errore ricevuti dipenderanno dalle API a cui ti stai connettendo. L&#39;errore potrebbe essere un errore di convalida derivante da dati incompleti o errati, principalmente a causa di un elemento mancante che è previsto per elaborare correttamente tutti i dati che attraversano un modulo. Oppure gli errori possono verificarsi a causa dell’indisponibilità della destinazione finale a causa di un errore temporaneo o a lungo termine di connessione (ad esempio durante la connessione a un server FTP remoto o via e-mail).

Se si verifica un errore sul primo modulo dello scenario, l&#39;esecuzione si arresta immediatamente e non viene memorizzata alcuna esecuzione incompleta.

Se si verifica un errore su qualsiasi altro modulo e non è collegata alcuna route del gestore di errori, allora:

* Se il tipo di errore è ConnectionError, RateLimitError, OutOfSpaceError o ModuleTimeoutError, viene memorizzato un record di esecuzione incompleto CON esecuzione automatica del nuovo tentativo.
* Se il tipo di errore è DataError, InvalidConfigurationError, InvalidAccessTokenError, UnexpectedError, MaxFileSizeExceeedError o MaxResultsExceeedError, viene memorizzato un record di esecuzione incompleto SENZA esecuzione di un nuovo tentativo automatico.
* Se il tipo di errore è diverso da quanto indicato sopra, l’esecuzione non riesce.

## Vuoi saperne di più? Si consiglia quanto segue:

[Documentazione di Workfront Fusion](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
