---
title: Creare filtri con caratteri jolly basati sull’utente
description: Scopri come utilizzare i caratteri jolly e creare un filtro con un carattere jolly basato sull’utente in [!DNL  Workfront].
activity: use
feature: Reports and Dashboards
thumbnail: 336810.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 9081
exl-id: 46c83acd-6e43-42aa-875f-ae24b09a7fee
source-git-commit: 83c7379a5398c78cea31a4571b34fd5b64bce027
workflow-type: tm+mt
source-wordcount: '336'
ht-degree: 0%

---

# Creare filtri con caratteri jolly basati sull’utente

Questo video illustra come:

* Scopri perché utilizzare i caratteri jolly
* Creare un filtro con un carattere jolly basato sull’utente

>[!VIDEO](https://video.tv.adobe.com/v/336810/?quality=12)

>[!TIP]
>
>Utilizzare l&#39;origine e il nome del campo Assegnazione utenti >> ID durante la creazione di filtri per esaminare le informazioni sull&#39;assegnazione di attività o problemi.  Questa opzione esamina tutti gli utenti assegnati all’attività o al problema, non solo il &quot;proprietario&quot; o l’assegnatario principale.

>[!TIP]
>
>Utilizza il $$USER.ID (invece del tuo nome) anche quando crei filtri per te stesso. In questo modo, se qualcuno vede un filtro che stai utilizzando e dice &quot;condividi con me&quot;, il filtro è già configurato in modo che ogni persona che lo utilizza veda le proprie informazioni.

>[!TIP]
>
>È sempre necessario utilizzare il qualificatore di filtro Equal quando si utilizzano caratteri jolly basati sull&#39;utente.

## Attività

Hai un po&#39; di tempo in più questa settimana, quindi vuoi vedere se c&#39;è qualcuno del tuo team che potrebbe usare dell&#39;assistenza per i loro compiti. Crea un filtro attività per individuare le attività che scadono questa settimana e che non sono state completate.

## Risposta

Sei fantastico per aver aiutato i tuoi compagni di squadra! Con il filtro impostato come nell&#39;immagine seguente, troverai le attività:

* Non è stato completato (ovvero non dispone di un [!UICONTROL Completa] stato o stato che equivale a [!UICONTROL Completa]);
* Nei progetti con un [!UICONTROL Corrente] stato (dopo tutto, non vuoi trovare attività per progetti che non sono ancora stati avviati);
* che sono assegnati a un utente del team di casa, come definito dalle impostazioni del team Workfront;
* E che hanno una data di completamento questa settimana (questa regola ha utilizzato il filtro data predefinito per definire &quot;questa settimana&quot;).

![Immagine della schermata per creare un filtro attività con un carattere jolly basato sull’utente](assets/user-wildcard-exercise-answer.png)

Potrebbe essere necessario aggiungere altri filtri se è necessario limitare un po&#39; di più l’elenco. Ad esempio, puoi aggiungere una regola di filtro per esaminare un programma o un portfolio specifico di cui il team si occupa.
