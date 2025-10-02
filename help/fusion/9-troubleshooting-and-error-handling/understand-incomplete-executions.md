---
title: Comprendere le esecuzioni incomplete
description: Scopri cosa sono le esecuzioni incomplete e come gestire un errore che determina un’esecuzione incompleta in [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9066
exl-id: 3b7bf669-4736-4ba5-bcec-0d3fe0b2ce74
recommendations: noDisplay,catalog
doc-type: video
source-git-commit: bbdf99c6bc1be714077fd94fc3f8325394de36b3
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Comprendere le esecuzioni incomplete

Le esecuzioni incomplete possono essere archiviate in Workfront Fusion dove possono essere successivamente riviste e risolte. Scopri come sfruttare questa straordinaria funzione.

In questo video scoprirai:

* Cosa sono le esecuzioni incomplete
* Come gestire un errore che determina un’esecuzione incompleta

>[!VIDEO](https://video.tv.adobe.com/v/335307/?quality=12&learn=on&enablevpops=1)

## Errori che hanno dato luogo ad esecuzioni incomplete

Esistono diverse categorie di errori che determinano la memorizzazione di esecuzioni incomplete.

I diversi tipi di errore ricevuti dipenderanno dalle API a cui ti stai connettendo. L’errore potrebbe essere un errore di convalida derivante da dati incompleti o errati, principalmente a causa di un elemento mancante previsto per elaborare correttamente tutti i dati che passano attraverso un modulo. In alternativa, gli errori potrebbero verificarsi se la destinazione finale non è disponibile a causa di un errore di connessione temporaneo o a lungo termine (ad esempio durante la connessione a un server e-mail o FTP remoto).

Se si verifica un errore nel primo modulo dello scenario, l’esecuzione viene subito interrotta e non viene memorizzata alcuna esecuzione incompleta.

Se si verifica un errore in un altro modulo e non è allegato alcun indirizzamento del gestore degli errori:

* Se il tipo di errore è ConnectionError, RateLimitError, OutOfSpaceError o ModuleTimeoutError, viene memorizzato un record di esecuzione incompleto CON nuovo tentativo automatico.
* Se il tipo di errore è DataError, InvalidConfigurationError, InvalidAccessTokenError, UnexpectedError, MaxFileSizeExceededError o MaxResultsExceededError, viene memorizzato un record di esecuzione incompleto SENZA nuovo tentativo automatico.
* Se il tipo di errore è diverso da quelli riportati sopra, l’esecuzione non riesce.

## Desideri ulteriori informazioni? Consigliamo quanto segue:

[Documentazione di Workfront Fusion](https://experienceleague.adobe.com/it/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)
