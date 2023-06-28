---
title: Mostra indisponibilità influisce sulle sequenze temporali del progetto
description: Scopri cosa succede alla timeline di un progetto quando l’impostazione dell’ora di inattività è attivata e disattivata.
feature: Resource Management
type: Tutorial
role: Leader, User
level: Intermediate, Experienced
activity: use
team: Technical Marketing
jira: KT-10180
exl-id: 0f79dd8d-b7ce-4ee9-b211-23c8ed5d497c
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '524'
ht-degree: 4%

---

# Effetti del tempo libero sulle sequenze temporali dei progetti

Se i fattori di indisponibilità di un utente assegnato nella sequenza temporale del progetto dipendono dall’impostazione di un progetto denominata [!UICONTROL Indisponibilità utente]. Questa impostazione determina se il tempo libero dell&#39;assegnatario principale dell&#39;attività regola le date pianificate per l&#39;attività nel progetto.

Osserviamo cosa accade con una sequenza temporale del progetto quando ciascuna delle impostazioni è selezionata:[!UICONTROL considerare l&#39;indisponibilità dell&#39;utente durante l&#39;attività] o [!UICONTROL Ignora indisponibilità utente durante l&#39;attività].

![Impostazione del tempo di inattività dell&#39;utente](assets/toapt_01.png)

## Considerare l&#39;indisponibilità dell&#39;utente durante l&#39;attività

Questa opzione è l’impostazione predefinita di Workfront.

In questo esempio, il calendario personale dell&#39;assegnatario principale dell&#39;attività contiene giorni liberi.

![calendario personale](assets/toapt_02.png)

Il project manager desidera assegnare questa persona a un&#39;attività con date pianificate che si sovrappongono all&#39;indisponibilità dell&#39;utente.

![attività progetto con date](assets/toapt_03.png)

Quando questo utente viene assegnato all&#39;attività, le date pianificate vengono regolate automaticamente. Ora la data di completamento pianificata dell’attività è stata estesa di diversi giorni per tenere conto del tempo libero dell’utente. È importante notare che questa modifica può influenzare le date pianificate di altre attività nel progetto e, potenzialmente, la data di completamento pianificata del progetto.

![attività di progetto con data di scadenza](assets/toapt_04.png)

## [!UICONTROL Ignorare l&#39;indisponibilità dell&#39;utente durante l&#39;attività]

Con questa opzione, le date pianificate dell&#39;attività rimangono quelle pianificate in origine, anche se l&#39;assegnatario principale presenta un&#39;indisponibilità durante la durata dell&#39;attività.

Il membro del team ha giorni liberi contrassegnati sul calendario.

![calendario pto con date contrassegnate](assets/toapt_05.png)

Il project manager assegna loro un&#39;attività che si sovrappone al tempo libero. Una volta assegnato l&#39;utente, le date pianificate dell&#39;attività rimangono quelle pianificate in origine.

![modificare le date delle attività di progetto](assets/toapt_06.png)

Per garantire che il lavoro venga eseguito in tempo, potrebbe essere utile assegnare un&#39;altra persona che possa lavorare sull&#39;attività mentre l&#39;assegnatario originale è fuori dall&#39;ufficio.

## Regolare l’impostazione a livello di progetto

Per modificare l’impostazione Indisponibilità utente in un progetto:

* Apri il progetto facendo clic sul nome in Workfront.

* Seleziona [!UICONTROL Modifica] dal menu a 3 punti nell’intestazione della pagina, a destra del nome del progetto.

* Scorri fino a [!UICONTROL Impostazioni progetto] e trova la sezione [!UICONTROL Indisponibilità utente] campo.

* Selezionare l&#39;opzione che si desidera applicare al progetto: [!UICONTROL Considerare l&#39;indisponibilità dell&#39;utente durante l&#39;attività] o I[!UICONTROL ignora indisponibilità dell&#39;utente durante l&#39;attività].

* Fai clic su [!UICONTROL Salva] nell&#39;angolo superiore destro della finestra.

![Considerare l&#39;indisponibilità dell&#39;utente durante l&#39;attività](assets/toapt_07.png)


**Nota**: questa impostazione non è disponibile quando si seleziona [!UICONTROL Dettagli progetto] dal menu del pannello sinistro della pagina del progetto.

Un&#39;impostazione globale esiste nelle preferenze del progetto in [!UICONTROL Configurazione] menu. Questa impostazione è gestita dall&#39;amministratore di sistema. Gli amministratori di gruppi possono regolare questa impostazione per i gruppi che gestiscono.

Workfront consiglia di impostare l’impostazione nel modo in cui desideri che la maggior parte dei progetti gestisca il tempo libero nella tua organizzazione.

L’impostazione può anche essere incorporata nei modelli di progetto, attraverso i dettagli del modello.
