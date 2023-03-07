---
title: Trovare e organizzare le risorse in [!UICONTROL DAM WORKFRONT]
description: Scopri come cercare le risorse, cercare all’interno delle cartelle, semplificare i risultati di ricerca, utilizzare metadati e parole chiave come filtri di ricerca e altro ancora in [!UICONTROL DAM WORKFRONT].
activity: use
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
kt: 8993
exl-id: 28b60118-a471-48bf-ae9b-3a2aed6a6130
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---

# Collaboratore: trovare le risorse

Questo video illustra come:

* Cercare le risorse
* Cerca nelle cartelle
* Semplificare i risultati della ricerca
* Utilizzare metadati e parole chiave come filtri di ricerca
* Visualizza dettagli cartella
* Visualizzare e aggiornare i metadati e le parole chiave delle risorse

>[!VIDEO](https://video.tv.adobe.com/v/335253/?quality=12)

## Criteri di ricerca di base

Una ricerca di base esamina i nomi dei file, i campi di metadati, le parole chiave e il contenuto delle risorse (a seconda del tipo di risorsa). Non include il nome della cartella.

La maggior parte dei risultati di ricerca sono corrispondenze esatte. Un’eccezione a questa regola di &quot;corrispondenza esatta&quot; si verifica quando il [!UICONTROL DAM WORKFRONT] cerca nel campo nome file. [!UICONTROL DAM WORKFRONT] restituisce corrispondenze parziali del nome file, anziché corrispondenze esatte del nome file.

## Operatori utente durante la ricerca

Anche se le funzioni di ricerca di base spesso individuano le risorse necessarie, potrebbe essere necessario utilizzare parametri di ricerca aggiuntivi di tanto in tanto.

### Corrispondenza parziale

Per trovare una corrispondenza parziale, aggiungi un asterisco al termine di ricerca. L&#39;asterisco può essere utilizzato solo alla fine di una parola.

### Operatore AND

Per trovare risultati contenenti più termini di ricerca, immettere AND tra le parole. Le parole possono essere trovate in qualsiasi ordine. Durante la ricerca in tutti i campi, entrambe le parole potrebbero non essere presenti nello stesso campo. Ad esempio, Paris AND Tower troverà risorse che contengono entrambe queste parole in qualsiasi campo.

### Operatore OR

Utilizza l’operatore OR per trovare le risorse che contengono uno dei termini di ricerca. Ad esempio, Paris OR Arc troverà le risorse che hanno una delle due parole, ma non necessariamente entrambe.

### Frase

Per trovare una frase esatta, racchiuderla tra virgolette. Tutte le parole saranno trovate insieme e in ordine. Per esempio, &quot;Torre Eiffel&quot; troverà quelle parole nell&#39;ordine esatto.

### Operatore negativo

Se si desidera escludere una parola dai risultati della ricerca, inserire un segno meno (-) davanti alla parola. Assicurati che non vi sia uno spazio tra il segno meno e la parola. Ad esempio, per escludere le risorse i cui metadati contengono la parola &quot;tower&quot;, la ricerca potrebbe essere impostata come Paris -tower.

### Operatore campo vuoto

Per trovare le risorse prive di informazioni in un campo di metadati specifico, inserisci il campo in cui desideri eseguire la ricerca in questo formato: ?[xxxxx]. Ad esempio, se desideri trovare risorse alle quali non sono state assegnate parole chiave, immetti ?[parola chiave] nel campo di ricerca.
