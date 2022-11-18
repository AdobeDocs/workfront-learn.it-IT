---
title: Oltre la mappatura di base
description: Scopri come utilizzare le formule del pannello di mappatura per manipolare o convertire i campi inviati a un modulo.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 11039
thumbnail: KT11039.png
exl-id: 979d794d-b936-402e-b07c-71e999f40780
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---

# Oltre la mappatura di base

Scopri come utilizzare le formule del pannello di mappatura per manipolare o convertire i campi inviati a un modulo.

## Panoramica sull&#39;esercizio

Modifica il nome del progetto, la data di inizio pianificata e la priorità dagli esercizi dettagliati della procedura dettagliata Oltre la mappatura di base utilizzando le formule del pannello di mappatura.

![Oltre la mappatura di base immagine 1](../12-exercises/assets/beyond-basic-mapping-walkthrough-1.png)

## Passaggi da seguire

**Crea un clone dello scenario di progettazione dello scenario iniziale.**

1. Selezionare l’opzione Clona a destra della progettazione dello scenario iniziale nella sezione dello scenario, come illustrato di seguito. Denomina &quot;Oltre la mappatura di base&quot;.

   ![Oltre la mappatura di base immagine 2](../12-exercises/assets/beyond-basic-mapping-walkthrough-2.png)

   **Ora utilizzeremo il pannello di mappatura nel modulo Crea progetti Workfront per configurare il nome del progetto, la data di inizio pianificata e i campi di priorità.**

1. Fai clic sul modulo Crea progetti Workfront per modificare le impostazioni. Utilizzando il pannello di mappatura, modifica il campo Nome in &quot;[Nome del progetto] da [Sponsor].&quot;

   + La [Nome del progetto] è la colonna 1 del modulo Parse CSV e [Sponsor] è la colonna 6. La parola &quot;by&quot; viene digitata tra i due.

1. Quindi, vai alla data di inizio pianificata e utilizza la formula addDays per aggiungere 15 giorni al campo, come descritto nel video introduttivo della mappatura di base Beyond .
1. Trova il campo Priorità e attiva il pulsante Mappa in alto a destra del campo. Il menu di scelta rapida diventa un numero. Crea un’istruzione if per etichettare un progetto come priorità alta(4) se il punteggio di affidabilità del file CSV è inferiore a 100, altrimenti può essere Normale(2).

   + Il punteggio di affidabilità è riportato nella colonna 4.

   **A questo punto, il pannello di mappatura deve avere un aspetto simile al seguente:**

   ![Oltre la mappatura di base immagine 3](../12-exercises/assets/beyond-basic-mapping-walkthrough-3.png)

1. Fare clic su OK e quindi su Esegui una volta.
1. Trova il progetto nella tua istanza Workfront per assicurarti che tutto sia stato mappato correttamente.
1. Salva lo scenario.
