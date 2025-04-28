---
title: Comprendere i componenti di reporting
description: I componenti di reporting di Workfront perfezionano la visualizzazione dei dati con filtri basati su oggetti, viste dinamiche, raggruppamenti strutturati e funzionalità con caratteri jolly per ottenere informazioni personalizzate.
activity: use
feature: Reports and Dashboards
thumbnail: 335146.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8850
exl-id: e9f9ba24-540f-49e1-ac52-740df489317b
doc-type: video
source-git-commit: 83382bc990fb6e3e39a8f858d3710cce14179a95
workflow-type: tm+mt
source-wordcount: '533'
ht-degree: 42%

---

# Comprendere i componenti di reporting

Il video illustra il concetto dei componenti di reporting di Workfront, essenziali per la creazione di filtri, visualizzazioni e raggruppamenti. I componenti chiave includono:

* **Tipo di oggetto:** Specifica l&#39;oggetto Workfront che viene gestito, ad esempio un progetto, un&#39;attività o un&#39;ora. &#x200B; I filtri, le visualizzazioni e i raggruppamenti sono specifici per il tipo di oggetto. &#x200B;
* **Source campo e nome campo:** L&#39;origine campo è l&#39;elemento in Workfront a cui sono allegate le informazioni e il nome campo è l&#39;informazione specifica (ad esempio, &quot;descrizione&quot; per un progetto). &#x200B;
* **Campo valore:** Rappresenta il contenuto di un campo, ad esempio &quot;low&quot;, &quot;normal&quot;, &quot;high&quot; o &quot;urgent&quot; per il campo priorità. &#x200B;
* **Qualificatore filtro:** definisce quali valori includere o escludere in un report, ad esempio le attività con priorità &quot;alta&quot;. &#x200B;


>[!VIDEO](https://video.tv.adobe.com/v/335146/?quality=12&learn=on)

## Punti chiave da eliminare

* **Componenti di reporting:** i componenti di reporting di Workfront includono il tipo di oggetto, l&#39;origine del campo, il nome del campo, i qualificatori di filtro e il campo valore, essenziali per la creazione di filtri, visualizzazioni e raggruppamenti. &#x200B;
* **Specificità del tipo di oggetto:** filtri, visualizzazioni e raggruppamenti sono associati a tipi di oggetto specifici, ad esempio progetti, attività o ore, in modo da garantire che i report siano personalizzati in base ai dati pertinenti. &#x200B;
* **Regole filtro:** I filtri utilizzano origine campo, nome campo, qualificatori e valori per definire i criteri. &#x200B; Ad esempio, il filtro &quot;I miei progetti&quot; mostra solo i progetti correnti in cui l’utente connesso fa parte del team di progetto. &#x200B;
* **Visualizzazioni e raggruppamenti:** Le visualizzazioni visualizzano le combinazioni di nome campo e origine campo nelle colonne (ad esempio, &quot;nome proprietario&quot;), mentre i raggruppamenti organizzano i dati in base a criteri specifici (ad esempio, &quot;nome società&quot;). &#x200B;
* **Utilizzo dei caratteri jolly:** I caratteri jolly nei filtri consentono la corrispondenza dinamica, ad esempio l&#39;identificazione degli utenti connessi in un team di progetto, migliorando la personalizzazione nei rapporti. &#x200B;

## Riferimento rapido sui componenti di reporting

![Immagine della schermata per creare un filtro](assets/reporting-components-1.png)

**A - Origine campo**

Le opzioni di origine del campo dipendono dal tipo di oggetto selezionato. Spesso, l’origine del campo è l’elemento in Workfront a cui appartiene un’informazione specifica (o il nome del campo). A volte l’origine del campo è la stessa del tipo di oggetto.
L’origine del campo determina i nomi dei campi disponibili.

Esempi: [!UICONTROL Progetto], [!UICONTROL Attività], [!UICONTROL Problema], [!UICONTROL Assegnato a]

**B - Nome campo**

I nomi dei campi sono informazioni disponibili su ciò che è stato selezionato come origine del campo.

Possono essere campi Workfront compilati, campi di un modulo personalizzato o informazioni acquisite automaticamente da Workfront.

I nomi dei campi determinano le opzioni dei campi dei valori.

Esempi: [!UICONTROL Stato di avanzamento], [!UICONTROL Descrizione], [!UICONTROL Data di completamento pianificata], Campi modulo personalizzati

**C - Qualificatori del filtro**

I qualificatori di filtro consentono di limitare i possibili risultati visualizzabili nell’origine campo e nel nome campo selezionati.

Specificano la correlazione tra l’origine e il nome del campo e il campo del valore.

Esempi: Equal, Contains, Null, Less than

**D - Valore**

Il valore è l’informazione immessa nel campo specificato dal nome del campo.

Le opzioni relative al valore sono determinate dall’origine del campo e dal nome del campo.

Nel valore è possibile utilizzare caratteri jolly per utenti e date, nonché testo in formato libero.

Esempi: Nuovo, Attuale, $$TODAYbw, Descrizione

>[!TIP]
>
>Per informazioni su nomi di campo specifici in Workfront, consulta il [Glossario della terminologia di Adobe Workfront](https://experienceleague.adobe.com/docs/workfront/using/basics/workfront-terminology-glossary.html?lang=it).

