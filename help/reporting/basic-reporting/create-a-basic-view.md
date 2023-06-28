---
title: Creare una visualizzazione di base
description: Scopri che cos’è una visualizzazione, come crearla e come condividerla con altri utenti in Workfront.
activity: use
feature: Reports and Dashboards
thumbnail: 335148.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
last-substantial-update: 2023-06-20T00:00:00Z
jira: KT-8854
exl-id: ba3c0e10-dcf1-4a7b-bf11-ccfed9040e6d
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '696'
ht-degree: 6%

---

# Creare una visualizzazione di base

Questo video illustra:

* Che cos’è una visualizzazione in Workfront
* Come creare e modificare una vista
* Come condividere una visualizzazione con altri utenti di Workfront

>[!VIDEO](https://video.tv.adobe.com/v/335148/?quality=12&learn=on)

## Attività 1: creare una visualizzazione dello stato delle attività

I project manager, i responsabili del team o i responsabili delle risorse devono tenere traccia dell&#39;avanzamento del lavoro dell&#39;attività. Con questa visualizzazione, si ottengono diversi indicatori di stato di un&#39;attività tutti in una riga dell&#39;elenco o del report.

Creare una visualizzazione delle attività denominata &quot;Visualizzazione stato attività&quot; con le colonne riportate di seguito.

* [!UICONTROL Nome attività]
* [!UICONTROL Assegnazioni]
* [!UICONTROL Durata]
* [!UICONTROL Percentuale completato]
* [!UICONTROL Stato]
* [!UICONTROL Stato di Avanzamento]
* [!UICONTROL Le icone di Stato]

## Risposta attività 1

![Immagine della schermata per creare una visualizzazione dello stato dell&#39;attività](assets/view-exercise.png)

1. In un report elenco attività, passare alla **[!UICONTROL Visualizza]** menu a discesa e selezionare **[!UICONTROL Nuova visualizzazione]**.
1. Denomina la visualizzazione &quot;Visualizzazione stato attività&quot;.
1. Rimuovi queste colonne: [!UICONTROL Ore Pian], [!UICONTROL Predecessori], [!UICONTROL Inizia il], e [!UICONTROL Scade il].
1. Clic **[!UICONTROL Aggiungi colonna]**.
1. In [!UICONTROL Mostra in questa colonna] , digitare &quot;status&quot; quindi selezionare &quot;Status&quot; sotto il [!UICONTROL Attività] origine del campo.
1. Clic **[!UICONTROL Aggiungi colonna]** di nuovo.
1. In [!UICONTROL Mostra in questa colonna] , digitare &quot;status&quot; quindi selezionare &quot;Progress Status&quot; (Stato di avanzamento) sotto [!UICONTROL Attività] origine del campo.
1. Clic **[!UICONTROL Aggiungi colonna]** di nuovo.
1. In [!UICONTROL Mostra in questa colonna] , digitare &quot;status&quot; quindi selezionare &quot;Status Icons&quot; nell&#39;origine del campo Task.
1. Fai clic su **[!UICONTROL Salva]**.

Passa il puntatore del mouse su ciascuna delle icone [!UICONTROL Icone di stato] per vedere cosa rappresentano. Se sono disattivate, significa che l&#39;attività non contiene note, documenti, processi di approvazione e così via. Se viene visualizzata un&#39;icona a colori, all&#39;attività è associato almeno un elemento. È possibile fare clic sulla nota o sulle icone del documento per passare a tale elemento.

## Attività 2: creare una vista milestone

Se utilizzi le milestone, questa vista rappresenta il modo più semplice per visualizzare le milestone per nome e aggiungerle o modificarle utilizzando la modifica in linea.

Creare una visualizzazione delle attività denominata &quot;Vista Milestone&quot; con le colonne seguenti:

* [!UICONTROL Nome attività]
* [!UICONTROL Assegnazioni]
* [!UICONTROL Durata]
* [!UICONTROL Ore pian.]
* [!UICONTROL Milestone: Name]
* [!UICONTROL Inizia il]
* [!UICONTROL Scade il]
* [!UICONTROL Percentuale completato]


## Risposta attività 2

![Immagine dello schermo per creare una vista milestone](assets/view-milestone-exercise-1.png)

1. In un elenco delle attività di un progetto, vai al **[!UICONTROL Visualizza]** menu a discesa e selezionare **[!UICONTROL Nuova visualizzazione]**.
1. Denomina la visualizzazione &quot;Vista Milestone&quot;.
1. Fai clic sul pulsante [!UICONTROL Predecessori] per selezionarla.
1. In [!UICONTROL Mostra in questa colonna] , fai clic sull’icona X nella sezione [!UICONTROL Attività >> Predecessori] , quindi digita &quot;[!UICONTROL nome milestone]&quot; e fai clic su &quot;[!UICONTROL Nome]&quot; nell’elenco.
1. Fai clic su **[!UICONTROL Salva]**.

![Immagine di un elenco di attività in una visualizzazione milestone](assets/view-milestone-exercise-2.png)

## Attività 3: creare una vista dei vincoli dei tipi di durata e delle attività

Questa vista consente di esaminare e modificare tutti i tipi di durata e i vincoli delle attività nel progetto.

Creare una vista delle attività denominata &quot;Visualizzazione tipi di durata e vincoli di attività&quot; con le colonne riportate di seguito.

* [!UICONTROL Nome attività]
* [!UICONTROL Assegnazioni]
* [!UICONTROL Durata]
* [!UICONTROL Durata Pianificata]
* [!UICONTROL Ore pian.]
* [!UICONTROL Predecessori]
* [!UICONTROL Inizia il]
* [!UICONTROL Scade il]
* [!UICONTROL Tipo di Durata]
* [!UICONTROL Vincolo attività]
* [!UICONTROL Data Vincolata]

Modificare il [!UICONTROL Formato campo] il [!UICONTROL Inizia il] e [!UICONTROL Scade il] colonne per visualizzare sia la data che l&#39;ora.

## Risposta all&#39;attività 3

![Un&#39;immagine della schermata che mostra la vista dei vincoli dei tipi di durata e delle attività](assets/view-activity-3.png)

1. In un elenco delle attività di un progetto, vai al **[!UICONTROL Visualizza]** menu a discesa e selezionare **[!UICONTROL Nuova visualizzazione]**.
1. Denomina la vista &quot;Visualizzazione dei tipi di durata e dei vincoli delle attività&quot;.
1. Rimuovi il [!UICONTROL % completamento] colonna.
1. Clic **[!UICONTROL Aggiungi colonna]**.
1. In [!UICONTROL Mostra in questa colonna] campo, tipo [!UICONTROL &quot;duration&quot;] quindi seleziona [!UICONTROL &quot;Durata Pianificata&quot;] sotto [!UICONTROL Attività] origine del campo.
1. Sposta questa colonna tra [!UICONTROL Durata] e [!UICONTROL Ore Pian] colonne.
1. Clic **[!UICONTROL Aggiungi colonna]** di nuovo.
1. In [!UICONTROL Mostra in questa colonna] campo, tipo [!UICONTROL &quot;tipo di durata&quot;] quindi seleziona [!UICONTROL &quot;Tipo di durata&quot;] sotto [!UICONTROL Attività] origine del campo.
1. Clic **[!UICONTROL Aggiungi colonna]** di nuovo.
1. In [!UICONTROL Mostra in questa colonna] campo, tipo [!UICONTROL &quot;vincolo&quot;] quindi seleziona [!UICONTROL &quot;Vincolo attività&quot;] nell&#39;origine del campo Attività.
1. Clic **[!UICONTROL Aggiungi colonna]** di nuovo.
1. In [!UICONTROL Mostra in questa colonna] campo, tipo [!UICONTROL &quot;vincolo&quot;] quindi seleziona [!UICONTROL &quot;Data Vincolata&quot;] nell&#39;origine del campo Attività.
1. Seleziona la [!UICONTROL Inizia il] , quindi fai clic su [!UICONTROL Opzioni avanzate].
1. Sotto [!UICONTROL Formato campo] menu a discesa seleziona [!UICONTROL &quot;10/17/60 03.00&quot;].
1. Seleziona la [!UICONTROL Scade il] , quindi fai clic su [!UICONTROL Opzioni avanzate].
1. Sotto [!UICONTROL Formato campo] menu a discesa seleziona [!UICONTROL &quot;10/17/60 03.00&quot;].
1. Fai clic su **[!UICONTROL Salva]**.
