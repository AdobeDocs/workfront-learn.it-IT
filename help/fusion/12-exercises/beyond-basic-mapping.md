---
title: Oltre la mappatura di base
description: Scopri come utilizzare le formule del pannello di mappatura per manipolare o convertire i campi inviati a un modulo.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11039
thumbnail: KT11039.png
exl-id: 979d794d-b936-402e-b07c-71e999f40780
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---

# Oltre la mappatura di base

Scopri come utilizzare le formule del pannello di mappatura per manipolare o convertire i campi inviati a un modulo.

## Panoramica dell’esercizio

Modifica il nome del progetto, la data di inizio pianificata e la priorità dagli esercizi di procedura dettagliata Oltre le mappature di base utilizzando le formule del pannello di mappatura.

![Oltre l&#39;immagine di mappatura di base 1](../12-exercises/assets/beyond-basic-mapping-walkthrough-1.png)

## Passaggi da seguire

**Crea un clone dello scenario di progettazione iniziale.**

1. Selezionare l&#39;opzione Clona a destra della progettazione dello scenario iniziale nella sezione dello scenario, come illustrato di seguito. Denominalo &quot;Oltre la mappatura di base&quot;.

   ![Oltre l&#39;immagine di mappatura di base 2](../12-exercises/assets/beyond-basic-mapping-walkthrough-2.png)

   **Ora utilizzeremo il pannello di mappatura nel modulo Crea progetti Workfront per configurare i campi Nome del progetto, Data di inizio pianificata e Priorità.**

1. Fai clic sul modulo Crea progetti Workfront per modificare le impostazioni. Utilizzando il pannello di mappatura, imposta il campo Nome su &quot;[Nome progetto] da [Sponsor].&quot;

   + Il [Nome progetto] è la colonna 1 del modulo CSV di analisi e [Sponsor] è la colonna 6. La parola &quot;by&quot; è solo digitata tra le due.

1. Passare quindi alla Data inizio pianificata e utilizzare la formula addDays per aggiungere 15 giorni al campo, come descritto nel video della procedura dettagliata relativa alla mappatura di base di Beyond.
1. Trova il campo Priorità e attiva il pulsante Mappa in alto a destra del campo. Il menu dell’elenco a discesa diventa un numero. Crea un&#39;istruzione if per etichettare un progetto come priorità Alta(4) se il livello di affidabilità del file CSV è inferiore a 100, altrimenti può essere Normale(2).

   + Il valore di affidabilità è riportato nella colonna 4.

   **A questo punto, il pannello di mappatura sarà simile al seguente:**

   ![Oltre l&#39;immagine di mappatura di base 3](../12-exercises/assets/beyond-basic-mapping-walkthrough-3.png)

1. Fare clic su OK e quindi su Esegui una volta.
1. Trova il progetto nell’istanza Workfront per assicurarti che tutto sia stato mappato correttamente.
1. Salva lo scenario.
