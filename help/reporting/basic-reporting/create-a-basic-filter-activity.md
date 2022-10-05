---
title: Creare un’attività filtro di base
description: In questo video, eseguirai un’attività per creare un filtro personalizzato in Workfront.
activity: use
feature: Reports and Dashboards
thumbnail: 336807.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
kt: 8856
exl-id: fc29b4ce-2937-478e-abd5-0b559657ead0
source-git-commit: b09d634a8b4ec32eda2663f1df04cc8bc04596a9
workflow-type: tm+mt
source-wordcount: '230'
ht-degree: 0%

---

# Creare un’attività filtro di base

In questo video, creerai un filtro di progetto denominato &quot;Progetti che ho chiuso questo mese&quot;. Se tieni d’occhio molti progetti, questo filtro può aiutarti a ingrandire quelli che sono pianificati per chiudersi presto.

Le istruzioni dettagliate sono incluse di seguito.

>[!VIDEO](https://video.tv.adobe.com/v/336807/?quality=12)

## Risposta

![Immagine della schermata per creare un nuovo filtro](assets/basic-filter-activity-updated-6-15-21.png)

1. Passa a [!UICONTROL Progetti] dalla [!UICONTROL Menu principale]. Viene visualizzato un elenco di progetti.
1. Fai clic sul pulsante **[!UICONTROL Filtro]** menu e seleziona **[!UICONTROL Nuovo filtro]**.
1. Denomina il filtro &quot;Progetti che possiedo Chiusura questo mese&quot;.
1. Fai clic su **[!UICONTROL Aggiungi regola filtro]**.
1. In [!UICONTROL Inizia a digitare il nome del campo] campo, digitare &quot;proprietario&quot;. Quindi seleziona [!UICONTROL ID proprietario] in [!UICONTROL Progetto] origine del campo.
1. Lascia la [!UICONTROL Uguale] l&#39;operatore così com&#39;è.
1. Digitare &quot;$$&quot; nel campo Nome digitato iniziale.
1. Seleziona [!UICONTROL $$USER.ID]. Questo è il carattere jolly per l&#39;utente connesso.
1. Fai clic su [!UICONTROL Aggiungi regola filtro] di nuovo.
1. In [!UICONTROL Inizia a digitare il nome del campo] inizia a digitare &quot;È completo&quot;. Quindi seleziona [!UICONTROL Completa] nell’origine del campo Progetto.
1. Lascia la [!UICONTROL Uguale] l&#39;operatore così com&#39;è.
1. Selezionare &quot;False&quot;.
1. Fai clic su [!UICONTROL Aggiungi regola filtro] di nuovo.
1. In [!UICONTROL Inizia a digitare il nome del campo] tipo di campo &quot;pianificato&quot;, quindi selezionare [!UICONTROL Data completamento pianificata] in [!UICONTROL Progetto] origine del campo.
1. Modificare la [!UICONTROL Uguale] operatore a [!UICONTROL Questo mese].
1. Fai clic su **[!UICONTROL Salva filtro]**
