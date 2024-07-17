---
title: Creare istruzioni OR nei filtri
description: Scopri come utilizzare un’istruzione OR per comunicare a Workfront che desideri visualizzare tale OR nel rapporto.
activity: use
team: Technical Marketing
feature: Reports and Dashboards
thumbnail: create-or-statements-in-filters.png
type: Tutorial
role: User
level: Intermediate
jira: KT-9987
exl-id: 1a56f2f6-12df-43a5-943c-986a85661efa
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '915'
ht-degree: 100%

---

# Creare istruzioni OR nei filtri

Quando crei un filtro con più righe di criteri, per impostazione predefinita Workfront inserisce un AND tra ogni riga. Ciò significa che ogni risultato nell’elenco quando utilizzi questo filtro soddisfa tutte le regole del filtro.

In questo esempio, sono disponibili tre criteri, o regole, per un filtro di progetto:

1. Il progetto deve avere una data di completamento pianificata che cade nel mese corrente.
1. Il progetto deve trovarsi nel portfolio Marketing degli eventi.
1. Il progetto deve essere attivo, ovvero avere lo stato Attuale.

![Immagine della creazione di un filtro con istruzioni AND in [!DNL Workfront]](assets/or-statement-1.png)

I progetti nell’elenco dei risultati soddisfano tutti e tre questi criteri, che consentono di limitare i risultati della ricerca in modo da visualizzare le informazioni esatte necessarie.

![Immagine di un elenco filtrato in [!DNL Workfront]](assets/or-statement-2.png)

Tuttavia, in alcuni casi potrebbe essere utile che i risultati del filtro soddisfino vari criteri ed è qui che le istruzioni OR possono essere utili. Con un’istruzione OR, stai dicendo al filtro che desideri visualizzare elementi che corrispondono a UNA QUALSIASI delle tue istruzioni OR, anziché TUTTE le tue istruzioni AND.

## Utilizzo delle istruzioni OR

Le istruzioni OR espandono o aumentano la quantità di informazioni trovate dal filtro perché, per essere visualizzato nell’elenco dei risultati, un elemento deve soddisfare solo una delle regole del filtro, non tutte.

Diamo un’occhiata a una semplice istruzione OR: i progetti di cui sei il project manager (proprietario) sono progetti OR creati da te.

![Immagine della creazione di un filtro con istruzioni OR in [!DNL Workfront]](assets/or-statement-3.png)

Dopo aver impostato entrambe le regole di filtro, fai clic sull’operatore AND tra le due e impostalo su OR.

![Immagine della creazione di un filtro con istruzioni OR in [!DNL Workfront]](assets/or-statement-4.png)

L’operatore OR tra le due regole di filtro espande i criteri di ricerca, indicando a Workfront di trovare i progetti che soddisfano una o l’altra di tali opzioni: il tuo nome si trova nel campo proprietario del progetto o sei la persona che ha creato il progetto.

## Più regole di filtro con istruzioni OR

Ora esaminiamo un’istruzione OR che contiene più regole di filtro su ciascun lato dell’operatore OR. In questo modo vengono utilizzate le stesse due regole precedenti, ma viene aggiunta una regola. Anche i progetti devono avere lo stato Corrente.

![Immagine della creazione di un filtro con istruzioni OR in [!DNL Workfront]](assets/or-statement-5.png)

Nota che Workfront ha “raggruppato” le regole del filtro su ciascun lato dell’operatore OR (attorno a esse è presente una casella grigia). Questo indica a Workfront di eseguire insieme le regole su ciascun lato dell’operatore OR, trovando progetti che soddisfino entrambi questi criteri perché sono uniti con l’operatore AND.

In questo esempio, Workfront cerca:

* I progetti il cui nome è indicato nel campo proprietario del progetto e che hanno anche lo stato Corrente.
* **PIÙ (OR)**
* Progetti creati che hanno anche lo stato Corrente.

Se si imposta la regola “Stato progetto uguale a Corrente” su ciascun lato dell’operatore OR, la regola funziona in combinazione con ciascuna delle altre regole. Questa regola comune è a volte indicata come la “costante”.

>[!NOTE]
>
>Non sei limitato a una regola di filtro ripetuta su ciascun lato dell’operatore OR. A seconda delle tue esigenze, potresti averne più di una. Workfront consiglia di mantenere queste regole ripetute al minimo, per garantire che il filtro fornisca i risultati necessari.

## Cosa succede senza la regola di filtro comune?

Senza le regole di filtro comuni, è possibile che non si ottengano i risultati di ricerca previsti.

Ad esempio, se inserisci la regola “Lo stato del progetto è uguale a Corrente” solo su un lato dell’operatore OR, questa funziona solo con le altre regole di filtro in quella sezione. Nell’immagine seguente, puoi vedere che la regola “Stato del progetto è uguale a corrente” è presente solo nella sezione superiore.

![Immagine della creazione di un filtro con istruzioni OR in [!DNL Workfront]](assets/or-statement-6.png)

Ciò significa che Workfront cercherà:

* Progetti che hanno il tuo nome nel campo proprietario del progetto e lo stato Attuale.
* **PIÙ (OR)**
* Tutti i progetti creati.

Come puoi vedere, questa impostazione del filtro fornisce risultati leggermente diversi rispetto al filtro con la regola del filtro ripetuto. Per questo motivo è importante assicurarsi che il filtro sia configurato correttamente per ottenere i risultati desiderati e necessari.

Non è possibile utilizzare frequentemente le istruzioni OR durante la creazione dei filtri. In questo modo, però, potresti ridurre il numero di filtri da creare. Assicurati solo che i filtri non restituiscano troppi risultati: un elenco lungo può rendere più difficile trovare le informazioni esatte necessarie per gli utenti.

## Attività filtro OR

Desideri trovare attività incomplete che ti sono state assegnate o che non sono state assegnate a nessuno. Hai impostato un filtro simile a quello riportato di seguito. Questo filtro ti darà i risultati desiderati? Perché sì o perché no?

![Immagine di un’istruzione OR creata in modo non corretto in [!DNL Workfront]](assets/or-statement-your-turn-1.png)

### Risposte

No, questo filtro non fornirà i risultati desiderati, ovvero le attività che non sono state completate e che sono state assegnate a te o a nessuno, perché la regola del filtro per lo stato dell’attività si trova solo su un lato dell’operatore OR.

Al contrario, questo filtro genera un elenco che mostra:

* Attività assegnate con stato In corso o Nuovo.
* **PIÙ (OR)**
* Tutte le attività non assegnate, indipendentemente dallo stato.

Il filtro deve essere simile a quello riportato di seguito. Questo filtro ha la regola di filtro per lo stato dell’attività su entrambi i lati dell’operatore OR.

![Immagine di un’istruzione OR creata correttamente in [!DNL Workfront]](assets/or-statement-your-turn-2.png)
