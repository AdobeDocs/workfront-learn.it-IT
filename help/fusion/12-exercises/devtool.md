---
title: Strumento di sviluppo
description: Migliora le tue capacità di risolvere i problemi di uno scenario e semplifica le configurazioni complesse utilizzando DevTool.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11057
thumbnail: KT11057.png
exl-id: 13080212-26cf-4e5f-8f0b-fc59a6f66eb1
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 0%

---

# Strumento di sviluppo

Migliora le tue capacità di risolvere i problemi di uno scenario e semplifica le configurazioni complesse utilizzando lo strumento di sviluppo.

## Panoramica dell’esercizio

Installa e utilizza le diverse aree dello strumento Workfront Dev per approfondire richieste/risposte e trucchi avanzati di progettazione degli scenari.

>[!NOTE]
>
>Lo strumento Workfront Fusion Dev è disponibile solo nel browser Chrome quando si utilizza [Strumento per sviluppatori Chrome](https://developer.chrome.com/docs/devtools/).

![Devtool Image 1](../12-exercises/assets/devtool-walkthrough-1.png)

## Passaggi da seguire

**Installare lo strumento di sviluppo.**

1. Scaricare il documento &quot;workfront-fusion-devtool.zip&quot; presente nella cartella dei file di esercizio di Fusion nell&#39;unità di prova.
1. Estrai i file ZIP in una cartella.
1. Apri una scheda in Chrome e immetti **chrome://extensions**.
1. Attiva la modalità Sviluppatore utilizzando lo switch in alto a destra, quindi fai clic sul pulsante &quot;Load unpacked&quot; che viene visualizzato in alto a sinistra. Selezionare la cartella contenente lo strumento di sviluppo (dove è stato decompresso).

   ![Devtool Image 2](../12-exercises/assets/devtool-walkthrough-2.png)

1. Una volta decompresso, lo strumento Dev viene visualizzato tra le altre estensioni.

   ![Devtool Image 3](../12-exercises/assets/devtool-walkthrough-3.png)

   **Utilizza Live Stream.**

1. Per iniziare, apri lo scenario &quot;Utilizzo degli archivi dati per sincronizzare i dati&quot;.
1. Aprire lo strumento Dev digitando F12 o F12. Oppure puoi fare clic sul menu a tre punti nella barra degli indirizzi di Chrome e passare a Strumenti per sviluppatori.

   ![Immagine Devtool 4](../12-exercises/assets/navigate-to-devtools.png)

1. Fai clic sulla scheda Workfront Fusion, quindi seleziona Live Stream dall’elenco a sinistra.
1. Fai clic su Esegui una volta per visualizzare gli eventi nel momento in cui si verificano.
1. Fai clic su un evento per visualizzare le schede a destra per Intestazioni di richiesta, Corpo della richiesta, Intestazioni di risposta e Corpo della risposta.

   ![Immagine Devtool 4](../12-exercises/assets/devtool-walkthrough-4.png)

   **Utilizzare Scenario Debugger**

1. Seleziona Scenario Debugger e fai clic su un modulo per visualizzare informazioni sulle operazioni del modulo.

   ![Immagine Devtool 5](../12-exercises/assets/devtool-walkthrough-5.png)

1. Passare alla scheda Cronologia. Fare clic su Dettagli su un&#39;esecuzione per esaminare i dettagli delle operazioni del modulo per un&#39;esecuzione specifica.

   ![Immagine Devtool 6](../12-exercises/assets/devtool-walkthrough-6.png)

   **Utilizzare gli strumenti**

1. Torna alla finestra di progettazione dello scenario e seleziona Strumenti nello strumento di sviluppo. Vengono visualizzati gli strumenti disponibili.

   ![Immagine Devtool 7](../12-exercises/assets/devtool-walkthrough-7.png)

+ Mettere a fuoco un modulo: trova e apri rapidamente un modulo utilizzando l’ID modulo.
+ Trova moduli per mappatura: cerca uno scenario utilizzando una parola chiave per trovare valori e/o chiavi mappati nei moduli.
+ Ottieni metadati app: consulta i metadati per l’app selezionata in uno scenario.
+ Copia mappatura: copia la mappatura da un modulo all’altro. Puoi anche clonare il modulo nella finestra di progettazione.
+ Copia filtro: copia un filtro. Il filtro viene sempre assegnato al modulo sulla destra.
+ Scambia connessione: lo strumento prende la connessione dal modulo selezionato e imposta la stessa connessione a tutti i moduli della stessa app nello scenario. Questa funzione è utile se devi modificare la connessione durante un completamento. Usando questo strumento, evita di perdere tutte le mappature e risparmia tempo.
+ Scambia variabile: trova tutte le occorrenze della variabile specificata in tutto lo scenario o in un modulo e le sostituisce con la nuova. I caratteri jolly non sono supportati. Se hai mappato accidentalmente un valore in tutto lo scenario, questo può aiutarti a scambiare facilmente il valore corretto.
+ Scambia app: scambia l’app specificata con un’altra.
+ Base 64: codifica i dati immessi in Base 64 o decodifica Base 64. Utile quando desideri cercare dati particolari nella richiesta codificata.
+ Copia nome modulo: copia negli Appunti il nome del modulo selezionato.
+ Origine della rimappatura: modifica l’origine della mappatura da un modulo all’altro. Devi innanzitutto aggiungere il modulo da utilizzare come modulo di origine al ciclo di lavorazione in uno scenario.
+ Migrazione del sistema operativo: realizzato appositamente per aggiornare i moduli Google Sheets (legacy) alla versione più recente di Google Sheets. Aggiunge una nuova versione del modulo subito dopo la versione legacy del modulo nel percorso dello scenario.
