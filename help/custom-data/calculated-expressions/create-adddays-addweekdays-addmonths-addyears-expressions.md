---
title: Creare espressioni ADDDAYS, ADDWEEKDAY, ADDMONTHS, ADDYEARS
description: Scopri come utilizzare e creare le espressioni ADD in un campo calcolato in Adobe [!DNL Workfront].
feature: System Setup and Administration
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: 335175.png
kt: 8912
exl-id: f194fbc8-99b3-4fed-9fc5-a2f5fa4593d2
doc-type: video
source-git-commit: 650e4d346e1792863930dcebafacab4c88f2a8bc
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---

# Creare espressioni ADDDAYS, ADDWEEKDAY, ADDMONTHS, ADDYEARS

In questo video imparerai:

* Calcolo delle espressioni ADDDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR
* Come creare un&#39;espressione di dati ADDWEEKDAYS in un campo calcolato

>[!VIDEO](https://video.tv.adobe.com/v/335175/?quality=12&learn=on)

## Esempi aggiuntivi

Di seguito sono riportate alcune espressioni aggiuntive ADDDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR create dai clienti Adobe Workfront.

**Dovrebbe essere stato fatto da**

Il cliente desiderava sapere quando l&#39;attività doveva essere stata completata in base alla data di inizio effettiva e alla durata prevista. La data di completamento prevista non funziona in questo caso perché può essere spostata se l&#39;attività è in ritardo e la data di completamento pianificata non aiuta in caso di ritardi nelle attività precedenti.

L&#39;espressione creata è ADDDAYS({effectiveStartDate},{durationMinutes}/480)

Il tempo nel campo Durata viene memorizzato in minuti. Pertanto, in questa espressione, il campo Duration non può restare da solo se l’ora deve essere riflessa in giorni. Affinché ciò accada, la durata deve essere divisa per 480 minuti (480 minuti = 8 ore = 1 giorno)

Questo è il motivo per cui lo slot del secondo valore contiene (Duration/480).


**Data completamento fattura**

Questo esempio include non solo l’espressione ADDDAYS, ma anche un campo personalizzato creato e salvato precedentemente nel modulo personalizzato.

Il cliente sta acquisendo la data di invio di una fattura tramite un campo di data personalizzato denominato &quot;Data di invio della fattura&quot;.

Una volta inoltrata, la fattura deve essere compilata e depositata entro 30 giorni. Per produrre automaticamente la data di completamento e di deposito, viene utilizzato un campo calcolato ADDDAYS insieme al campo personalizzato &quot;Data invio fattura&quot;. L&#39;espressione si presenta così:

ADDDAYS({DE:Data di invio fattura},30)
