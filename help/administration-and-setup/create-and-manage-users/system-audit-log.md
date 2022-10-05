---
title: Comprendere il registro di controllo del sistema
description: Scopri come utilizzare il registro di controllo del sistema per esaminare quando sono state apportate modifiche e quando apportare modifiche agli elementi.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Beginner, Intermediate
thumbnail: 10040.jpeg
kt: 10040
exl-id: 9de6fd40-10fb-47a6-b186-3a38c411f1ac
source-git-commit: adf12d7846d2a1b4c32513a3955c080905044576
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 0%

---

# Comprendere il registro di controllo del sistema

Il registro di controllo del sistema è il modo migliore per l’amministratore di sistema per controllare cosa succede [!DNL Workfront]. Pensa al log come la tua fonte di verità per chi ha fatto ciò che cambia e quando.

Accedi al registro di controllo andando al [!UICONTROL Preferenze] nella sezione [!UICONTROL Configurazione] area. Per impostazione predefinita, vengono visualizzati i dati degli ultimi sette giorni. Modifica i criteri di filtro per visualizzare i dati provenienti da diversi intervalli di date.

Quando un utente esegue determinate azioni, [!UICONTROL Workfront] li registra nel [!UICONTROL Registri di controllo] della sezione [!UICONTROL Configurazione] area.

![[!UICONTROL Tipo di registro] menu a discesa [!UICONTROL Registri di controllo] in [!UICONTROL Configurazione]](assets/admin-fund-audit-log-1.png)

Ogni azione registrata o registrata mostra:

* Data e ora della modifica
* Tipo di registro
* Nome dell’utente che ha completato l’azione
* L&#39;oggetto
* Eventuali dettagli associati all’azione
* Indirizzo IP

![[!UICONTROL Registro di controllo] elenco](assets/admin-fund-audit-log-2.JPG)

## Esportare il registro di controllo

L’esportazione dei dati del registro di controllo consente agli amministratori di sistema di condividere le informazioni con revisori interni/esterni o specialisti della sicurezza. Alcune organizzazioni richiedono la conservazione di alcuni registri per rispettare le normative sulla sicurezza informatica. Altri hanno bisogno delle informazioni importate in un sistema di sicurezza per l&#39;analisi.

I registri di controllo possono essere esportati in un file CSV (con valori separati da virgole), che può essere aperto in un’applicazione per fogli di calcolo o in un editor di testo normale. L’esportazione è limitata a 50.000 righe alla volta, quindi utilizza i filtri per restringere l’elenco se il totale supera 50.000 righe.

![[!UICONTROL Esporta] pulsante [!UICONTROL Registri di controllo] page](assets/admin-fund-audit-log-3.png)

<!---
learn more URLs
Audit logs
Managing audit logs
--->
