---
title: Modulo switch
description: Scopri come utilizzare il modulo Switch quando devi eseguire trasformazioni di dati più complesse o dinamiche.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11052
thumbnail: KT11052.png
exl-id: 1b810168-582d-4d7d-b061-d152af546bc8
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '319'
ht-degree: 0%

---

# Modulo switch

Scopri come utilizzare il modulo Switch quando devi eseguire trasformazioni di dati più complesse o dinamiche.

## Panoramica dell’esercizio

Cerca i progetti di direct mailing nell&#39;unità di test, quindi modifica il nome di ciascun progetto in base a un valore selezionato in un campo personalizzato allegato al progetto.

![Modulo switch Immagine 1](../12-exercises/assets/switch-module-walkthrough-1.png)

## Passaggi da seguire

1. Creare un nuovo scenario e denominarlo &quot;Utilizzo del modulo Switch&quot;.
1. Per il modulo trigger, utilizza il modulo Workfront Search.
1. Imposta la connessione Workfront e imposta il tipo di record su Progetto.
1. Nei criteri di ricerca, specifica che desideri visualizzare solo i progetti con un valore nel campo personalizzato Canale.
1. Per gli output, seleziona ID, Nome, Numero di riferimento e il campo personalizzato Canale.

   ![Modulo switch Immagine 2](../12-exercises/assets/switch-module-walkthrough-2.png)

1. Aggiungere il modulo Switch da Strumenti.
1. Per il campo Input, mappa il campo personalizzato Canale dal modulo di ricerca.

   ![Modulo switch Immagine 3](../12-exercises/assets/switch-module-walkthrough-3.png)

1. Quindi aggiungi dei casi per ogni possibile valore proveniente dal campo personalizzato Canale. Il valore possibile viene inserito nel campo Pattern. Il campo di output deve includere un codice di 3 lettere specifico seguito dal numero di riferimento del progetto e quindi dal nome del progetto.

   **Il pannello di mappatura deve essere simile al seguente:**

   ![Modulo switch Immagine 4](../12-exercises/assets/switch-module-walkthrough-4.png)

1. Puoi aggiungere tutti i casi aggiuntivi che desideri. Osserva il campo Else in basso. Verrà utilizzato se il valore specificato non corrisponde a nessuno dei casi.

   **Aggiorna il nome del progetto in Workfront.**

   ![Modulo switch Immagine 5](../12-exercises/assets/switch-module-walkthrough-5.png)

1. Aggiungere un modulo Record di Workfront Update.
1. Nel campo ID, mappa con l’ID dal modulo trigger.
1. Impostare Tipo record su Progetto.
1. Selezionare il campo Nome dalla sezione Seleziona campi da mappare e associarlo all&#39;output del modulo Switch.
1. Salva lo scenario ed esegui una volta. Visualizza i nomi dei progetti aggiornati nell’unità di test.
