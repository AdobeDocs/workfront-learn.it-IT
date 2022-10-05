---
title: Trovare e organizzare le risorse in [!UICONTROL Workfront DAM]
description: Scopri come cercare le risorse, eseguire ricerche nelle cartelle, ottimizzare i risultati della ricerca, utilizzare metadati e parole chiave come filtri di ricerca e altro ancora in [!UICONTROL Workfront DAM].
activity: use
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
kt: 8993
exl-id: 28b60118-a471-48bf-ae9b-3a2aed6a6130
source-git-commit: d1f5c4a558f737cb8188e209a16b91b67d32285c
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---

# Collaboratore: trovare risorse

Questo video illustra come:

* Cercare risorse
* Cerca nelle cartelle
* Semplificazione dei risultati di ricerca
* Utilizzare metadati e parole chiave come filtri di ricerca
* Visualizza dettagli cartella
* Visualizzare e aggiornare i metadati e le parole chiave delle risorse

>[!VIDEO](https://video.tv.adobe.com/v/335253/?quality=12)

## Criteri di ricerca di base

Una ricerca di base esamina i nomi dei file, i campi di metadati, le parole chiave e il contenuto della risorsa (a seconda del tipo di risorsa). Non include il nome della cartella.

La maggior parte dei risultati di ricerca sono corrispondenze esatte. Un&#39;eccezione a questa regola di &quot;corrispondenza esatta&quot; è quando [!UICONTROL Workfront DAM] cerca il campo del nome del file. [!UICONTROL Workfront DAM] restituisce corrispondenze parziali del nome file, anziché solo corrispondenze esatte del nome file.

## Operatori utente durante la ricerca

Anche se le funzioni di ricerca di base spesso individuano le risorse necessarie, potrebbe essere necessario utilizzare parametri di ricerca aggiuntivi di tanto in tanto.

### Corrispondenza parziale

Per trovare una corrispondenza parziale, aggiungi un asterisco al termine di ricerca. L&#39;asterisco può essere utilizzato solo alla fine di una parola.

### Operatore AND

Per trovare i risultati contenenti più termini di ricerca, immettere AND tra le parole. Le parole possono essere trovate in qualsiasi ordine. Durante la ricerca in tutti i campi, entrambe le parole potrebbero non essere presenti nello stesso campo. Per esempio, Parigi AND tower troverà risorse che hanno entrambe queste parole in uno qualsiasi dei campi.

### Operatore OR

Utilizza l’operatore OR per trovare le risorse che contengono uno dei termini di ricerca. Ad esempio, Parigi O Arco troveranno risorse che hanno una delle parole, ma non necessariamente entrambe.

### Frase

Per trovare una frase esatta, utilizza virgolette doppie intorno alle parole. Tutte le parole saranno trovate insieme e in ordine. Per esempio, &quot;Torre Eiffel&quot; troverà quelle parole in quell&#39;ordine esatto.

### Operatore negativo

Se si desidera escludere una parola dai risultati della ricerca, mettere un segno meno (-) davanti alla parola. Assicurati che non ci sia uno spazio tra il segno meno e la parola. Ad esempio, per escludere le risorse che contengono la parola &quot;tower&quot; nei metadati, la ricerca può essere impostata come Paris-tower.

### Operatore campo vuoto

Per trovare risorse prive di informazioni in un campo di metadati specifico, immetti il campo da cercare in questo formato: ?[xxxxx]. Ad esempio, per trovare risorse a cui non sono assegnate parole chiave, immetti ?[keyword] nel campo di ricerca.
