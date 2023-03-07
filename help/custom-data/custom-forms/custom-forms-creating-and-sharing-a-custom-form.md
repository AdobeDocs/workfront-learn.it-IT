---
title: Creare e condividere un modulo personalizzato
description: Scopri come creare un modulo personalizzato, aggiungere campi univoci al modulo, organizzare i campi mediante sezioni e logiche e condividere i moduli con gli utenti.
feature: System Setup and Administration
type: Tutorial
role: Admin, Leader, User
level: Beginner, Intermediate
activity: use
team: Technical Marketing
thumbnail: 335172.png
kt: 8909
exl-id: b37334c7-67d0-4359-9537-dc26843582d1
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 5%

---

# Creare e condividere un modulo personalizzato

Questo video illustra come:

* Determinare gli oggetti da utilizzare per il modulo
* Aggiungere campi univoci in diversi formati
* Organizzare i campi utilizzando sezioni e logica
* Condividere moduli con altri utenti

>[!VIDEO](https://video.tv.adobe.com/v/335172/?quality=12)

## I moduli personalizzati funzionano con più tipi di oggetto

Quando fai clic su [!UICONTROL Nuovo modulo personalizzato] , è possibile selezionare tutti gli oggetti che si desidera utilizzare con un singolo modulo personalizzato. Tutti i campi aggiunti al modulo saranno disponibili per gli oggetti selezionati quando il modulo personalizzato verrà allegato a tali oggetti.

![Finestra del modulo personalizzato che mostra [!UICONTROL Nuovo modulo personalizzato] opzioni oggetto](assets/create-custom-form.png)

Quando modifichi un modulo personalizzato puoi visualizzare tutti i tipi di oggetto selezionati. È possibile aggiungere o eliminare tipi di oggetto da questo elenco.

![Finestra del modulo personalizzato che mostra i tipi di oggetto selezionati durante la modifica del modulo](assets/edit-custom-form.png)

Potrebbe essere utile creare un modulo personalizzato di tipo progetto e problema. Quando è allegato a un problema, è possibile compilare qualsiasi campo relativo al problema. Successivamente, se decidi di convertire il problema in un progetto, il modulo personalizzato verrà caricato automaticamente nel progetto e i dati inseriti nei campi del modulo personalizzato del problema saranno disponibili per la visualizzazione o la modifica nel modulo personalizzato del progetto.

## Opzioni campo personalizzato

**[!UICONTROL Etichetta] e [!UICONTROL Nome] campi**

Il [!UICONTROL Etichetta] e [!UICONTROL Nome] I campi di un campo personalizzato hanno scopi diversi. [!UICONTROL Etichetta] è il nome del campo che verrà visualizzato agli utenti in [!DNL Workfront]. [!UICONTROL Nome] è ciò che può essere utilizzato con le integrazioni, ad esempio API.

![Finestra del modulo personalizzato visualizzata [!UICONTROL Etichetta] e [!UICONTROL Nome] campi](assets/custom-forms-field-label-and-name.png)

Questo offre la flessibilità di modificare l’etichetta rivolta all’utente in modo che corrisponda alle modifiche apportate all’interno dell’organizzazione, senza influire sulle integrazioni o su altre connessioni che si basano su un nome di campo specifico.

**[!UICONTROL Campo di testo con formattazione]**

Il [!UICONTROL Campo di testo con formattazione ]contiene semplici strumenti di markup di testo che consentono agli utenti di aggiungere grassetto, corsivo o sottolineato al testo durante la compilazione del campo in un modulo personalizzato.

![Finestra del modulo personalizzato visualizzata [!UICONTROL Campo di testo con formattazione] opzione](assets/custom-forms-text-field-with-formatting.png)

Il campo ha anche un limite di 15.000 caratteri, che consente di disporre di molto spazio per fornire informazioni vitali e utilizzare la formattazione per semplificare la lettura.

**[!UICONTROL Automatico] campo**

Il [!UICONTROL Automatico] consente al sistema di compilare automaticamente un elenco di opzioni in base all&#39;oggetto selezionato per il campo.

![Finestra del modulo personalizzato visualizzata [!UICONTROL Automatico] opzione campo](assets/custom-forms-typeahead-1.png)

Ad esempio, se crei un’ [!UICONTROL Automatico] campo denominato &quot;Nome di approvazione del Marketing Manager&quot; e selezionare [!UICONTROL Utente] come tipo di oggetto di riferimento, viene visualizzato un elenco di nomi utente quando un utente compila tale campo in un modulo personalizzato. Il [!UICONTROL Automatico] Il campo serve a collegare i dati personalizzati con le informazioni acquisite nel sistema ed elimina la necessità di mantenere manualmente molte opzioni nei campi a discesa.

![Finestra del modulo personalizzato visualizzata [!UICONTROL Automatico] menu a discesa](assets/custom-forms-typeahead-2.png)
