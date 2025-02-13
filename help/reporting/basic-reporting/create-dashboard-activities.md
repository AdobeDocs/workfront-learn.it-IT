---
title: Creare attività dashboard
description: Esercitarsi a creare dashboard, con istruzioni dettagliate.
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335157.png
jira: KT-8862
hidefromtoc: true
source-git-commit: 915b28bbbf138fa84dce6d1915387fbe22c63362
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 49%

---

# Creare attività dashboard

Esercitarsi a creare dashboard, con istruzioni dettagliate.

## Attività 1: creare un dashboard

Crea un [!UICONTROL dashboard] contenente un solo report:&quot;Cerca note in questo progetto&quot;. Ciò è utile per trovare rapidamente qualsiasi aggiornamento apportato a un progetto, anche tra migliaia di aggiornamenti in cui cercare. In questo modo, la ricerca viene effettuata nei thread di aggiornamento per estrarre rapidamente tutti gli aggiornamenti che soddisfano i criteri specificati nelle richieste.

Crea questo rapporto effettuando una copia del rapporto &quot;Cerca note&quot; creato nell’attività &quot;Crea un rapporto di nota&quot; (oppure, se non l’hai fatto, utilizza un altro rapporto).

* Rimuovi il prompt Nome progetto dalla copia e rinomina il report &quot;Cerca note in questo progetto&quot;.
* Denomina [!UICONTROL Dashboard] &quot;Note di ricerca&quot;.
* Passa alla pagina di destinazione di qualsiasi progetto e crea una sezione personalizzata per una [!UICONTROL dashboard].
* Quando si cercano le note nella sezione personalizzata, vengono visualizzate solo le note contenute all&#39;interno del progetto in cui ci si trova.

## Risposta 1

1. Esegui il rapporto creato nell’attività &quot;Creare un rapporto di nota&quot;.
1. Fai clic su **[!UICONTROL Azioni rapporto]** e seleziona **[!UICONTROL Copia]**. [!DNL Workfront] crea un nuovo report denominato &quot;Ricerca nota (copia)&quot;.
1. Passa ad **[!UICONTROL Azioni rapporto]** e seleziona **[!UICONTROL Modifica]**. Fai clic su **[!UICONTROL Impostazioni report]** e cambia il nome in &quot;Cerca le note in questo progetto&quot;.
1. Fai clic su [!UICONTROL Prompt rapporto] ed elimina il prompt [!UICONTROL Progetto] > [!UICONTROL Nome] dall’elenco.

   ![Immagine della schermata per creare una nuova dashboard](assets/edit-report-prompts.png)

1. Seleziona la casella **[!UICONTROL Mostra prompt nella dashboard]**.
1. Fai clic su **[!UICONTROL Fine]**, quindi **[!UICONTROL Salva e Chiudi]**. Ora stai esaminando la schermata [!UICONTROL Prompt] del rapporto.

   Ora utilizzerai un collegamento per creare una nuova dashboard e aggiungere questo rapporto.

1. Fai clic su **[!UICONTROL Azioni rapporto]** e seleziona **[!UICONTROL Aggiungi alla dashboard]** > **[!UICONTROL Nuova dashboard]**.
1. Trascina il report &quot;Cerca note in questo progetto&quot; nel pannello **[!UICONTROL Layout]**.
1. Il nome del report diventa ora il nome della dashboard. Modifica il nome in &quot;Cerca note&quot;.

   ![Immagine della schermata per creare una nuova dashboard](assets/create-dashboard.png)

1. Fai clic su **[!UICONTROL Salva e Chiudi]**.

   Ora aggiungi la dashboard a una pagina di progetto.

   ![Immagine della schermata per creare una nuova dashboard](assets/add-custom-section.png)

1. Passa a qualsiasi progetto. Dal menu del pannello a sinistra, fai clic sull’icona **[!UICONTROL Aggiungi sezione personalizzata]**.
1. Nel campo **[!UICONTROL Aggiungi dashboard]** digitare &quot;Cerca note&quot; e selezionare [!UICONTROL dashboard] dall&#39;elenco.
1. Nel campo **[!UICONTROL Titolo sezione personalizzato]** digitare &quot;Cerca note&quot;.
1. Fai clic su **[!UICONTROL Aggiungi nuova sezione]**.
1. Dal menu del pannello a sinistra, trova Cerca note. Fai clic sui punti a sinistra del nome della sezione e trascinalo sotto Aggiornamenti.
