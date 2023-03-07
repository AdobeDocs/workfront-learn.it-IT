---
title: Creare un’attività filtro di base
description: In questa attività creerai un filtro per progetti denominato "Progetti di cui sono Proprietario che chiudono questo mese".
activity: use
feature: Reports and Dashboards
thumbnail: 336807.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
kt: 8856
exl-id: fc29b4ce-2937-478e-abd5-0b559657ead0
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---

# Creare un’attività filtro di base

Questo video illustra come creare un filtro per i progetti denominato &quot;Progetti di cui sono Proprietario - Chiusura di questo mese&quot;. Se stai tenendo d’occhio molti progetti, questo filtro può aiutarti a ingrandire quelli che si prevede di chiudere a breve.

Le istruzioni dettagliate sono incluse di seguito.

>[!VIDEO](https://video.tv.adobe.com/v/336807/?quality=12)

## Risposta

![Immagine dello schermo per creare un nuovo filtro](assets/basic-filter-activity-updated-6-15-21.png)

1. Accedi a [!UICONTROL Progetti] area da [!UICONTROL Menu principale]. Qui viene visualizzato un elenco di progetti.
1. Fai clic su **[!UICONTROL Filtro]** menu e seleziona **[!UICONTROL Nuovo filtro]**.
1. Denomina il filtro &quot;Progetti di cui sono Proprietario - Chiusura di questo mese&quot;.
1. Clic **[!UICONTROL Aggiungi regola filtro]**.
1. In [!UICONTROL Inizia a digitare il nome del campo] , digitare &quot;owner&quot;. Quindi seleziona [!UICONTROL ID proprietario] sotto [!UICONTROL Progetto] origine del campo.
1. Lascia [!UICONTROL Uguale] dell&#39;operatore.
1. Digita &quot;$$&quot; nel campo Inizia a digitare il nome.
1. Seleziona [!UICONTROL $$USER.ID]. Carattere jolly per l&#39;utente connesso.
1. Clic [!UICONTROL Aggiungi regola filtro] di nuovo.
1. In [!UICONTROL Inizia a digitare il nome del campo] , inizia a digitare &quot;È completo&quot;. Quindi seleziona [!UICONTROL E&#39; Completo] nel campo Origine progetto.
1. Lascia [!UICONTROL Uguale] dell&#39;operatore.
1. Selezionare &quot;False&quot;.
1. Clic [!UICONTROL Aggiungi regola filtro] di nuovo.
1. In [!UICONTROL Inizia a digitare il nome del campo] tipo di campo &quot;scheduled&quot; (pianificato), quindi seleziona [!UICONTROL Data di completamento Pianificata] sotto [!UICONTROL Progetto] origine del campo.
1. Modificare il [!UICONTROL Uguale] operatore a [!UICONTROL Questo mese].
1. Clic **[!UICONTROL Salva filtro]**
