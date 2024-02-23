---
title: Esercitazione sui router
description: Comprendere l’importanza dei router e come utilizzarli per elaborare in modo condizionale i diversi moduli.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11043
thumbnail: KT11043.png
recommendations: noDisplay,noCatalog
exl-id: f2a60273-c19b-4423-b354-8cff0dd7bd6b
source-git-commit: a4e61514567ac8c2b4ad5c9ecacb87bd83947731
workflow-type: ht
source-wordcount: '755'
ht-degree: 100%

---

# Esercitazione sui router

Comprendere l’importanza dei router e come utilizzarli per elaborare in modo condizionale i diversi moduli.

## Panoramica dell’esercizio

Utilizza un router per passare i bundle Pokemon e supereroi lungo il percorso corretto, quindi crea un’attività per ogni carattere.

![Router immagine 1](../12-exercises/assets/routers-walkthrough-1.png)

## Passaggi da seguire

1. Clona lo scenario Utilizzo dei connettori universali dell’esercizio precedente. Denominalo “Creazione di percorsi diversi utilizzando i router”.

   **Crea un nuovo percorso per i supereroi clonando i moduli e aggiungendo un router.**

   ![Router immagine 2](../12-exercises/assets/routers-walkthrough-2.png)

1. Fai clic con il pulsante destro del mouse sul modulo Ottieni informazioni Pokemon e scegli Clona. Una volta clonato, trascinalo e collegalo alla linea tra il nuovo modulo HTTP e il modulo Analizza CSV.

   >[!NOTE]
   >
   > Nota come aggiunge automaticamente un router con due percorsi.

1. Denomina questo modulo “Ottieni l’aspetto di supereroe”.
1. Clona questo modulo, sposta il clone a destra e denominalo “Ottieni abilità da supereroe”.
1. Clona il modulo Strumenti e spostalo alla fine del secondo percorso.
1. Fai clic sull’icona della bacchetta, il pulsante Allineamento automatico, nella barra degli strumenti.

   **Lo scenario dovrebbe essere simile al seguente:**

   ![Router immagine router 3](../12-exercises/assets/routers-walkthrough-3.png)

   **Successivamente, modificherai i valori mappati nei nuovi moduli clonati.**

1. Vai a <https://www.superheroapi.com/> e utilizza il tuo account Facebook per ottenere un token di accesso.

   >[!NOTE]
   >
   >Se hai problemi ad accedere al tuo token di supereroe, puoi utilizzare questo token condiviso: 10110256647253588. Tieni in considerazione quante volte richiami l’API supereroe in modo che questo token condiviso continui a funzionare per tutti.

1. Apri le impostazioni relative all’aspetto Ottieni supereroe e modifica l’URL in `https://www.superheroapi.com/api/[access- token]/332/appearance`. Assicurati di includere il token di accesso nell’URL. Fai clic su OK.
1. Apri le impostazioni per le abilità Ottieni supereroe e modifica l’URL in `https://www.superheroapi.com/api/[access- token]/332/powerstats`. Assicurati di includere il token di accesso nell’URL. Fai clic su OK.
1. Fai clic con il pulsante destro del mouse su ciascun modulo di supereroe e seleziona Esegui solo questo modulo. Verrà generata la struttura dati necessaria per la mappatura.
1. Dopo aver eseguito entrambi, modifica il numero “332” in ciascun campo URL in Colonna 4 mappata dal modulo Analizza CSV.

   ![Router immagine 4](../12-exercises/assets/routers-walkthrough-4.png)

   **Ora puoi fare clic sul modulo Imposta più variabili nel percorso di supereroe e aggiornare il nome, l’altezza, il peso e le abilità.**

1. Aggiorna i campi Nome e Abilità dal modulo Ottieni abilità da supereroe (modulo 8).

   ![Router immagine 5](../12-exercises/assets/routers-walkthrough-5.png)

1. Aggiorna i campi Altezza e Spessore dal modulo Ottieni aspetto supereroe (modulo 6).

   ![Router immagine 6](../12-exercises/assets/routers-walkthrough-6.png)

   **Al termine dell’operazione, le variabili dovrebbero avere questo aspetto. I numeri dei moduli vengono visualizzati nei valori campo.**

   ![Router immagine 7](../12-exercises/assets/routers-walkthrough-7.png)

1. Fai clic su OK, quindi salva lo scenario.

   **Crea un altro percorso per generare un’attività per personaggio.**

1. In Workfront, crea un progetto vuoto. Denominalo “Progetto Manifesto di spedizione” e copia l’ID del progetto dall’URL.
1. Torna a Workfront Fusion e fai clic al centro del router per creare un altro percorso.

   ![Router immagine 8](../12-exercises/assets/routers-walkthrough-8.png)

1. Fai clic al centro del modulo vuoto visualizzato e aggiungi un modulo Crea record dall’app Workfront.
1. Imposta Tipo record su Attività e seleziona ID progetto dalla sezione Campi da mappare.
1. Incolla l’ID progetto copiato da Workfront nel campo ID progetto.
1. Seleziona ora il campo Nome dalla sezione Campi da mappare.
1. Denomina l’attività “[Personaggio] da [Franchise]”, prendendo il nome del personaggio e il nome del franchise dal file CSV. La colonna 3 è il nome del personaggio e la colonna 2 è il nome del franchise.

   ![Router immagine 9](../12-exercises/assets/routers-walkthrough-9.png)

1. Fai clic su OK e rinomina questo modulo in “Crea un’attività per ogni personaggio”.

   **Aggiungi filtri in modo che lo scenario possa essere eseguito senza errori. Desideri che solo i personaggi Pokemon percorrano il percorso principale, solo i personaggi supereroi percorrano il percorso centrale e tutti i personaggi percorrano il percorso inferiore.**

1. Fai clic sulla linea tratteggiata a sinistra del modulo Ottieni informazioni Pokemon per creare il primo filtro. Denominalo “Personaggio Pokemon”.
1. Per la condizione, consenti solo i record in cui il franchise (colonna 2) sia uguale a “Pokemon”. Scegli l’operatore di testo “Uguale a”.
1. Fai clic sulla linea tratteggiata a sinistra del modulo Ottieni l’aspetto di supereroe per creare il filtro successivo. Denominalo “Personaggio Supereroe”.
1. Poiché i supereroi possono provenire da vari franchise, utilizza il campo ID supereroe (Colonna 4) per determinare se un personaggio è un supereroe o meno.

   **I filtri dovrebbero essere simili a quanto segue:**

   ![Router immagine 11](../12-exercises/assets/routers-walkthrough-11.png)

   ![Router immagine 10](../12-exercises/assets/routers-walkthrough-10.png)

1. Salva lo scenario e fai clic su Esegui una volta. Utilizza i controlli di esecuzione per verificare che tutte le operazioni siano state completate correttamente e controlla le attività create nel progetto Workfront.

   ![Router immagine 12](../12-exercises/assets/routers-walkthrough-12.png)
