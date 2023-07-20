---
title: Creare espressioni ADDDAYS, ADDWEEKDAY, ADDMONTHS, ADDYEARS
description: Scopri come utilizzare e creare le espressioni ADD in un campo calcolato in Adobe [!DNL Workfront].
feature: Custom Forms
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: 335175.png
jira: KT-8912
exl-id: f194fbc8-99b3-4fed-9fc5-a2f5fa4593d2
doc-type: video
source-git-commit: 409147f9a62302d28e14b834981992a0421d4e4b
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---

# Creare espressioni ADDDAYS, ADDWEEKDAY, ADDMONTHS, ADDYEARS

Questo video illustra:

* Calcolo delle espressioni ADDDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR
* Creare un&#39;espressione dati ADDWEEKDAYS in un campo calcolato

>[!VIDEO](https://video.tv.adobe.com/v/335175/?quality=12&learn=on)

## Altri esempi

Di seguito sono riportate alcune espressioni ADDDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR aggiuntive create dai clienti Adobe Workfront.

**L&#39;operazione avrebbe dovuto essere eseguita da**

Il cliente desiderava sapere quando l&#39;attività avrebbe dovuto essere completata in base alla data di inizio effettiva e alla durata pianificata. La data di completamento prevista non funzionerà in questo caso perché può essere spostata se l&#39;attività è in ritardo e la data di completamento pianificata non aiuta se ci sono ritardi nelle attività precedenti.

L’espressione creata era ADDDAYS({actualStartDate},{durationMinutes}/480)

Il tempo nel campo Durata viene memorizzato in minuti. Pertanto, in questa espressione, il campo Durata non può essere autonomo se il tempo deve essere espresso in giorni. Affinché ciò accada, la Durata deve essere divisa per 480 minuti (480 minuti = 8 ore = 1 giorno)

Per questo motivo il secondo slot di valori contiene (Durata/480).


**Data di completamento fattura**

Questo esempio include non solo l&#39;espressione ADDDAYS, ma anche un campo personalizzato creato e salvato in precedenza nel modulo personalizzato.

Il cliente acquisisce la data di invio di una fattura mediante un campo data personalizzato denominato &quot;Data di invio fattura&quot;.

Dopo l&#39;invio, la fattura deve essere compilata e compilata entro 30 giorni. Per generare automaticamente il completamento e la data di archiviazione, viene utilizzato un campo calcolato ADDDAYS insieme al campo personalizzato &quot;Data invio fattura&quot;. L’espressione si presenta così:

ADDDAYS({DE:Data di invio fattura},30)
