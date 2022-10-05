---
title: Procedura dettagliata per i router
description: Scopri come utilizzare un router per passare i bundle Pokemon vs supereroi nel percorso corretto in [!DNL Adobe Workfront Fusion].
activity: use
doc-type: feature video
team: Technical Marketing
kt: 9013
exl-id: 6c111e5b-1c8f-43fd-9e2d-16599de2a337
source-git-commit: 82b0e8e5875f3cedd25446507b29a46c9d598d29
workflow-type: tm+mt
source-wordcount: '879'
ht-degree: 0%

---

# Procedura dettagliata dei router

## Panoramica

Utilizzare un router per passare i bundle Pokemon vs. supereroi nel percorso corretto, quindi creare un&#39;attività per ogni carattere.

![Immagine dello scenario di fusione](assets/universal-connectors-and-routing-2.png)

## Procedura dettagliata dei router

Workfront consiglia di guardare il video dettagliato sull&#39;esercizio prima di cercare di ricreare l&#39;esercizio nel proprio ambiente.

>[!VIDEO](https://video.tv.adobe.com/v/335272/?quality=12)

## URL di esercizio

* Sito web API supereroe: https://www.superheroapi.com/
* Primo URL per l’esercizio: https://www.superheroapi.com/api/{access-token}/{character-id}/aspect
* Secondo URL per l’esercizio: https://www.superheroapi.com/api/{access-token}/{character-id}/powerstats

Se hai problemi ad accedere al tuo token supereroe, puoi usare questo token condiviso: 10110256647253588. Presta attenzione a quante volte chiami l’API del supereroe in modo che questo token condiviso continui a funzionare per tutti.

>[!TIP]
>
>Per istruzioni dettagliate su come completare la procedura dettagliata, consulta [Procedura dettagliata dei router](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/routers.html?lang=en) esercizio fisico.


## Cercare elementi nel pannello di mappatura

Il campo Cerca elementi nella parte superiore dei pannelli di mappatura consente di trovare rapidamente i campi nel pannello, anche se nidificati in array. La ricerca non distingue tra maiuscole e minuscole.

![Immagine del primo pannello di ricerca](assets/universal-connectors-and-routing-3.png)

![Immagine del secondo pannello di ricerca](assets/universal-connectors-and-routing-4.png)

## Suggerimenti per lavorare con le API

Finora hai lavorato con un’API molto semplice (Application Programming Interface) che non richiede un’autenticazione aggiuntiva per estrarre le informazioni necessarie nello scenario. Di seguito sono riportati alcuni suggerimenti per aiutarti a navigare utilizzando le API e i connettori universali.

## Passaggio 1: Determinare il tipo di API

Workfront e molti sistemi software vengono creati utilizzando un’API REST (Rappresentational State Transfer), il tipo di API più semplice e standard attualmente disponibile. Tuttavia, ce ne sono alcuni altri, come:

* SOAP (Simple Object Access Protocol) (l’API di prova di Workfront è basata su SOAP)
* FTP (File Transfer Protocol)
* SFTP (Secure File Transfer Protocol)
* Per ulteriori informazioni, effettua una ricerca web per tipi di API e parole chiave di interesse.

>[!NOTE]
>
>Quando ci si connette a piattaforme più grandi come Salesforce, diverse aree di tali piattaforme forniscono API diverse. Assicurati di trovare quello corretto per il servizio a cui desideri connetterti.

## Passaggio 2: Determinare il tipo di autenticazione richiesto dall’API

L&#39;autenticazione API è una forma di identificazione utilizzata per controllare l&#39;accesso a un servizio, ad esempio quando si tenta di connettersi tramite Workfront Fusion. Ti aiuta a dimostrare a un altro sistema che sei autorizzato ad accedere al sistema. OAuth 2 è il tipo di autenticazione più comune utilizzato oggi. Ulteriori informazioni con una ricerca su Internet sull’autenticazione API.

L’autenticazione può essere l’aspetto più difficile dell’utilizzo di un’API. Una delle caratteristiche più importanti dei connettori universali di Workfront Fusion è che Workfront Fusion è in grado di gestire l’autenticazione quando si utilizzano metodi di autenticazione comuni come l’autenticazione di base, come OAuth 2, la chiave API e altri. Una volta creata una connessione utilizzando il modulo Workfront Fusion appropriato per il metodo di autenticazione (ad esempio, OAuth 2), Workfront Fusion genererà continuamente chiavi API e/o token ogni volta che si desidera eseguire lo scenario.

Scopri i diversi tipi di autenticazione forniti da Workfront nell’articolo Panoramica sull’autenticazione avanzata di Experience League.

## Passaggio 3: Leggi la documentazione API e trova gli endpoint necessari

Quando un’API interagisce con un altro sistema, i punti di contatto di questa comunicazione sono considerati endpoint. Un endpoint è il luogo in cui le API inviano le richieste e in cui risiede la risorsa.

Quando interagisci con un’API utilizzando un connettore universale, è necessario comprendere gli endpoint supportati dall’API e i dati richiesti per ogni richiesta. La documentazione API descrive gli endpoint di un’API e come eseguire operazioni comuni come creare, leggere, aggiornare o eliminare elementi. L’esecuzione di queste chiamate richiede una certa pratica, soprattutto se hai poca esperienza nell’effettuare chiamate API o lavorare con una nuova API.

Scopri di più sui connettori universali di Workfront Fusion e come configurarli per connettersi alle API necessarie in Experience League.

## Nota finale

Puoi controllare l’intero elenco dei connettori app predefiniti nell’Experience League. Se desideri suggerire un nuovo connettore app al team di prodotto Workfront Fusion, invia la tua idea a Innovation Lab. Se non hai ancora inoltrato la tua richiesta, scopri di più sul Innovation Lab e su come votare le idee e partecipare alla definizione delle priorità della classifica due volte all’anno. Se hai già accesso a Innovation lab, accedi e invia le tue idee.

## Il tuo turno

Questo esercizio si basa su ciò che hai appreso nella procedura dettagliata, ma la soluzione non viene fornita.

Nel modulo Imposta variabili multiple per i caratteri Pokemon, crea una variabile chiamata &quot;Stat (Level)&quot;. Mappa il nome delle statistiche Pokemon in questa variabile. Utilizzare la funzionalità valore array per modificare la modalità di visualizzazione dell&#39;array, in modo che ogni stato sia una nuova riga come mostrato di seguito.

**Suggerimento:** Ci sono solo sei statistiche Pokemon diverse con un livello corrispondente.

![Immagine delle statistiche](assets/universal-connectors-and-routing-5.png)

**Sfida:** Verificare se è possibile utilizzare le formule di array per ottenere la possibilità di visualizzare la stessa modalità di cui sopra come righe diverse anziché come una stringa di valori separati da una virgola. C&#39;è un suggerimento nella schermata seguente.

![Immagine di un nome di matrice](assets/universal-connectors-and-routing-6.png)

## Vuoi saperne di più? Si consiglia quanto segue:

[Documentazione di Workfront Fusion](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
