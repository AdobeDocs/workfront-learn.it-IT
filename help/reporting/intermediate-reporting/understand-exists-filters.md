---
title: Comprendere i filtri EXISTS
description: Scopri cos’è un filtro EXISTS, cosa può fare per te e come crearne uno da zero. Inoltre vedi molti utili esempi di filtri EXISTS.
activity: use
team: Technical Marketing
feature: Reports and Dashboards
type: Tutorial
role: User
level: Intermediate
jira: KT-1880
last-substantial-update: 2025-08-25T00:00:00Z
doc-type: video
source-git-commit: 7be0b8cce9cba04927d6704d0009b482bbcf4b41
workflow-type: tm+mt
source-wordcount: '682'
ht-degree: 0%

---

# Comprendere i filtri EXISTS

I filtri EXISTS sono filtri avanzati in modalità testo, che ci consentono di aggirare il limite di 2 salti di tabella/campo in un generatore di rapporti standard. In alternativa, possono essere utilizzati per identificare gli oggetti nel sistema che non dispongono di una condizione di relazione specifica tramite NOTEXISTS.

Questo video illustra come creare un filtro EXISTS per visualizzare &quot;Approvazioni bozza su progetti correnti&quot; in un rapporto sulle approvazioni bozza.

Per informazioni dettagliate sulla funzione EXISTS, vedere [Creare filtri in modalità testo complessi utilizzando istruzioni EXISTS](https://experienceleague.adobe.com/it/docs/workfront/using/reporting/reports/text-mode/create-complex-text-mode-filters-using-exists-statements).

>[!VIDEO](https://video.tv.adobe.com/v/3471211/?quality=12&learn=on&enablevpops&captions=ita)

## Esempi di filtro EXISTS

### Report di progetto ESISTENTE

In questo modo l&#39;attività viene utilizzata come oggetto di collegamento, confrontando il projectID trovato a livello di attività e confrontandolo con il campo ID a livello di progetto. Questo consente di confrontare gli utenti dell’assegnazione sull’attività con un carattere jolly $$USER.ID. In questo modo vengono restituiti solo i progetti a cui l’utente che li visualizza è assegnato.
attività, indipendentemente dal fatto che siano o meno l’assegnatario principale.

```
EXISTS:A:$$OBJCODE=TASK
EXISTS:A:assignmentsUsersMM:ID=$$USER.ID
EXISTS:A:assignmentsUsersMM:ID_Mod=in
EXISTS:A:projectID=FIELD:ID
```


In questo modo viene utilizzato il problema (optask) come oggetto di collegamento, confrontando anche il projectID trovato a livello di problema (optask) e confrontandolo con il campo ID a livello di progetto. Questo controlla quindi se uno di questi problemi (optasks) ha una data di ingresso entro l&#39;intervallo specificato. In questo caso restituirebbe qualsiasi progetto che abbia
nessun problema (optask) registrato negli ultimi 30 giorni, a causa di NOTEXISTS.

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=OPTASK
EXISTS:A:entryDate=$$TODAY
EXISTS:A:entryDate_Mod=between
EXISTS:A:entryDate_Range=$$TODAY-30d
EXISTS:A:projectID=FIELD:ID
```

### Report modello ESISTENTE

Questo filtro mostra tutti i modelli che non sono stati utilizzati per creare un progetto o che sono stati allegati a un progetto nell’ultimo anno. Un&#39;avvertenza è che per capire se un modello è stato utilizzato o meno come allegato, dipende da tale modello che contiene attività.

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=TASK
EXISTS:A:entryDate=$$TODAY-1y
EXISTS:A:entryDate_Mod=gte
EXISTS:A:templateTask:templateID=FIELD:ID
EXISTS:B:$$EXISTSMOD=NOTEXISTS
EXISTS:B:$$OBJCODE=PROJ
EXISTS:B:entryDate=$$TODAY-1y
EXISTS:B:entryDate_Mod=gte
EXISTS:B:templateID=FIELD:ID
```

### Rapporto attività ESISTENTE

In questo modo viene utilizzata la tabella User come oggetto di collegamento, che si connette tramite l&#39;ID attività assegnazioni e l&#39;ID attività. Questa controlla quindi l’insieme di ID dei team agli ID del team utente, restituendo l’attività se uno qualsiasi degli assegnatari si trova nello stesso team dell’utente che visualizza l’ID.

```
EXISTS:1:$$OBJCODE=USER
EXISTS:1:teams:ID=$$USER.teamIDs
EXISTS:1:userAssignments:taskID=FIELD:ID
```

### Report utente ESISTENTE

Verranno restituiti tutti gli utenti che non hanno pubblicato un aggiornamento nelle ultime 3 settimane. In questo modo viene utilizzato l&#39;oggetto note per colmare il gap e viene confrontato l&#39;ID proprietario con un ID utente. Restituisce quindi l’utente se nessuna nota di sua proprietà ha una data di ingresso superiore a 3 settimane fa.

```
EXISTS:A:$$OBJCODE=NOTE
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:ownerID=FIELD:ID
EXISTS:A:entryDate=$$TODAY-3w
EXISTS:A:entryDate_Mod=gt
```

Verranno restituiti tutti gli utenti che non hanno registrato ore nell’ultima settimana. Questo utilizza un metodo estremamente simile all’esempio precedente, ma utilizza le informazioni sul proprietario delle ore e la data di immissione delle ore per determinare gli utenti restituiti.

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=HOUR
EXISTS:A:entryDate=$$TODAY-1w
EXISTS:A:entryDate_Mod=gte
EXISTS:A:ownerID=FIELD:ID
```

In un report utenti, mostra un elenco di utenti che corrisponde alla scheda Persone di un progetto.

```
EXISTS:1:$$OBJCODE=PRTU
EXISTS:1:projectID=<projectID>
EXISTS:1:userID=FIELD:ID
```

### Report categoria (modulo personalizzato) ESISTENTE

Questo testo ti fornirà un elenco di tutti i moduli di progetto che non sono mai stati utilizzati in un progetto. Questo deve essere utilizzato insieme a specificare il tipo di oggetto del modulo su cui ci concentriamo. In questo caso, l&#39;elemento attivo è PROJ, quindi è necessario includere le didascalie nelle righe objTypes. Questo potrebbe essere utilizzato
per altri tipi di oggetto modificando le parti correlate al codice oggetto. In questo modo viene controllata la raccolta di progetti allegati ai moduli elencati e viene restituita una corrispondenza, se non esiste.

```
EXISTS:A:$$OBJCODE=PROJ
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:objectCategories:categoryID=FIELD:ID
objTypes=PROJ
objTypes_Mod=in
```

### Report parametro (campo personalizzato) ESISTENTE

Restituisce qualsiasi campo personalizzato non attualmente associato a un modulo personalizzato nel sistema.

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=CTGYPA
EXISTS:A:parameterID=FIELD:ID
```

### Report già esistente

Questo restituirà qualsiasi rapporto che utilizza un valore specifico nei suoi filtri.

```
EXISTS:1:$$OBJCODE=UIFT
EXISTS:1:ID=FIELD:filterID
EXISTS:1:preference:value=<value here>
EXISTS:1:preference:value_Mod=cicontains
```

Questo restituirà qualsiasi rapporto allegato a qualsiasi dashboard.

```
EXISTS:A:$$OBJCODE=PRTBSC
EXISTS:A:internalSectionID=FIELD:ID
EXISTS:A:portalTab:ID_Mod=notblank
```

### Rapporto Approvazione bozza ESISTENTE

In questo modo le approvazioni delle bozze vengono restituite solo ai progetti con lo stato Attuale. Viene utilizzato l&#39;oggetto Document per colmare il gap tra l&#39;approvazione della bozza e il progetto verificando currentVersionID e documentVersionID, da qui si passa allo stato dei progetti.

```
EXISTS:1:$$OBJCODE=DOCU
EXISTS:1:currentVersionID=FIELD:documentVersionID
EXISTS:1:project:status=CUR
EXISTS:1:project:status_Mod=in
```
