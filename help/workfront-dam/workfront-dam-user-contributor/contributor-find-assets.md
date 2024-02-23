---
title: Comprendere la ricerca di risorse come collaboratore
description: Scopri come cercare le risorse, cercare all’interno delle cartelle, semplificare i risultati di ricerca, utilizzare metadati e parole chiave come filtri di ricerca in [!UICONTROL DAM WORKFRONT].
activity: use
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8993
exl-id: 28b60118-a471-48bf-ae9b-3a2aed6a6130
doc-type: video
source-git-commit: 2cb3cc67f4f1fcd1345f178bf525d7b00f6271cf
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 90%

---

# Comprendere la ricerca di risorse come collaboratore

In questo video scoprirai come:

* Cercare le risorse
* Cercare all’interno delle cartelle
* Semplificare i risultati di ricerca
* Utilizzare metadati e parole chiave come filtri di ricerca
* Visualizzare i dettagli cartella
* Visualizzare e aggiornare i metadati e le parole chiave delle risorse

>[!VIDEO](https://video.tv.adobe.com/v/335253/?quality=12&learn=on)

## Criteri di ricerca di base

Una ricerca di base esamina nomi di file, campi di metadati, parole chiave e contenuto delle risorse (a seconda del tipo di risorsa). Non include il nome della cartella.

La maggior parte dei risultati della ricerca è costituita da corrispondenze esatte. Un’eccezione a questa regola di &quot;corrispondenza esatta&quot; si verifica quando il [!UICONTROL DAM WORKFRONT] cerca nel campo nome file. [!UICONTROL Workfront DAM] restituisce corrispondenze parziali del nome del file, anziché corrispondenze esatte.

## Utilizzo degli operatori durante la ricerca

Anche se le funzioni di ricerca di base spesso sono in grado di individuare le risorse necessarie, in alcuni casi potrebbe essere necessario utilizzare parametri di ricerca aggiuntivi.

### Corrispondenze parziali

Per trovare una corrispondenza parziale, aggiungi un asterisco al termine di ricerca. L’asterisco può essere utilizzato solo alla fine di una parola.

### Operatore AND

Per trovare risultati contenenti più termini di ricerca, inserisci AND tra le parole. Le parole possono essere trovate in qualsiasi ordine. Durante una ricerca in tutti i campi, è possibile che nello stesso campo non siano presenti entrambe le parole. Ad esempio, Parigi AND torre restituiranno risorse che contengono entrambe queste parole in qualsiasi campo.

### Operatore OR

Utilizza l’operatore OR per trovare le risorse che contengono uno qualsiasi dei termini di ricerca. Ad esempio, Parigi OR Arco restituirà risorse che contengono una delle due parole, ma non necessariamente entrambe.

### Frase

Per trovare una frase esatta, racchiudila tra virgolette. Tutte le parole saranno trovate insieme e in ordine. Ad esempio, la ricerca di “Torre Eiffel” troverà quelle parole in quell’ordine esatto.

### Operatore negativo

Se desideri escludere una parola dai risultati della ricerca, inserisci un segno meno (–) davanti alla parola. Assicurati che non vi sia uno spazio tra il segno meno e la parola. Ad esempio, per escludere le risorse i cui metadati contengono la parola “torre”, la ricerca può essere impostata come Parigi -torre.

### Operatore campo vuoto

Per trovare risorse prive di informazioni in un campo di metadati specifico, inserisci il campo in cui desideri eseguire la ricerca usando questo formato: ?[xxxxx]. Ad esempio, se desideri trovare risorse alle quali non sono state assegnate parole chiave, immetti ?[parola chiave] nel campo di ricerca.
