---
title: Comprendere le esecuzioni incomplete
description: Scopri cosa sono le esecuzioni incomplete e come gestire un errore che determina un’esecuzione incompleta in [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 9066
exl-id: 3b7bf669-4736-4ba5-bcec-0d3fe0b2ce74
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---

# Comprendere le esecuzioni incomplete

Le esecuzioni incomplete possono essere archiviate in Workfront Fusion dove possono essere successivamente esaminate e risolte. Scopri come sfruttare questa straordinaria funzione.

Questo video illustra:

* Cosa sono le esecuzioni incomplete
* Come gestire un errore che determina un’esecuzione incompleta

>[!VIDEO](https://video.tv.adobe.com/v/335307/?quality=12)

## Errori che hanno dato luogo ad esecuzioni incomplete

Esistono diverse categorie di errori che determinano la memorizzazione di esecuzioni incomplete.

I diversi tipi di errore ricevuti dipendono dalle API a cui ti stai connettendo. L’errore potrebbe essere dovuto a errori di convalida derivanti da dati incompleti o errati, principalmente a causa di un elemento mancante previsto per elaborare correttamente tutti i dati che passano attraverso un modulo. In alternativa, gli errori potrebbero verificarsi a causa dell’indisponibilità della destinazione finale a causa di un errore di connessione temporaneo o a lungo termine (ad esempio durante la connessione a un server e-mail o FTP remoto).

Se si verifica un errore nel primo modulo dello scenario, l’esecuzione viene interrotta immediatamente e non viene memorizzata alcuna esecuzione incompleta.

Se si verifica un errore in un altro modulo e non è collegata alcuna route del gestore degli errori, procedere come segue:

* Se il tipo di errore è ConnectionError, RateLimitError, OutOfSpaceError o ModuleTimeoutError, viene memorizzato un record di esecuzione incompleto WITH auto-retry.
* Se il tipo di errore è DataError, InvalidConfigurationError, InvalidAccessTokenError, UnexpectedError, MaxFileSizeExceededError o MaxResultsExceededError, viene memorizzato un record di esecuzione incompleto SENZA un nuovo tentativo automatico.
* Se il tipo di errore è diverso da quello riportato sopra, l’esecuzione non riesce.

## Vuoi saperne di più? Consigliamo quanto segue:

[Documentazione di Workfront Fusion](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
