---
title: Integrare [!DNL Analytics] con [!DNL Commerce] esercitazione
description: Scopri come integrare [!DNL Analytics] con [!DNL Commerce].
solution: Analytics, Commerce
feature: Integrations
topic: Integrations
role: Leader, Architect, Admin, Developer
level: Beginner
index: true
hidefromtoc: true
kt: null
thumbnail: null
last-substantial-update: 2023-04-11T00:00:00Z
badgeIntegration: label="Integrazione" type="positive"
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '887'
ht-degree: 4%

---


# Integrare [!DNL Analytics] con [!DNL Commerce]

## Onboarding iniziale

Queste istruzioni sono per Adobe [!DNL Commerce] Progetti ospitati dal cloud. L’hosting autonomo può variare in una certa misura, ma il processo complessivo dovrebbe essere simile.

1. Verifica il codice nell’ambiente locale
1. Utilizzare il compositore e installare il modulo
1. Segui le singole istruzioni qui e, una volta completato, torna indietro per completare i passaggi rimanenti
   [Installare e configurare l’esperienza [!DNL Platform] connettore](https://experienceleague.adobe.com/docs/commerce-merchant-services/experience-platform-connector/fundamentals/install.html){target="_blank"}


1. Eseguire il commit del file compositore.json e, se nel cloud, del file compositore.lock
1. Verifica che il modulo si trovi negli ambienti di staging e/o produzione Effettuando l’accesso alla sezione di amministrazione di Adobe [!DNL Commerce] e cercando queste nuove sezioni in Sistema > Servizi
   ![Esperienza [!DNL Platform] estensione del connettore](./assets/analytics-commerce/admin-view-experience-platform-commector-extension.png)

1. Configura il modulo con le tue credenziali dall’interno dell’Adobe [!DNL Commerce] back office.
   * Prima il [!DNL Commerce] Configurazioni del connettore servizi, come illustrato di seguito.
     ![[!DNL Commerce] Configurazione di Services Connector](./assets/analytics-commerce/commerce-services-connector-setup.png)
   * Poi l’esperienza [!DNL Platform] impostazioni del connettore, come illustrato di seguito.
     ![Esperienza [!DNL Platform] connettore](./assets/analytics-commerce/experience-platform-connector.png)

Per maggiori dettagli su ciascuna fase e fase del processo di onboarding, segui le istruzioni riportate sulla sezione [Esperienza [!DNL Platform] panoramica del connettore](https://experienceleague.adobe.com/docs/commerce-merchant-services/experience-platform-connector/overview.html){target="_blank"}. L&#39;esperienza [!DNL Platform] il tutorial sul connettore descrive in modo approfondito ogni sezione e fornisce risposte a eventuali domande. Utilizza questa esercitazione per gli altri passaggi della configurazione rapida.

## Configurazione di Experience Edge e Adobe [!DNL Analytics]

1. Verifica che la tua organizzazione abbia (e tu abbia) accesso a Adobe [!DNL Analytics]. Per confermare, vai al [Home page di Adobe Experience Cloud](https://experience.adobe.com/) e facendo clic sul selettore dell’applicazione (nove punti) nella navigazione superiore.

1. Creare una nuova suite di rapporti in Adobe [!DNL Analytics], o identifica l&#39;ID della suite di rapporti che verrà inviata [!DNL Commerce] dati in. Per ulteriori informazioni, guarda un tutorial su [creazione di una nuova suite di rapporti](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/intro-to-analytics/analytics-basics/understanding-and-creating-report-suites.html?lang=it). Questo ID suite di rapporti è necessario nel passaggio dello stream di dati seguente.

1. Accedi a [Adobe Experience [!DNL Platform] Interfaccia](https://platform.adobe.com) se hai accesso a Experience [!DNL Platform]. Se non hai accesso a tale interfaccia, puoi eseguire tutti i passaggi necessari elencati di seguito in Adobe Experience [!DNL Platform] [Interfaccia di Data Collection](https://experience.adobe.com/it#/data-collection).

1. Crea o aggiorna lo schema XDM con [!DNL Commerce]gruppi di campi specifici di. Per ulteriori informazioni su come creare uno schema, consulta [&quot;Creare schemi&quot;](https://experienceleague.adobe.com/docs/platform-learn/tutorials/schemas/create-schemas.html?lang=it) esercitazione.
   * Dovrai selezionare questo schema dalle opzioni nel passaggio dello stream di dati seguente. Per creare uno schema, cerca nella colonna a sinistra sotto **Gestione dati** e trova **Schemi**. Ora fai clic su in alto a destra nell’interfaccia **Crea schema**. Seleziona ExperienceEvent XDM.
   * Dopo aver creato un nuovo schema, aggiungi [!DNL Commerce] gruppi di campi. Sul lato sinistro dell’interfaccia utente, individua i gruppi di campi e fai clic su **Aggiungi**
      * Nella ricerca, puoi filtrare immettendo `ExperienceEvent [!DNL Commerce]`
      * Seleziona la **Adobe [!DNL Analytics] ExperienceEvent[!DNL Commerce]** selezionando la casella
      * Quindi fai clic su **Aggiungi gruppi di campi** in alto a destra per salvare e continuare

1. Facoltativamente (e solo se sei nell’esperienza [!DNL Platform] ) - Crea un nuovo set di dati
   * Questo passaggio ti consente di portare [!DNL Commerce] dati nell’esperienza [!DNL Platform] (separatamente da portare i dati in Adobe [!DNL Analytics]). Esegui questo passaggio se hai accesso a Experience [!DNL Platform]e prevedono di utilizzare il [!DNL Commerce] dati nell’esperienza [!DNL Platform]- applicazioni supportate, come Real-Time Customer Data [!DNL Platform], Percorso di clienti [!DNL Analytics]o Journey Optimizer.
   * Dovrai selezionare questo set di dati dalle opzioni nel passaggio dello stream di dati seguente.
   * Sotto la colonna sinistra **Gestione dati** nel menu di navigazione a sinistra, seleziona **Set di dati**.
   * Clic **Crea set di dati** in alto a destra. Scegli la **Crea set di dati dallo schema** opzione.
   * Cerca e utilizza lo schema creato nell’ultimo passaggio

1. Creare lo stream di dati per inviare [!DNL Commerce] dati da Adobe [!DNL Analytics]
   * Sotto **Raccolta dati** nella colonna sinistra, seleziona **Flussi di dati**.
   * Clic **Nuovo flusso di dati** in alto a destra nell’interfaccia.
   * Fornisci un nome e una descrizione facoltativa.
   * Trova e seleziona lo schema creato/identificato nel passaggio precedente.
   * Aggiungi le opzioni avanzate desiderate. Per ulteriori informazioni sulle opzioni avanzate, visita il [documentazione](https://experienceleague.adobe.com/docs/experience-platform/datastreams/configure.html).
   * Clic **Salva** per continuare.
   * Clic **Aggiungi servizio** e scegli **Adobe[!DNL Analytics]** nel campo a discesa.
   * Clic **Aggiungi suite di rapporti** e immetti l’ID suite di rapporti creato/identificato in un passaggio precedente. Puoi aggiungere più di una suite di rapporti se desideri che i dati fluiscano in più suite di rapporti.
   * Facoltativamente, e se hai creato un set di dati in un passaggio precedente, fai clic su **Aggiungi servizio** di nuovo, scegliendo **Adobe Experience[!DNL Platform]** dal campo a discesa. Nel campo Set di dati evento, seleziona il set di dati creato in precedenza.
   * Salva lo stream di dati.

1. Per visualizzare [!DNL Commerce] dati, dovrai passare ad Analysis Workspace in Adobe [!DNL Analytics], crea un progetto, scegli la tua suite di rapporti e aggiungi tabelle a forma libera e altre visualizzazioni per generare rapporti e analizzare i tuoi [!DNL Commerce] dati. L’immagine seguente mostra un esempio di tabella che è possibile creare in Analysis Workspace.

   ![[!DNL Analytics] Schermata di alcuni dati di e-commerce](./assets/analytics-commerce/analytics-screenshot-commerce-items.png)

   Di seguito sono riportate alcune risorse aggiuntive per aiutarti a lavorare in Analysis Workspace:

   * [Panoramica di Analysis Workspace](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/analysis-workspace-basics/analysis-workspace-overview.html)
   * [Creazione di un progetto Workspace da zero](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/analysis-workspace-basics/building-a-workspace-project-from-scratch.html)
   * [Utilizzo di tabelle, visualizzazioni e pannelli in Analysis Workspace](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/using-panels/using-tables-visualizations-and-panels.html)
   * [Casi d’uso per le visualizzazioni](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/visualizations/visualization-use-cases.html)

   Inoltre, sono disponibili corsi gratuiti su Experience League. Consulta [!DNL Analytics] corsi disponibili [QUI](https://experienceleague.adobe.com/?lang=en&amp;Solution=[!DNL Analytics]#courses).
