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
jira: KT-10040
exl-id: 9de6fd40-10fb-47a6-b186-3a38c411f1ac
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 0%

---

# Comprendere il registro di controllo del sistema

Il registro di audit del sistema è il modo migliore per l’amministratore di sistema di tenere d’occhio ciò che accade in [!DNL Workfront]. Pensa al registro come alla tua fonte di verità per chi ha fatto ciò che cambia e quando.

Accedi al registro di controllo accedendo a [!UICONTROL Preferenze] sezione nella sezione [!UICONTROL Configurazione] area. Per impostazione predefinita, vengono visualizzati i dati degli ultimi sette giorni. Modifica i criteri del filtro per visualizzare i dati di intervalli di date diversi.

Quando un utente esegue determinate azioni, [!UICONTROL Workfront] li registra in [!UICONTROL Registri di controllo] sezione del [!UICONTROL Configurazione] area.

![[!UICONTROL Tipo di registro] menu a discesa sulla [!UICONTROL Registri di controllo] pagina in [!UICONTROL Configurazione]](assets/admin-fund-audit-log-1.png)

Ogni azione registrata o registrata mostra:

* Data e ora della modifica
* Tipo di registro
* Nome dell&#39;utente che ha completato l&#39;azione
* L&#39;oggetto
* Qualsiasi dettaglio associato all’azione
* Indirizzo IP

![[!UICONTROL Registro di controllo] list](assets/admin-fund-audit-log-2.JPG)

## Esportare il registro di controllo

L’esportazione dei dati del registro di audit consente agli amministratori di sistema di condividere le informazioni con revisori interni/esterni o specialisti della sicurezza. Alcune organizzazioni richiedono la conservazione di alcuni registri per garantire la conformità alle normative sulla cibersicurezza. Altri hanno bisogno delle informazioni importate in un sistema di sicurezza per l&#39;analisi.

I registri di controllo possono essere esportati in un file CSV (con valori delimitati da virgole), che può essere aperto in un’applicazione per fogli di calcolo o in un editor di testo normale. L’esportazione è limitata a 50.000 righe alla volta. Pertanto, se il totale supera le 50.000, restringi l’elenco utilizzando i filtri.

![[!UICONTROL Esporta] pulsante attivato [!UICONTROL Registri di controllo] pagina](assets/admin-fund-audit-log-3.png)

<!---
learn more URLs
Audit logs
Managing audit logs
--->
