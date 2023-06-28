---
title: Procedura dettagliata sui webhook
description: Scopri come utilizzare un webhook per creare un’app per determinare se un cliente è abbastanza grande per acquistare alcool, il tutto in [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9051
exl-id: 7870c9db-d538-440a-8972-e7bc5ac5af93
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '371'
ht-degree: 0%

---

# Procedura dettagliata sui webhook

Questo scenario crea un&#39;app per un negozio di generi alimentari in modo che possano facilmente determinare se un cliente è abbastanza grande per acquistare alcol. Il cassiere deve semplicemente pubblicare il nome e la data di nascita del cliente E un token client verificato in un URL fornito. Una volta inserito, questo attiverà il nostro scenario per calcolare la risposta appropriata e restituirla al richiedente.

![Un&#39;immagine che utilizza il modulo switch](assets/beyond-basic-modules-5.png)

## Procedura dettagliata sui webhook

Workfront consiglia di guardare il video con procedura dettagliata dell’esercizio prima di tentare di ricrearlo nel tuo ambiente.

>[!VIDEO](https://video.tv.adobe.com/v/335292/?quality=12&learn=on)

>[!TIP]
>
>Per istruzioni dettagliate sul completamento della procedura dettagliata, vedere [Procedura dettagliata sui webhook](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/webhooks.html?lang=en) esercizio fisico.

## Configurazione Postman

Per seguire insieme all&#39;esercizio di procedura dettagliata, è necessario scaricare l&#39;applicazione Postman gratuita. Per accedere all&#39;area destra di Postman per l&#39;esercizio, eseguire la procedura seguente.

1. Crea un’area di lavoro, quindi aprila.
1. Fai clic sulla scheda Nuovo e crea una nuova raccolta denominata Età potabile.
1. Fai di nuovo clic sulla scheda Nuovo e crea una nuova richiesta GET denominata GET data di nascita.
1. Modifica l’azione di richiesta da GET a POST.
1. Passa all’area della scheda secondaria Corpo sotto il campo URL POST.
1. Scegliere i dati del modulo sotto la scheda secondaria Autorizzazione.
1. Crea tre chiavi per Nome, Data di nascita e clientToken.

![Un&#39;immagine che utilizza il modulo switch](assets/beyond-basic-modules-6.png)

## Tocca a te

>[!NOTE]
>
>Gli esercizi pratici e le sfide sono facoltativi e non sono necessari per completare la formazione su Fusion.

Questo esercizio di esercitazione si basa su quanto appreso nella procedura dettagliata, ma la soluzione non viene fornita.

Crea un webhook di Workfront in attesa di nuovi aggiornamenti creati e quindi registra la data, il nome della persona che ha effettuato l’aggiornamento e ciò che dice l’aggiornamento. Invia a te stesso queste informazioni tramite e-mail.

**Suggerimento**: utilizza il modulo di attivazione degli eventi Workfront Watch per creare il webhook. Inoltre, in Workfront gli aggiornamenti sono denominati note.

**Sfida**: per accedervi facilmente, è possibile trovare e aggiungere l’URL per il punto in cui è stato effettuato l’aggiornamento?


## Vuoi saperne di più? Consigliamo quanto segue:

[Documentazione di Workfront Fusion](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
