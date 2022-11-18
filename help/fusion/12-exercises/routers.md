---
title: Router
description: Comprendere l'importanza dei router e come possono essere utilizzati per elaborare i diversi moduli in modo condizionato.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 11043
thumbnail: KT11043.png
exl-id: f2a60273-c19b-4423-b354-8cff0dd7bd6b
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '732'
ht-degree: 0%

---

# Router

Comprendere l&#39;importanza dei router e come possono essere utilizzati per elaborare i diversi moduli in modo condizionato.

## Panoramica sull&#39;esercizio

Utilizzare un router per passare i bundle Pokemon vs. supereroi nel percorso corretto, quindi creare un&#39;attività per ogni carattere.

![Router Immagine 1](../12-exercises/assets/routers-walkthrough-1.png)

## Passaggi da seguire

1. Clona lo scenario Utilizzo di connettori universali dall’esercizio precedente. Denominalo &quot;Creazione di percorsi diversi utilizzando i router&quot;.

   **Crea un nuovo percorso per i supereroi clonando moduli e aggiungendo un router.**

   ![Router Immagine 2](../12-exercises/assets/routers-walkthrough-2.png)

1. Fare clic con il pulsante destro del mouse sul modulo Get Pokemon info e scegliere Clone. Una volta clonata, trascinala e collegala alla linea tra il nuovo modulo HTTP e il modulo CSV Parse.

   >[!NOTE]
   >
   > Osserva come aggiunge automaticamente un router con due percorsi.

1. Denomina questo modulo &quot;Ottieni l&#39;aspetto del supereroe&quot;.
1. Clona questo modulo, sposta il clone a destra e lo chiama &quot;Ottieni abilità supereroe&quot;.
1. Clonare il modulo Strumenti e spostarlo alla fine del secondo percorso.
1. Fare clic sull’icona della bacchetta, il pulsante Allinea automaticamente, nella barra degli strumenti.

   **Il tuo scenario dovrebbe essere simile al seguente:**

   ![Router Immagine 3](../12-exercises/assets/routers-walkthrough-3.png)

   **Successivamente, verranno modificati i valori mappati nei nuovi moduli clonati.**

1. Vai a <https://www.superheroapi.com/> e utilizza il tuo account Facebook per ottenere un token di accesso.

   >[!NOTE]
   >
   >Se hai problemi ad accedere al tuo token supereroe, puoi usare questo token condiviso: 10110256647253588. Presta attenzione a quante volte chiami l’API del supereroe in modo che questo token condiviso continui a funzionare per tutti.

1. Apri le impostazioni per l’aspetto Ottieni supereroe e modifica l’URL in `https://www.superheroapi.com/api/[access- token]/332/appearance`. Accertati di includere il token di accesso nell’URL. Fate clic su OK.
1. Apri le impostazioni per le funzionalità Get superhero e modifica l&#39;URL in `https://www.superheroapi.com/api/[access- token]/332/powerstats`. Accertati di includere il token di accesso nell’URL. Fate clic su OK.
1. Fai clic con il pulsante destro del mouse su ciascun modulo supereroe e seleziona Esegui solo questo modulo. In questo modo verrà generata la struttura dati da visualizzare per la mappatura.
1. Dopo aver eseguito entrambi, cambia il numero &quot;332&quot; in ciascun campo URL in Colonna 4 mappata dal modulo Analizza CSV.

   ![Router Immagine 4](../12-exercises/assets/routers-walkthrough-4.png)

   **Ora puoi fare clic sul modulo Imposta più variabili nel percorso del supereroe e aggiornare nome, altezza, peso e abilità.**

1. Aggiorna i campi Nome e Abilità dal modulo Ottieni abilità supereroe—Modulo 8.

   ![Router Immagine 5](../12-exercises/assets/routers-walkthrough-5.png)

1. Aggiornare i campi Altezza e Peso dal modulo Ottieni aspetto supereroe, Modulo 6.

   ![Router Immagine 6](../12-exercises/assets/routers-walkthrough-6.png)

   **Al termine, le variabili devono avere questo aspetto. I numeri del modulo vengono visualizzati nei valori del campo.**

   ![Router Immagine 7](../12-exercises/assets/routers-walkthrough-7.png)

1. Fare clic su OK, quindi salvare lo scenario.

   **Crea un altro percorso per creare un&#39;attività per carattere.**

1. In Workfront, crea un progetto vuoto. Denomina &quot;Shipping Manifest Project&quot; e copia l&#39;ID del progetto dall&#39;URL.
1. Tornare a Workfront Fusion e fare clic nel centro del router per creare un altro percorso.

   ![Router Immagine 8](../12-exercises/assets/routers-walkthrough-8.png)

1. Fai clic al centro del modulo vuoto che viene visualizzato e aggiungi un modulo Crea record dall’app Workfront.
1. Imposta Tipo di record su Attività e seleziona ID progetto dalla sezione Campi da mappare .
1. Incolla l&#39;ID progetto copiato da Workfront nel campo ID progetto .
1. Ora, seleziona il campo Nome dalla sezione Campi da mappare .
1. Assegna un nome all&#39;attività &quot;[Carattere] da [Franchise],&quot; prendendo il nome del carattere e il nome del franchising dal file CSV. La colonna 3 è il nome del carattere e la colonna 2 è il nome del franchising.

   ![Router Immagine 9](../12-exercises/assets/routers-walkthrough-9.png)

1. Fare clic su OK e rinominare questo modulo in &quot;Crea un&#39;attività per ogni carattere&quot;.

   **Aggiungi i filtri in modo che lo scenario possa essere eseguito senza errori. Vuoi che solo i personaggi Pokemon scendano lungo il sentiero superiore, solo i personaggi dei supereroi che scendano lungo il sentiero centrale, e tutti i personaggi che scendono lungo il sentiero inferiore.**

1. Fai clic sulla linea tratteggiata a sinistra del modulo Get Pokemon info per creare il primo filtro. Denomina &quot;Pokemon personaggio.&quot;
1. Per la condizione, consenti solo record in cui il franchising (Colonna 2) è uguale a &quot;Pokemon&quot;. Scegli l’operatore &quot;Uguale a&quot; del testo.
1. Fai clic sulla linea tratteggiata a sinistra del modulo di aspetto Ottieni supereroe per creare il filtro successivo. Chiamalo &quot;personaggio supereroe&quot;.
1. Poiché i supereroi possono provenire da varie franchising, utilizza il campo ID supereroe (Colonna 4) per determinare se un personaggio è un supereroe o meno.

   **I filtri dovrebbero essere così:**

   ![Router Immagine 11](../12-exercises/assets/routers-walkthrough-11.png)

   ![Immagine router 10](../12-exercises/assets/routers-walkthrough-10.png)

1. Salva lo scenario e fai clic su Esegui una volta. Utilizzare gli ispettori di esecuzione per verificare che tutte le operazioni siano state completate e controllare le attività create nel progetto Workfront.

   ![Immagine router 12](../12-exercises/assets/routers-walkthrough-12.png)
