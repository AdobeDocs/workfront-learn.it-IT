---
title: Creare le espressioni ADDDAYS, ADDWEEKDAY, ADDMONTHS, ADDYEARS
description: Scopri come utilizzare e creare le espressioni ADD in un campo calcolato in Adobe  [!DNL Workfront].
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
TQID: https://experienceleague.adobe.com/22KjuMtDdhm9A6JohWlThfOHwKcegLwT3nuFO--70N4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: f8a45b24-4be7-4f1b-909b-60d06b483a20
source-git-commit: 36674ed53c8645f556862bb2d99f3bfd6c993c1e
workflow-type: tm+mt
source-wordcount: 275
ht-degree: 97%

---

# Creare le espressioni ADDDAYS, ADDWEEKDAY, ADDMONTHS, ADDYEARS

In questo video scoprirai:

* Calcolo delle espressioni ADDDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR
* Creare un’espressione dati ADDWEEKDAYS in un campo calcolato

>[!VIDEO](https://video.tv.adobe.com/v/335175/?quality=12&learn=on&enablevpops=1)

## Altri esempi

Di seguito sono riportate alcune espressioni ADDDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR aggiuntive create dalla clientela di di Adobe Workfront.

**L’operazione avrebbe dovuto essere completata entro**

Il cliente desiderava sapere quando l’attività avrebbe dovuto essere completata in base alla data di inizio effettiva e alla durata pianificata. In questo caso, la data di completamento prevista non funzionerà perché può essere spostata se l’attività è in ritardo e la data di completamento pianificata non aiuta se ci sono ritardi nelle attività precedenti.

L&#39;espressione creata è ADDDAYS({actualStartDate},{durationMinutes}/480)

Il tempo nel campo Durata viene memorizzato in minuti. Pertanto, in questa espressione, il campo Durata non può essere autonomo se il tempo deve essere espresso in giorni. Affinché ciò accada, la Durata deve essere divisa per 480 minuti (480 minuti = 8 ore = 1 giorno)

Per questo motivo il secondo slot di valori contiene (Durata/480).


**Data di completamento fattura**

Questo esempio include non solo l’espressione ADDDAYS, ma anche un campo personalizzato creato e salvato in precedenza nel modulo personalizzato.

Il cliente acquisisce la data di invio di una fattura mediante un campo data personalizzato denominato “Data di invio fattura”.

Dopo l’invio, la fattura dovrà essere compilata e archiviata entro 30 giorni. Per generare automaticamente la data di completamento e archiviazione, viene utilizzato un campo calcolato ADDDAYS insieme al campo personalizzato “Data invio fattura”. L’espressione si presenta così:

ADDDAYS({DE:Invoice Submission Date},30)
