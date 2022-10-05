---
title: Creare istruzioni OR nei filtri
description: Con un'istruzione OR, stai dicendo al filtro che desideri visualizzare questo operatore OR.
feature: Reports and Dashboards
thumbnail: create-or-statements-in-filters.png
type: Tutorial
role: User
level: Intermediate
kt: 9987
exl-id: 1a56f2f6-12df-43a5-943c-986a85661efa
source-git-commit: 27e8f0aada77488bd6cfc2e786b997f759fd0a17
workflow-type: tm+mt
source-wordcount: '895'
ht-degree: 0%

---

# Creare istruzioni OR nei filtri

Quando crei un filtro con più linee di criteri, per impostazione predefinita inserisce un valore AND tra ciascuna riga. Questo significa che ogni risultato nell’elenco quando utilizzi questo filtro soddisfa tutte le regole del filtro.

In questo esempio sono disponibili tre criteri o regole per un filtro di progetto:

1. Il progetto deve disporre di una data di completamento pianificata corrispondente al mese corrente.
1. Il progetto deve essere incluso nel portafoglio Eventi Marketing .
1. Il progetto deve essere un progetto attivo, ovvero deve avere lo stato Corrente.

![Immagine della creazione di un filtro con istruzioni AND in [!DNL Workfront]](assets/or-statement-1.png)

I progetti nell’elenco dei risultati soddisfano tutti e tre i criteri, facilitando la riduzione dei risultati della ricerca per visualizzare le informazioni esatte necessarie.

![Immagine di un elenco filtrato in [!DNL Workfront]](assets/or-statement-2.png)

Tuttavia, in alcuni casi può essere utile che i risultati del filtro soddisfino vari criteri, ovvero che le istruzioni OR siano utili. Con un&#39;istruzione OR, stai dicendo al filtro che desideri visualizzare questo operatore OR.

## Uso delle istruzioni OR

Le istruzioni OR espandono o aumentano la quantità di informazioni che il filtro trova perché per essere visualizzate nell&#39;elenco dei risultati, un elemento deve soddisfare solo una delle regole del filtro, non tutte.

Diamo un’occhiata a un’istruzione OR semplice: progetti creati dall’utente come project manager (proprietario) per progetti OR.

![Immagine della creazione di un filtro con istruzioni OR in [!DNL Workfront]](assets/or-statement-3.png)

Dopo aver impostato entrambe le regole di filtro, fai clic sull&#39;AND tra di esse e passa a OR.

![Immagine della creazione di un filtro con istruzioni OR in [!DNL Workfront]](assets/or-statement-4.png)

L’operatore OR tra le due regole di filtro espande i criteri di ricerca, indicando ad Workfront di trovare i progetti che soddisfano una o più di tali opzioni: il tuo nome si trova nel campo proprietario del progetto o sei la persona che ha creato il progetto.

## Più regole di filtro con istruzioni OR

Ora esaminiamo un’istruzione OR che contiene più regole di filtro su ciascun lato dell’OR. Vengono utilizzate le stesse due regole di prima, ma viene aggiunta una regola. I progetti devono avere anche uno stato Corrente.

![Immagine della creazione di un filtro con istruzioni OR in [!DNL Workfront]](assets/or-statement-5.png)

Tieni presente che Workfront ha &quot;raggruppato&quot; le regole di filtro su ciascun lato dell’OR (è presente una casella grigia intorno ad esse). Questo comunica a Workfront di eseguire insieme le regole su ciascun lato dell’OR, individuando progetti che soddisfano entrambi i criteri perché sono uniti con AND.

In questo esempio, Workfront cerca:

* Progetti con il tuo nome nel campo proprietario del progetto che hanno anche lo stato Corrente.
* **PIÙ (O)**
* Progetti creati con uno stato anche Corrente.

Se la regola &quot;stato progetto è uguale a corrente&quot; su ciascun lato dell’OR, la regola funziona insieme a ciascuna delle altre regole. Questa regola comune è a volte indicata come &quot;costante&quot;.

>[!NOTE]
>
>Non sei limitato a una regola di filtro ripetuta su ciascun lato dell&#39;operatore OR. A seconda delle tue esigenze, potresti averne diverse. Workfront consiglia di mantenere al minimo queste regole ripetute, per garantire che il filtro fornisca i risultati necessari.

## Cosa succede senza la regola di filtro comune?

Senza le regole di filtro comuni, è possibile che non si ottengano i risultati di ricerca previsti.

Ad esempio, se metti la regola &quot;stato progetto uguale a corrente&quot; solo su un lato dell’OR, funziona solo con le altre regole di filtro in quella sezione. Nell’immagine seguente, la regola &quot;stato progetto è uguale a corrente&quot; si trova solo nella sezione superiore.

![Immagine della creazione di un filtro con istruzioni OR in [!DNL Workfront]](assets/or-statement-6.png)

Ciò significa che Workfront cercherà:

* Progetti con il tuo nome nel campo relativo al proprietario del progetto e con lo stato Corrente.
* **PIÙ (O)**
* Tutti i progetti creati.

Come puoi vedere, questa configurazione del filtro fornisce risultati leggermente diversi rispetto al filtro con la regola di filtro ripetuta. Per questo motivo è importante assicurarsi che il filtro sia configurato correttamente per ottenere i risultati desiderati e necessari.

Non è possibile utilizzare frequentemente le istruzioni OR durante la creazione di filtri. Tuttavia, così facendo potresti ridurre il numero di filtri necessari. Assicurati semplicemente che i filtri non restituiscano troppi risultati: una lista lunga può rendere più difficile trovare le informazioni esatte necessarie per gli utenti.

## Attività filtro OR

Individuare attività incomplete assegnate a te o non assegnate a nessuno. Imposta un filtro come quello sottostante. Questo filtro ti darà i risultati desiderati? Perché o perché no?

![Immagine di un&#39;istruzione OR creata in modo errato in [!DNL Workfront]](assets/or-statement-your-turn-1.png)

### Risposte

No, questo filtro non fornirà i risultati sperati, ovvero le attività non completate che sono state assegnate a te o a nessuno, perché la regola di filtro per lo stato dell&#39;attività si trova solo su un lato dell&#39;OR.

Questo filtro genera invece un elenco che mostra:

* Attività assegnate all&#39;utente con stato In corso o Nuovo.
* **PIÙ (O)**
* Tutte le attività non assegnate, indipendentemente dallo stato.

Il filtro deve essere simile a quello sottostante. Nota che questo filtro ha la regola di filtro per lo stato dell&#39;attività su entrambi i lati dell&#39;operatore OR.

![Immagine di un&#39;istruzione OR creata correttamente in [!DNL Workfront]](assets/or-statement-your-turn-2.png)
