---
title: Imposta/Ottieni variabili
description: Scopri come utilizzare i moduli Imposta e Ottieni variabile per utilizzare i campi disponibili in un percorso diverso.
feature: Workfront Fusion
role: User
level: Beginner
kt: 11045
thumbnail: KT11045.png
source-git-commit: 1f7a4da813805691fc0e52d3ad1ea708f9e07a9a
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 0%

---


# Imposta/Ottieni variabili

Scopri come utilizzare i moduli Imposta e Ottieni variabile per utilizzare i campi disponibili in un percorso diverso.

## Panoramica sull&#39;esercizio

Cerca informazioni su un progetto in Workfront e invia un’e-mail con le relative informazioni.

![Imposta Get variables Immagine 1](../12-exercises/assets/set-get-variables-walkthrough-1.png)

## Passaggi da seguire

1. Crea un nuovo scenario e denominalo &quot;Condivisione di variabili tra percorsi di indirizzamento&quot;.
1. Per l’attivatore, seleziona il modulo Ricerca nell’app Workfront.

   + Imposta il tipo di record su Progetto.
   + Per il set di risultati, scegliere Tutti i record corrispondenti.
   + Per i criteri di ricerca, impostalo su Stato uguale a CUR.
   + Per Output, scegli ID, nome, descrizione e ID sponsor.

   ![Imposta Get variables Immagine 2](../12-exercises/assets/set-get-variables-walkthrough-2.png)

   ![Imposta Get variables Image 3](../12-exercises/assets/set-get-variables-walkthrough-3.png)

1. Fare clic su OK e rinominare il modulo &quot;Trova progetti correnti&quot;.
1. Aggiungi un altro modulo e seleziona il modulo Workfront Read a record.

   + Per Tipo di record, scegli Utente.
   + Per Output scegliere Nome.
   + Mappa l’ID sponsor dal modulo Ricerca al campo ID.

1. Fate clic su OK.
1. Rinomina il modulo &quot;Trova nome sponsor&quot;.

   ![Imposta Get variables Immagine 4](../12-exercises/assets/set-get-variables-walkthrough-4.png)

1. Salva lo scenario e fai clic su Esegui una volta.

   Se si riceve un errore nel modulo Leggi un record, è probabile che il modulo Ricerca trovi un progetto senza uno sponsor elencato.

   **Per evitare questo errore, crea due percorsi: uno per i progetti che hanno un ID sponsor e uno per i progetti che non lo sono.**

1. Aggiungere un router tra i due moduli facendo clic sull&#39;icona chiave tra il router e il modulo Leggi un record. Imposta un filtro denominato &quot;Sponsor exists&quot; (Esiste uno sponsor) e imposta la condizione su Sponsor ID Exists (Esiste un ID sponsor).

   ![Imposta Get variables Immagine 5](../12-exercises/assets/set-get-variables-walkthrough-5.png)

1. Fare clic sul router per creare un altro percorso. Aggiungi un modulo Invia un’e-mail dall’app E-mail.

   + Inserisci il tuo indirizzo e-mail nel campo A.
   + Nel campo Oggetto digitare &quot;Informazioni progetto corrente&quot;.
   + Nel campo Contenuto , inserisci il nome, la descrizione e lo sponsor del progetto.
   + Impossibile estrarre l&#39;output del nome dello sponsor dal modulo Leggi un record. È possibile accedere all&#39;ID dello sponsor solo dal modulo di ricerca prima del router. Sarà necessario trovare un modo per accedere al nome dello sponsor dall&#39;altro percorso del router.

   ![Imposta Get variables Image 6](../12-exercises/assets/set-get-variables-walkthrough-6.png)

1. Fai clic su OK per ora e rinomina il modulo &quot;Invia informazioni progetto&quot;

   **Utilizza le variabili Set/Get per condividere i dati tra percorsi diversi.**

1. Dopo il modulo Trova nome sponsor, aggiungi un modulo strumento Imposta variabile.

   + Inserisci &quot;Nome sponsor&quot; come nome della variabile.
   + Lasciare la durata della variabile a un ciclo.
   + Mappare il campo all&#39;output del nome dal modulo Trova nome sponsor.

1. Fare clic su OK, quindi rinominare il modulo &quot;Imposta nome sponsor&quot;.

   ![Imposta Get variables Image 7](../12-exercises/assets/set-get-variables-walkthrough-7.png)

1. Quindi, fare clic con il pulsante destro del mouse tra il router e il modulo Invia un&#39;e-mail per aggiungere un modulo strumento Get variable. Immettere &quot;Nome sponsor&quot; nel campo Nome variabile.
1. Fate clic su OK. Rinomina il modulo &quot;Ottieni nome sponsor&quot;.

   ![Imposta Get variables Image 8](../12-exercises/assets/set-get-variables-walkthrough-8.png)

1. Torna al modulo Invia un messaggio e-mail e mappa il valore dal modulo Ottieni nome sponsor nel campo del contenuto. Fate clic su OK.

   ![Imposta Get variables Image 8](../12-exercises/assets/set-get-variables-walkthrough-8.png)

   >[!IMPORTANT]
   >
   >Prima di testare lo scenario, consigliamo di limitare il numero di progetti elaborati per evitare di ricevere un flusso di e-mail.

1. Vai alla tua unità di test Workfront e individua il progetto Northstar Fashion Exhibitors Booth. Questo è un progetto corrente con uno sponsor. Copia l&#39;ID del progetto dall&#39;URL.

   ![Imposta Ottieni variabili Immagine 10](../12-exercises/assets/set-get-variables-walkthrough-10.png)

1. Nel tuo scenario, fai clic sul modulo Trova progetti correnti . Aggiungi un’altra condizione ai criteri di ricerca facendo clic sul pulsante verde &quot;Aggiungi regola AND&quot;. Specifica che l&#39;ID deve essere uguale all&#39;ID progetto copiato. Fate clic su OK.
1. Salva lo scenario e fai clic su Esegui una volta.
1. Controlla gli ispettori di esecuzione e l&#39;e-mail che ricevi.

   ![Imposta Ottieni variabili Immagine 11](../12-exercises/assets/set-get-variables-walkthrough-11.png)
