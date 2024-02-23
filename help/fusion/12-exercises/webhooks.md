---
title: Esercizio sui webhook
description: Scopri come creare, attivare e gestire scenari avviati da webhook.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11053
thumbnail: KT11053.png
recommendations: noDisplay,noCatalog
exl-id: d6a62a26-a8ab-477c-a8f2-98f3b9ff5edf
source-git-commit: a4e61514567ac8c2b4ad5c9ecacb87bd83947731
workflow-type: ht
source-wordcount: '654'
ht-degree: 100%

---

# Esercizio sui webhook

Scopri come creare, attivare e gestire scenari avviati da webhook.

## Panoramica dell’esercizio

Lo scopo di questo scenario è creare un&#39;app da vendere ai minimarket in modo che possano determinare facilmente se un cliente ha l&#39;età giusta per acquistare alcolici. Il cassiere deve semplicemente pubblicare il nome e la data di nascita del cliente su un URL che gli è stato fornito. Tale post attiverà lo scenario che calcolerà la risposta e la restituirà al richiedente.

1. Lo scenario è costituito da tre webhook.
1. Il modulo trigger è un webhook personalizzato che resta in ascolto per un post.
1. Quando riceve un post, lo invierà a uno dei moduli successivi.
1. Il modulo successivo restituisce una risposta al richiedente.

   ![Webhook Immagine 1](../12-exercises/assets/webhooks-walkthrough-1.png)

## Passaggi da seguire

**Impostare il webhook del trigger.**

1. Crea un nuovo scenario e chiamalo “Utilizzo dei webhook”.
1. Per il trigger, aggiungi il modulo webhook personalizzato dall’app Webhooks.
1. Fai clic su Aggiungi per creare un nuovo Webhook.
1. Inserisci il nome del webhook &quot;App per bere alcolici&quot;.
1. Lascia vuote le restrizioni IP, in modo che chiunque possa inviare dati al suo interno.
1. Fai clic su Salva.


   ![Webhook Immagine 2](../12-exercises/assets/webhooks-walkthrough-2.png)

1. Nel pannello di mappatura dei webhook è stato creato un URL per questo webhook specifico. Fai clic su “Copia indirizzo negli appunti” per copiare l’URL.
1. Fai clic su OK.
1. Fai clic su Esegui una volta.
1. Utilizza l’URL in Postman per inviare un nome e una data di nascita al tuo webhook personalizzato. Per istruzioni sulla configurazione di Postman, consulta il tutorial [Procedura dettagliata sui webhook](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/beyond-basic-modules/webhooks-walkthrough.html?lang=it).

   **Il pannello del modulo Webhook dovrebbe avere un aspetto simile al seguente:**

   ![Webhook Immagine 3](../12-exercises/assets/webhooks-walkthrough-3.png)

   **Il webhook è ora in uno stato in cui è in ascolto dei dati per determinarne la struttura.**

1. È possibile definire la struttura dati del payload che si prevede di ottenere (le strutture dati verranno discusse più avanti). Se non definisci una struttura dati, Fusion la determinerà automaticamente quando il post verrà inviato.
1. Sul lato Postman desideri inviare all’URL copiato. Il post dovrebbe includere i dati del modulo di base. Per questo esempio sono necessari tre campi: Nome, Data di nascita e clientToken.

   ![Webhook Immagine 4](../12-exercises/assets/webhooks-walkthrough-4.png)

1. Dopo aver fatto clic su Invia da Postman dovresti ricevere un’indicazione che il post è stato accettato.
1. Questo è il punto in cui il tuo scenario mostrerà che la struttura dati è stata determinata con successo.
1. Puoi vedere che i dati sono stati ricevuti aprendo l’execution inspector (controllo di esecuzione).

   ![Webhook Immagine 5](../12-exercises/assets/webhooks-walkthrough-5.png)

   **Configurare l’indirizzamento per i token client.**

1. Aggiungi un router al modulo trigger.
1. Nel percorso superiore, aggiungi un modulo di risposta webhook. Questo sarà il percorso quando il token client non corrisponde.
1. Imposta lo stato su 401.
1. Imposta il corpo su {&quot;errore&quot;: &quot;Impossibile autenticare la richiesta. Controlla il clientToken&quot;}.

   ![Webhook Immagine 6](../12-exercises/assets/webhooks-walkthrough-6.png)

1. Crea un filtro tra il router e il modulo di risposta webhook. Chiamalo “Client token does not match” (Token client non corrisponde).
1. Per la condizione, utilizza il campo clientToken dal modulo trigger ed esegui un confronto numerico “Not equal to” (Non uguale a) con il numero 5121933.

   ![Immagine 7 dei webhook](../12-exercises/assets/webhooks-walkthrough-7.png)

1. Nel percorso inferiore, aggiungi un altro modulo di risposta webhook. Questo sarà il percorso da usare quando il token client corrisponde.
1. Imposta lo stato su 200.
1. Per impostare il corpo (Body), utilizza le funzioni del pannello di mappatura per verificare se la persona ha almeno 21 anni. Se sì, restituisci “You are old enough to drink!” (Sei abbastanza grande per bere), altrimenti restituisci “You are out of luck…” (Peccato).

   ![Immagine 9 dei webhook](../12-exercises/assets/webhooks-walkthrough-9.png)

1. Crea un filtro tra il router e il modulo di risposta webhook nel percorso inferiore. Chiamalo “Client token does match” (Client token corrisponde).
1. Per la condizione, utilizza il campo clientToken dal modulo trigger ed esegui un confronto numerico “Equal to” con il numero 5121933.


   ![Immagine 8 dei webhook](../12-exercises/assets/webhooks-walkthrough-8.png)

1. Fai clic sul pulsante Scheduling (Pianificazione) sotto Run once (Esegui una volta) per attivare lo scenario in modo che ogni nuovo post venga ricevuto, segua uno dei due percorsi e generi una risposta.
