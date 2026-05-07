---
title: Comprendere la ricerca di risorse come collaboratore
description: Scopri come cercare le risorse, cercare all’interno delle cartelle, semplificare i risultati di ricerca, utilizzare i metadati e le parole chiave come filtri di ricerca in [!UICONTROL Workfront DAM].
activity: use
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8993
exl-id: 28b60118-a471-48bf-ae9b-3a2aed6a6130
doc-type: video
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-05T20:25:54.114Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 407
ht-degree: 89%

---

# Comprendere la ricerca di risorse come collaboratore

In questo video scoprirai come:

* Cercare le risorse
* Cercare all’interno delle cartelle
* Semplificare i risultati di ricerca
* Utilizzare metadati e parole chiave come filtri di ricerca
* Visualizzare i dettagli cartella
* Visualizzare e aggiornare i metadati e le parole chiave delle risorse

>[!VIDEO](https://video.tv.adobe.com/v/3453930/?captions=ita&quality=12&learn=on&enablevpops=1)

## Criteri di ricerca di base

Una ricerca di base esamina nomi di file, campi di metadati, parole chiave e contenuto delle risorse (a seconda del tipo di risorsa). Non include il nome della cartella.

La maggior parte dei risultati della ricerca è costituita da corrispondenze esatte. Un’eccezione a questa regola della “corrispondenza esatta” si verifica quando [!UICONTROL Workfront DAM] esegue la ricerca nel campo del nome del file. [!UICONTROL Workfront DAM] restituisce corrispondenze parziali del nome del file, anziché corrispondenze esatte.

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

Per trovare le risorse prive di informazioni in un campo di metadati specifico, immettere il campo che si desidera cercare in questo formato: ?[xxxxx]. Ad esempio, se desideri trovare risorse alle quali non sono state assegnate parole chiave, immetti ?[parola chiave] nel campo di ricerca.
