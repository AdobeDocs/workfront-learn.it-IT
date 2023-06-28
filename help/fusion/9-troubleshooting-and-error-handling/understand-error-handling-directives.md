---
title: Comprendere le direttive per la gestione degli errori
description: Scopri le direttive del gestore degli errori che consentono la continuazione dell’esecuzione e quelle che la interrompono, in [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9064
exl-id: cb8d0880-73d2-4118-b800-a126f8509309
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '318'
ht-degree: 0%

---

# Comprendere le direttive per la gestione degli errori

Questo video illustra:

* Le tre direttive del gestore degli errori che consentono la continuazione dell’esecuzione
* Le due direttive del gestore degli errori che interrompono l’esecuzione

>[!VIDEO](https://video.tv.adobe.com/v/335305/?quality=12&learn=on)

## Direttive — Scenario continua

### Riprendi

* Viene specificato e fornito un output sostitutivo al modulo che rileva un errore.
* Vengono elaborati i moduli successivi.
* Lo stato di esecuzione dello scenario è contrassegnato come &quot;Completato&quot;.

![Immagine di una direttiva Riprendi](assets/troubleshooting-and-error-handling-2.png)

### Interrompi

* Lo stato dell’esecuzione dello scenario viene memorizzato nella coda di esecuzioni incomplete, dove l’errore può essere risolto manualmente. Vi sono tuttavia alcune eccezioni qui menzionate.
* I moduli successivi non vengono elaborati.
* Se sono presenti bundle non elaborati, l’esecuzione dello scenario continua normalmente.
* Lo stato di esecuzione dello scenario è contrassegnato come &quot;avviso&quot;.

![Immagine di una direttiva di interruzione](assets/troubleshooting-and-error-handling-3.png)

### Ignora

* L’errore viene ignorato e i moduli successivi non vengono elaborati.
* Se sono presenti bundle non elaborati, l’esecuzione dello scenario continua normalmente.
* Lo stato di esecuzione dello scenario è contrassegnato come &quot;Completato&quot;.

![Immagine di una direttiva Ignora](assets/troubleshooting-and-error-handling-4.png)

## Direttive — Interruzione dello scenario

### Rollback

* L’esecuzione dello scenario viene interrotta immediatamente e viene avviata una fase di rollback su tutti i moduli nel tentativo di ripristinarne lo stato iniziale.
* I moduli successivi non vengono elaborati.
* Salvo alcuni tipi di errore, lo scenario viene disattivato dopo il &quot;numero di errori consecutivi&quot; specificato in Impostazioni scenario.
* Lo stato di esecuzione dello scenario è contrassegnato come &quot;error&quot; (Errore).

>[!NOTE]
>
>Questo è il comportamento predefinito se al modulo non è collegata alcuna route del gestore degli errori e l’impostazione &quot;Consenti memorizzazione di esecuzioni incomplete&quot; in Impostazioni scenario non è selezionata.

![Immagine di una direttiva di rollback](assets/troubleshooting-and-error-handling-5.png)

### Conferma

* L’errore viene ignorato e i moduli successivi non vengono elaborati.
* Se sono presenti bundle non elaborati, l’esecuzione dello scenario continua normalmente.
* Lo stato di esecuzione dello scenario è contrassegnato come &quot;Completato&quot;.

![Immagine di una direttiva Commit](assets/troubleshooting-and-error-handling-6.png)
