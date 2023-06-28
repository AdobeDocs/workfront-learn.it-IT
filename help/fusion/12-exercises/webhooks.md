---
title: Webhook
description: Scopri come creare, attivare e gestire gli scenari avviati dal webhook.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11053
thumbnail: KT11053.png
exl-id: d6a62a26-a8ab-477c-a8f2-98f3b9ff5edf
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 0%

---

# Webhook

Scopri come creare, attivare e gestire gli scenari avviati dal webhook.

## Panoramica dell’esercizio

Lo scopo di questo scenario è quello di creare un&#39;app per vendere ai minimarket in modo che possano facilmente determinare se un cliente è abbastanza grande per acquistare alcool. Il cassiere deve semplicemente pubblicare il nome e la data di nascita del cliente sull’URL fornito. Il post attiverà lo scenario che calcolerà la risposta e la restituirà al richiedente.

1. Lo scenario è costituito da tre webhook.
1. Il modulo trigger è un webhook personalizzato che ascolta un post.
1. Quando riceve un post, lo invia a uno dei moduli successivi.
1. Il modulo successivo restituisce una risposta al richiedente.

   ![Webhook - Immagine 1](../12-exercises/assets/webhooks-walkthrough-1.png)

## Passaggi da seguire

**Imposta il webhook del trigger.**

1. Crea un nuovo scenario e denominalo &quot;Utilizzo dei webhook&quot;.
1. Per il trigger, aggiungi il modulo webhook personalizzato dall’app Webhook.
1. Fai clic su Aggiungi per creare un nuovo webhook.
1. Immetti il nome del webhook &quot;Drinking age app&quot;.
1. Lascia vuote le restrizioni IP, il che significa che chiunque può inviarvi dati.
1. Fai clic su Salva.


   ![Webhook - Immagine 2](../12-exercises/assets/webhooks-walkthrough-2.png)

1. Nel pannello di mappatura dei webhook è stato creato un URL per questo webhook specifico. Fai clic su &quot;Copia indirizzo negli Appunti&quot; per copiare tale URL.
1. Fare clic su OK.
1. Fare clic su Esegui una volta.
1. Utilizza l’URL in Postman per inviare un nome e una data di nascita al tuo webhook personalizzato. Per istruzioni sulla configurazione di Postman, vedere [Procedura dettagliata sui webhook](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/beyond-basic-modules/webhooks-walkthrough.html?lang=en) esercitazione.

   **Il pannello del modulo Webhooks deve essere simile al seguente:**

   ![Immagine 3 dei webhook](../12-exercises/assets/webhooks-walkthrough-3.png)

   **Il webhook si trova ora in uno stato in cui è in ascolto dei dati per determinare la struttura dei dati.**

1. Puoi definire la struttura dati del payload che prevedi di ottenere (le strutture dati verranno discusse in seguito). Se non definisci una struttura dati, Fusion la determinerà automaticamente quando il post viene inviato.
1. Sul lato Postman si desidera inviare all’URL copiato. Il post deve includere dati modulo di base. In questo esempio sono necessari tre campi: Name, Birthdate e clientToken.

   ![Immagine 4 dei webhook](../12-exercises/assets/webhooks-walkthrough-4.png)

1. Dopo aver fatto clic su Invia da Postman si dovrebbe ottenere un&#39;indicazione che il post è stato accettato.
1. Questo è il punto in cui lo scenario mostrerà che la struttura dati è stata determinata correttamente.
1. Per verificare che i dati siano stati ricevuti, aprire il controllo di esecuzione.

   ![Immagine 5 dei webhook](../12-exercises/assets/webhooks-walkthrough-5.png)

   **Imposta il routing per i token client.**

1. Aggiungere un router al modulo trigger.
1. Nel percorso superiore, aggiungi un modulo di risposta Webhook. Questo sarà il nostro percorso quando il token client non corrisponde.
1. Imposta lo stato su 401.
1. Imposta il corpo su {&quot;error&quot;: &quot;Impossibile autenticare la richiesta. Controlla il clientToken&quot;}.

   ![Immagine Webhook 6](../12-exercises/assets/webhooks-walkthrough-6.png)

1. Crea un filtro tra il router e il modulo di risposta Webhook. Denominalo &quot;Il token client non corrisponde&quot;.
1. Per la condizione, utilizza il campo clientToken del modulo trigger ed esegui un confronto numerico &quot;Not equal to&quot; con il numero 5121933.

   ![Immagine 7 dei webhook](../12-exercises/assets/webhooks-walkthrough-7.png)

1. Nel percorso inferiore, aggiungi un altro modulo di risposta Webhook. Questo sarà il nostro percorso per quando il token client non corrisponde.
1. Imposta lo stato su 200.
1. Durante la configurazione del corpo, utilizza le funzioni del pannello di mappatura per verificare se la persona ha 21 anni o più. Se lo sono, restituisci &quot;Sei abbastanza grande da bere!&quot;, altrimenti restituisci &quot;Sei sfortunato...&quot;

   ![Webhook - Immagine 9](../12-exercises/assets/webhooks-walkthrough-9.png)

1. Crea un filtro tra il router e il modulo di risposta Webhook nel percorso inferiore. Denominalo &quot;Il token client non corrisponde&quot;.
1. Per la condizione, utilizza il campo clientToken del modulo trigger ed esegui un confronto numerico &quot;Uguale a&quot; con il numero 5121933.


   ![Immagine 8 dei webhook](../12-exercises/assets/webhooks-walkthrough-8.png)

1. Fai clic sul pulsante Pianificazione in Esegui una volta per attivare lo scenario in modo che, ogni volta che verrà ricevuto un nuovo post, scenderà in entrambi i percorsi e genererà una risposta.
