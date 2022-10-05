---
title: L’ora di disattivazione influisce sulle timeline del progetto
description: Scopri cosa succede alla timeline di un progetto quando l’impostazione dell’ora di disattivazione è attivata e disattivata.
feature: Resource Management
type: Tutorial
role: Leader, User
level: Intermediate, Experienced
activity: use
team: Technical Marketing
kt: 10180
exl-id: 0f79dd8d-b7ce-4ee9-b211-23c8ed5d497c
source-git-commit: 02bc5a09a838be6d98c9b746bff731236ee4116f
workflow-type: tm+mt
source-wordcount: '524'
ht-degree: 4%

---

# Effetti del tempo di inattività sulle timeline dei progetti

Il fattore di tempo libero assegnato a un utente nella timeline del progetto dipende da un’impostazione di progetto denominata [!UICONTROL Ora di disattivazione utente]. Questa impostazione determina se il tempo di inattività per l&#39;assegnatario principale dell&#39;attività regola le date pianificate per tale attività sul progetto.

Osserviamo cosa succede nella timeline di un progetto quando ciascuna delle impostazioni è selezionata: C[!UICONTROL Considerare il tempo di inattività dell&#39;utente nelle durate delle attività] o [!UICONTROL Ignora il tempo di inattività dell&#39;utente nelle durate dell&#39;attività].

![Impostazione del tempo di disattivazione dell&#39;utente](assets/toapt_01.png)

## Considerare l&#39;indisponibilità dell&#39;utente durante l&#39;attività

Questa opzione è l’impostazione predefinita di Workfront.

In questo esempio, l&#39;assegnatario principale per l&#39;attività ha giorni liberi contrassegnati sul proprio calendario personale.

![calendario personale](assets/toapt_02.png)

Il project manager desidera assegnare questa persona a un&#39;attività con date pianificate che si sovrappongono al tempo di inattività dell&#39;utente.

![attività del progetto con date](assets/toapt_03.png)

Quando l&#39;utente viene assegnato all&#39;attività, le date pianificate vengono regolate automaticamente. Ora la data di completamento pianificata dell’attività è stata estesa di diversi giorni per adattarsi al tempo di inattività dell’utente. È importante notare che questa modifica può influenzare le date pianificate di altre attività del progetto e, potenzialmente, la data di completamento pianificata del progetto.

![attività del progetto con scadenza](assets/toapt_04.png)

## [!UICONTROL Ignorare l&#39;indisponibilità dell&#39;utente durante l&#39;attività]

Con questa opzione, le date pianificate dell&#39;attività rimangono come pianificate in origine, anche se l&#39;assegnatario primario ha del tempo di inattività durante la durata dell&#39;attività.

Il membro del team ha giorni liberi contrassegnati sul calendario.

![calendario pto con date contrassegnate](assets/toapt_05.png)

Il project manager assegna loro un&#39;attività che si sovrappone al tempo di inattività. Una volta assegnato l&#39;utente, le date pianificate dell&#39;attività rimangono come originariamente pianificate.

![regola le date delle attività del progetto](assets/toapt_06.png)

Per garantire che il lavoro venga svolto in tempo, potrebbe essere utile assegnare un&#39;altra persona che può lavorare sull&#39;attività mentre l&#39;assegnatario originale è fuori ufficio.

## Regolare l’impostazione a livello di progetto

Per modificare l’impostazione Ora di disattivazione utente di un progetto:

* Apri il progetto facendo clic sul suo nome in Workfront.

* Seleziona [!UICONTROL Modifica] dal menu a 3 punti nell’intestazione della pagina, a destra del nome del progetto.

* Scorri fino a [!UICONTROL Impostazioni progetto] e trova la sezione [!UICONTROL Ora di disattivazione utente] campo .

* Seleziona l’opzione da applicare al progetto — [!UICONTROL Considerare il tempo di inattività dell&#39;utente nelle durate delle attività] o I[!UICONTROL ignorare il tempo di inattività dell&#39;utente nelle durate delle attività].

* Fai clic sul pulsante [!UICONTROL Salva] nell&#39;angolo superiore destro della finestra.

![Considerare l&#39;indisponibilità dell&#39;utente durante l&#39;attività](assets/toapt_07.png)


**Nota**: Questa impostazione non è disponibile quando si seleziona [!UICONTROL Dettagli progetto] dal menu del pannello a sinistra della pagina del progetto.

Un’impostazione globale per questo problema esiste nelle preferenze del progetto in [!UICONTROL Configurazione] menu. Questa impostazione è gestita dall’amministratore di sistema. Gli amministratori dei gruppi possono regolare questa impostazione per i gruppi gestiti.

Workfront consiglia di impostare l’impostazione in modo che la maggior parte dei progetti gestisca il tempo di inattività dell’organizzazione.

L’impostazione può essere integrata anche nei modelli di progetto, attraverso i dettagli del modello.
