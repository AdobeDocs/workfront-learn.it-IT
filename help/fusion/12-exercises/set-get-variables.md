---
title: Esercizio per le variabili Set e Get
description: Scopri come utilizzare i moduli Variabile Set e Get per utilizzare i campi disponibili in un percorso diverso dall’originale.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11045
thumbnail: KT11045.png
recommendations: noDisplay,noCatalog
exl-id: 225f0090-0428-40e2-8a4b-9c6b18b205d2
source-git-commit: a4e61514567ac8c2b4ad5c9ecacb87bd83947731
workflow-type: ht
source-wordcount: '641'
ht-degree: 100%

---

# Esercizio per le variabili Set e Get

Scopri come utilizzare i moduli Variabile Set e Get per utilizzare i campi disponibili in un percorso diverso dall’originale.

## Panoramica dell’esercizio

Cerca informazioni su un progetto in Workfront e invia un’e-mail con le informazioni correlate.

![Immagine 1 Variabili Set e Get](../12-exercises/assets/set-get-variables-walkthrough-1.png)

## Passaggi da seguire

1. Crea un nuovo scenario e denominalo “Condivisione di variabili tra percorsi di indirizzamento”.
1. Per il trigger, seleziona il modulo Ricerca nell’app Workfront.

   + Imposta il Tipo record su Progetto.
   + Scegli Tutti i record corrispondenti come Set di risultati.
   + Imposta Stato uguale a CUR come Criteri di ricerca.
   + Scegli ID, Nome, Descrizione e ID sponsor come Output.

   ![Immagine 2 Variabili Set e Get](../12-exercises/assets/set-get-variables-walkthrough-2.png)

   ![Immagine 3 Variabili Set e Get](../12-exercises/assets/set-get-variables-walkthrough-3.png)

1. Fai clic su OK e rinomina il modulo “Trova progetti correnti”.
1. Aggiungi un altro modulo e seleziona il modulo Workfront Leggi un record.

   + Scegli Utente come Tipo di record.
   + Scegli Nome come Output.
   + Mappa l’ID sponsor al campo ID dal modulo Ricerca.

1. Fai clic su OK.
1. Rinomina il modulo “Trova nome sponsor”.

   ![Immagine 4 Variabili Set e Get](../12-exercises/assets/set-get-variables-walkthrough-4.png)

1. Salva lo scenario e fai clic su Esegui una volta.

   Se ricevi un errore nel modulo Leggi un record, è probabile che il modulo Ricerca stia trovando un progetto privo di sponsor elencato.

   **Per evitare questo errore, crea due percorsi: uno per i progetti che hanno un ID sponsor e uno per i progetti che non lo hanno.**

1. Aggiungi un router tra i due moduli facendo clic sull’icona della chiave inglese tra il router e il modulo Leggi un record. Imposta un filtro denominato “Sponsor esistente” e imposta la condizione su ID sponsor esistente.

   ![Immagine 5 Variabili Set e Get](../12-exercises/assets/set-get-variables-walkthrough-5.png)

1. Fai clic sul router per creare un altro percorso. Aggiungi un modulo Invia un’e-mail dall’app E-mail.

   + Inserisci il tuo indirizzo e-mail nel campo A.
   + Nel campo Oggetto, digita “Informazioni sul progetto corrente”.
   + Nel campo Contenuto, inserisci il nome del progetto, la descrizione e lo sponsor.
   + Non è possibile recuperare l’output del nome dello sponsor dal modulo Leggi un record. È possibile accedere all’ID sponsor solamente dal modulo Ricerca prima del router. È necessario trovare un modo per accedere al nome dello sponsor dall’altro percorso del router.

   ![Immagine 6 Variabili Set e Get](../12-exercises/assets/set-get-variables-walkthrough-6.png)

1. Per il momento, fai clic su OK e rinomina il modulo “Invia informazioni sul progetto”.

   **Utilizza le variabili Set/Get per condividere i dati tra percorsi diversi.**

1. Dopo il modulo Trova nome sponsor, aggiungi un modulo Strumento variabile Set.

   + Inserisci “Nome sponsor” come nome di Variabile.
   + Lascia la durata della variabile su Un ciclo.
   + Mappa il campo all’output del nome dal modulo Trova nome sponsor.

1. Fai clic su OK, quindi rinomina il modulo “Imposta nome sponsor”.

   ![Immagine 7 Variabili Set e Get](../12-exercises/assets/set-get-variables-walkthrough-7.png)

1. Successivamente, fai clic con il pulsante destro del mouse tra il router e il modulo Invia un’e-mail per aggiungere un modulo Strumento variabile Get. Inserisci “Nome sponsor” nel campo Nome variabile.
1. Fai clic su OK. Rinomina il modulo “Ottieni nome sponsor.”

   ![Immagine 8 Variabili Set get](../12-exercises/assets/set-get-variables-walkthrough-8.png)

1. Torna al modulo Invia un’e-mail e mappa il valore dal modulo Ottieni nome sponsor nel campo Contenuto. Fai clic su OK.

   ![Immagine 8 Variabili Set Get](../12-exercises/assets/set-get-variables-walkthrough-8.png)

   >[!IMPORTANT]
   >
   >Prima di testare lo scenario, ti consigliamo di limitare il numero di progetti elaborati per evitare di ricevere un’ondata di e-mail.

1. Vai alla prova di Workfront e individua il progetto Northstar Fashion Exhibitors Booth. Questo è un progetto corrente che ha uno sponsor. Copia l’ID del progetto dall’URL.

   ![Immagine 10 Variabili Set Get](../12-exercises/assets/set-get-variables-walkthrough-10.png)

1. Nel tuo scenario, fai clic sul modulo Trova progetti correnti. Aggiungi un’altra condizione ai criteri di ricerca facendo clic sul pulsante verde “Aggiungi regola AND”. Specifica che l’ID deve essere uguale all’ID del progetto che hai copiato. Fai clic su OK.
1. Salva lo scenario e fai clic su Esegui una volta.
1. Esamina i controlli di esecuzione e l’e-mail che ricevi.

   ![Immagine 11 Variabili Set e Get](../12-exercises/assets/set-get-variables-walkthrough-11.png)
