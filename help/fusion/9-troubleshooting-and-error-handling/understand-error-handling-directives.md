---
title: Comprendere le direttive per la gestione degli errori
description: Scopri le direttive del gestore di errori che consentono il proseguimento dell’esecuzione e quelle che ne arrestano l’esecuzione, in [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: Jira ticket
exl-id: cb8d0880-73d2-4118-b800-a126f8509309
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '318'
ht-degree: 0%

---

# Comprendere le direttive per la gestione degli errori

In questo video imparerai:

* Le tre direttive del gestore di errori che consentono di continuare l&#39;esecuzione
* Le due direttive del gestore di errori che arrestano l&#39;esecuzione

>[!VIDEO](https://video.tv.adobe.com/v/335305/?quality=12)

## Direttive - Continua lo scenario

### Riprendi

* Viene specificato e fornito un output sostitutivo al modulo che rileva un errore.
* I moduli successivi vengono elaborati.
* Lo stato di esecuzione dello scenario è contrassegnato come &quot;riuscito&quot;.

![Immagine di una direttiva Resume](assets/troubleshooting-and-error-handling-2.png)

### Interruzione

* Lo stato dell’esecuzione dello scenario viene memorizzato nella coda delle esecuzioni incomplete in cui l’errore può essere risolto manualmente. Vi sono tuttavia alcune eccezioni che vengono menzionate in questa sede.
* I moduli successivi non vengono elaborati.
* Se sono presenti bundle non elaborati, l&#39;esecuzione dello scenario continua normalmente.
* Lo stato di esecuzione dello scenario è contrassegnato come &quot;avviso&quot;.

![L&#39;immagine di una direttiva di rottura](assets/troubleshooting-and-error-handling-3.png)

### Ignora

* L’errore viene ignorato e i moduli successivi non vengono elaborati.
* Se sono presenti bundle non elaborati, l&#39;esecuzione dello scenario continua normalmente.
* Lo stato di esecuzione dello scenario è contrassegnato come &quot;riuscito&quot;.

![Immagine di una direttiva Ignore](assets/troubleshooting-and-error-handling-4.png)

## Direttive - Stop allo scenario

### Ripristino

* L&#39;esecuzione dello scenario viene interrotta immediatamente e viene avviata una fase di rollback su tutti i moduli per tentare di ripristinarli tutti allo stato iniziale.
* I moduli successivi non vengono elaborati.
* Per alcuni tipi di errore, lo scenario viene disattivato dopo il &quot;numero di errori consecutivi&quot; specificato nelle impostazioni Scenario.
* Lo stato di esecuzione dello scenario è contrassegnato come &quot;error&quot;.

>[!NOTE]
>
>Questo è il comportamento predefinito se non è collegato alcun percorso del gestore di errori al modulo e l&#39;impostazione &quot;Consenti archiviazione esecuzioni incomplete&quot; nelle impostazioni Scenario non è selezionata.

![Immagine di una direttiva Rollback](assets/troubleshooting-and-error-handling-5.png)

### Conferma

* L’errore viene ignorato e i moduli successivi non vengono elaborati.
* Se sono presenti bundle non elaborati, l&#39;esecuzione dello scenario continua normalmente.
* Lo stato di esecuzione dello scenario è contrassegnato come &quot;riuscito&quot;.

![L&#39;immagine di una direttiva sui Commit](assets/troubleshooting-and-error-handling-6.png)
