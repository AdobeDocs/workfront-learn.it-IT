---
title: Procedura dettagliata sui router
description: Scopri come utilizzare un router per trasferire i bundle Pokemon e supereroi lungo il percorso corretto in  [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9013
exl-id: 6c111e5b-1c8f-43fd-9e2d-16599de2a337
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: ht
source-wordcount: '878'
ht-degree: 100%

---

# Procedura dettagliata sui router

Utilizza un router per passare i bundle Pokemon e supereroi lungo il percorso corretto, quindi crea un’attività per ogni carattere.

![Immagine dello scenario Fusion](assets/universal-connectors-and-routing-2.png)

## Procedura dettagliata sui router

Workfront consiglia di guardare il video della procedura dettagliata relativa all’esercizio, prima di provare a ricrearlo nel proprio ambiente.

>[!VIDEO](https://video.tv.adobe.com/v/335272/?quality=12&learn=on)

## URL di esercizio

* Sito Web API di Superhero: `https://www.superheroapi.com/`
* Primo URL per l’esercizio: `https://www.superheroapi.com/api/{access-token}/{character-id}/appearance`
* Secondo URL per l’esercizio: `https://www.superheroapi.com/api/{access-token}/{character-id}/powerstats`

Se hai problemi ad accedere al tuo token di supereroe, puoi utilizzare questo token condiviso: 10110256647253588. Tieni in considerazione quante volte richiami l’API supereroe in modo che questo token condiviso continui a funzionare per tutti.

>[!TIP]
>
>Per istruzioni dettagliate sul completamento della procedura dettagliata, vai all’esercizio [Procedura dettagliata sui router](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/routers.html?lang=it).


## Cerca elementi nel pannello di mappatura

Il campo Cerca elementi nella parte superiore dei pannelli di mappatura ti aiuta a trovare rapidamente i campi nel pannello, anche se sono nidificati in array. La ricerca non distingue tra maiuscole e minuscole.

![Immagine del primo pannello di ricerca](assets/universal-connectors-and-routing-3.png)

![Immagine del secondo pannello di ricerca](assets/universal-connectors-and-routing-4.png)

## Suggerimenti per lavorare con le API

Fino a questo punto, hai lavorato con un’API (Application Programming Interface) molto semplice che non richiede alcuna autenticazione aggiuntiva per ottenere le informazioni necessarie nello scenario. Di seguito sono riportati alcuni suggerimenti per aiutarti a lavorare con le API e i connettori universali.

## Passaggio 1: determinare il tipo di API

Workfront e molti sistemi software sono creati utilizzando un’API REST (Representative State Transfer), il tipo di API più semplice e standard oggi disponibile. Tuttavia, ce ne sono altre, come:

* SOAP (Simple Object Access Protocol) (l’API di Workfront Proof è basata su SOAP)
* FTP (File Transfer Protocol)
* SFTP (Secure File Transfer Protocol)
* Per ulteriori informazioni, esegui una ricerca web per tipi di API e parole chiave di interesse.

>[!NOTE]
>
>Quando ci si connette a piattaforme più grandi come Salesforce, diverse aree di tali piattaforme forniscono API diverse. Assicurati di trovare quella corretta per il servizio a cui desideri connetterti.

## Passaggio 2: determinare il tipo di autenticazione richiesta dall’API

L’autenticazione API è una forma di identificazione utilizzata per controllare l’accesso a un servizio, ad esempio quando si tenta di connettersi tramite Workfront Fusion. Consente di provare a un altro sistema che si è autorizzati ad accedere al sistema. OAuth 2 è il tipo di autenticazione più comune utilizzato oggi. Per saperne di più, consulta la ricerca Internet sull’autenticazione API.

L’autenticazione può essere l’aspetto più difficile dell’utilizzo di un’API. Una delle funzionalità più importanti dei connettori universali di Workfront Fusion è che Workfront Fusion può gestire l’autenticazione per te quando utilizzi metodi di autenticazione comuni, come l’autenticazione di base, ad esempio OAuth 2, API Key e altri. Una volta creata una connessione utilizzando il modulo Workfront Fusion appropriato per il metodo di autenticazione (ad esempio, OAuth 2), Workfront Fusion genera in modo continuo chiavi API e/o token ogni volta che desideri eseguire lo scenario.

Scopri i diversi tipi di autenticazione forniti da Workfront nell’articolo Panoramica dell’autenticazione avanzata su Experience League.

## Passaggio 3: leggi la documentazione API e trova gli endpoint necessari

Quando un’API interagisce con un altro sistema, i punti di contatto di questa comunicazione sono considerati endpoint. Un endpoint è il luogo in cui le API inviano richieste e in cui si trova la risorsa.

Quando interagisci con un’API utilizzando un connettore universale, devi comprendere quali endpoint supporta l’API e quali dati sono richiesti per ciascuna richiesta. La documentazione API descrive gli endpoint di un’API e come eseguire operazioni comuni come creare, leggere, aggiornare o eliminare. L’esecuzione di queste chiamate richiede alcune esercitazioni, soprattutto se non hai familiarità con l’esecuzione di chiamate API o con l’utilizzo di una nuova API.

Scopri di più sui connettori universali di Workfront Fusion e come configurarli per connettersi alle API necessarie su Experience League.

## Nota finale

Consulta l’intero elenco dei connettori di app predefiniti, in Experience League. Se desideri suggerire un nuovo connettore di app al team di prodotto Workfront Fusion, invia la tua idea a Innovation Lab. Se non hai ancora inviato alcun suggerimento, scopri di più su Innovation Lab, su come votare le idee proposte e come partecipare alla definizione delle priorità della classifica due volte all’anno. Se hai già accesso a Innovation Lab, accedi e invia le tue idee.

## Tocca a te

>[!NOTE]
>
>Gli esercizi pratici e le sfide sono facoltativi e non necessari per completare la formazione su Fusion.

Questa esercitazione si basa su quanto appreso nella procedura dettagliata, ma è priva di soluzione.

Nel modulo Set multiple variables (Imposta più variabili) per i personaggi Pokemon, crea una variabile denominata “Stat (Level)”. Mappa il nome delle statistiche Pokemon in questa variabile. Utilizza la funzionalità del valore array per modificare la visualizzazione dell’array, in modo che ogni variabile Stat sia su una nuova riga, come illustrato di seguito.

**Suggerimento:** ci sono solo sei diverse statistiche Pokemon con un livello corrispondente.

![Immagine delle variabili Stat](assets/universal-connectors-and-routing-5.png)

**Sfida:** prova a utilizzare le formule per array in modo da visualizzare le Abilità come riportato sopra, come righe diverse anziché come una stringa di valori separati da una virgola. Trovi un suggerimento nella schermata di seguito.

![Immagine di un nome di array](assets/universal-connectors-and-routing-6.png)

## Desideri ulteriori informazioni? Consigliamo quanto segue:

[Documentazione di Workfront Fusion](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=it)
