---
title: Procedura dettagliata sui webhook
description: Scopri come utilizzare un webhook per creare un’app per determinare se un cliente è abbastanza grande o meno per acquistare alcol, il tutto in [!DNL Adobe Workfront Fusion].
activity: use
doc-type: feature video
team: Technical Marketing
kt: Jira ticket
exl-id: 7870c9db-d538-440a-8972-e7bc5ac5af93
source-git-commit: 1f7a4da813805691fc0e52d3ad1ea708f9e07a9a
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 0%

---

# Procedura dettagliata sui webhook

## Panoramica

Questo scenario crea un&#39;app per comodità in modo che possano facilmente determinare se un cliente è abbastanza grande o meno per acquistare alcol. Il cassiere deve semplicemente pubblicare il nome e la data di nascita del cliente E un token client verificato a un URL fornito. Una volta inserito, questo attiverà il nostro scenario per calcolare la risposta appropriata e restituirla al richiedente.

![Immagine che utilizza il modulo switch](assets/beyond-basic-modules-5.png)

## Procedura dettagliata sui webhook

Workfront consiglia di guardare il video dettagliato sull&#39;esercizio prima di cercare di ricreare l&#39;esercizio nel proprio ambiente.

>[!VIDEO](https://video.tv.adobe.com/v/335292/?quality=12)

>[!TIP]
>
>Per istruzioni dettagliate su come completare la procedura dettagliata, consulta [Procedura dettagliata sui webhook](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/webhooks.html?lang=en) esercizio fisico.

## Configurazione Postman

Per seguire insieme all&#39;esercizio dettagliata, è necessario scaricare l&#39;applicazione gratuita Postman. Segui i passaggi riportati di seguito per accedere all’area di destra di Postman per l’esercizio.

1. Crea un’area di lavoro, quindi aprila.
1. Fai clic sulla scheda Nuovo e crea una nuova raccolta denominata Età di bere.
1. Fai nuovamente clic sulla scheda Nuovo e crea una nuova richiesta di GET denominata Data di nascita GET.
1. Modifica l’azione di richiesta da GET a POST.
1. Passa all’area della sottoscheda Corpo sotto il campo URL di POST.
1. Scegliere i dati del modulo sotto la sottoscheda Autorizzazione.
1. Crea tre chiavi per Name, Birthdate e clientToken.

![Immagine che utilizza il modulo switch](assets/beyond-basic-modules-6.png)

## Il tuo turno

Questo esercizio si basa su ciò che hai appreso nella procedura dettagliata, ma la soluzione non viene fornita.

Crea un webhook di Workfront in attesa di nuovi aggiornamenti creati e quindi registra la data, il nome della persona che ha effettuato l&#39;aggiornamento e ciò che viene indicato nell&#39;aggiornamento. Invia queste informazioni via e-mail.

**Suggerimento**: Utilizza il modulo trigger Workfront Watch Events per creare il tuo webhook. Inoltre, in Workfront gli aggiornamenti sono chiamati note.

**Sfida**: Puoi trovare e aggiungere l’URL per il punto in cui è stato effettuato l’aggiornamento per un facile accesso?


## Vuoi saperne di più? Si consiglia quanto segue:

[Documentazione di Workfront Fusion](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
