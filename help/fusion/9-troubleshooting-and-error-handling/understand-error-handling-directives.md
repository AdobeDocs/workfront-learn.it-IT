---
title: Comprendere le direttive per la gestione degli errori
description: Scopri le direttive dell’handler degli errori che consentono la continuazione dell’esecuzione e quelle che la interrompono, in [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9064
exl-id: cb8d0880-73d2-4118-b800-a126f8509309
recommendations: noDisplay,catalog
doc-type: video
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: c3a155b4-a54b-4a82-a3d2-c8f0f971673e
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-06T16:07:23.288Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 318
ht-degree: 100%

---

# Comprendere le direttive per la gestione degli errori

In questo video scoprirai:

* Le tre direttive dell’handler degli errori che consentono la continuazione dell’esecuzione
* Le due direttive dell’handler degli errori che interrompono l’esecuzione

>[!VIDEO](https://video.tv.adobe.com/v/335305/?quality=12&learn=on&enablevpops=1)

## Direttive — Continuazione dello scenario

### Resume (Riprendi)

* Un output sostitutivo viene specificato e fornito al modulo che rileva un errore.
* I moduli successivi vengono elaborati.
* Lo stato di esecuzione dello scenario viene contrassegnato come “Success” (Completato).

![Immagine di una direttiva Resume (Riprendi)](assets/troubleshooting-and-error-handling-2.png)

### Break (Interrompi)

* Lo stato di esecuzione dello scenario viene memorizzato nella coda delle esecuzioni incomplete dove l’errore può essere risolto manualmente. Vi sono tuttavia alcune eccezioni qui menzionate.
* I moduli successivi non vengono elaborati.
* Se sono presenti bundle non elaborati, l’esecuzione dello scenario continua normalmente.
* Lo stato di esecuzione dello scenario è contrassegnato come “Warning” (Avvertenza).

![Immagine di una direttiva Break (Interrompi)](assets/troubleshooting-and-error-handling-3.png)

### Ignora

* L’errore viene ignorato e i moduli successivi non vengono elaborati.
* Se sono presenti bundle non elaborati, l’esecuzione dello scenario continua normalmente.
* Lo stato di esecuzione dello scenario viene contrassegnato come “Success” (Completato).

![Immagine di una direttiva Ignore (Ignora)](assets/troubleshooting-and-error-handling-4.png)

## Direttive — Interruzione dello scenario

### Rollback

* L’esecuzione dello scenario viene interrotta immediatamente e viene avviata una fase di rollback su tutti i moduli nel tentativo di ripristinarne lo stato iniziale.
* I moduli successivi non vengono elaborati.
* Salvo alcuni tipi di errore, lo scenario viene disattivato dopo il “numero di errori consecutivi” specificato nelle impostazioni dello scenario.
* Lo stato di esecuzione dello scenario è contrassegnato come “Error” (Errore).

>[!NOTE]
>
>Questo è il comportamento predefinito se al modulo non è collegato alcun percorso dell’handler degli errori e l’impostazione “Allow Storing Incomplete Executions” (Consenti memorizzazione di esecuzioni incomplete) nelle impostazioni dello scenario non è selezionata.

![Immagine di una direttiva di rollback](assets/troubleshooting-and-error-handling-5.png)

### Conferma

* L’errore viene ignorato e i moduli successivi non vengono elaborati.
* Se sono presenti bundle non elaborati, l’esecuzione dello scenario continua normalmente.
* Lo stato di esecuzione dello scenario viene contrassegnato come “Success” (Completato).

![Immagine di una direttiva Commit (Conferma)](assets/troubleshooting-and-error-handling-6.png)
