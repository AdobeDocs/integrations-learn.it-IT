---
title: Integra [!DNL Analytics] con [!DNL Commerce] esercitazione
description: Scopri come integrare  [!DNL Analytics] con [!DNL Commerce].
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
exl-id: ef50b6b3-1e2b-4fe9-98d5-555bc14ae8d6
source-git-commit: 46803595cf8e199e0c331ea8b82f7fe4a2afc801
workflow-type: tm+mt
source-wordcount: '821'
ht-degree: 0%

---

# Integra [!DNL Analytics] con [!DNL Commerce]

## Onboarding iniziale

Queste istruzioni sono per Adobe [!DNL Commerce] progetti ospitati da Cloud. L’hosting autonomo può variare in una certa misura, ma il processo complessivo dovrebbe essere simile.

1. Verifica il codice nell’ambiente locale
1. Utilizzare il compositore e installare il modulo
1. Segui le singole istruzioni qui e, una volta completato, torna indietro per completare i passaggi rimanenti
   [Installa e configura Experience [!DNL Platform] connector](https://experienceleague.adobe.com/docs/commerce-merchant-services/experience-platform-connector/fundamentals/install.html?lang=it){target="_blank"}


1. Eseguire il commit del file compositore.json e, se nel cloud, del file compositore.lock
1. Verifica che il modulo si trovi negli ambienti di staging e/o produzione
Per eseguire questa operazione, accedere alla sezione di amministrazione dell&#39;Adobe [!DNL Commerce] e cercare queste nuove sezioni in Sistema > Servizi
   ![Estensione connettore [!DNL Platform] esperienza](./assets/analytics-commerce/admin-view-experience-platform-commector-extension.png)

1. Configurare il modulo con le credenziali dall&#39;interno del back office Adobe [!DNL Commerce].
   * Innanzitutto le configurazioni del connettore dei servizi [!DNL Commerce], come illustrato di seguito.

     Installazione di ![[!DNL Commerce] Services Connector](./assets/analytics-commerce/commerce-services-connector-setup.png)
   * Quindi le impostazioni del connettore Experience [!DNL Platform], come illustrato di seguito.

     ![Esperienza [!DNL Platform] connettore](./assets/analytics-commerce/experience-platform-connector.png)

Per maggiori dettagli su ogni fase e passaggio del processo di onboarding, segui le istruzioni riportate nella [Panoramica del connettore [!DNL Platform] Experience](https://experienceleague.adobe.com/docs/commerce-merchant-services/experience-platform-connector/overview.html?lang=it){target="_blank"}. Il tutorial sul connettore Experience [!DNL Platform] tratta ogni sezione in modo approfondito e risponde alle tue eventuali domande. Utilizza questa esercitazione per gli altri passaggi della configurazione rapida.

## Configurazione di Experience Edge e Adobe [!DNL Analytics]

1. Verifica che la tua organizzazione disponga dell&#39;accesso all&#39;Adobe [!DNL Analytics]. Per confermare questa operazione, vai alla [home page di Adobe Experience Cloud](https://experience.adobe.com/) e fai clic sul selettore dell&#39;applicazione (nove punti) nella navigazione superiore.

1. Crea una nuova suite di rapporti nell&#39;Adobe [!DNL Analytics] o identifica l&#39;ID della suite di rapporti in cui verranno inseriti i dati di [!DNL Commerce]. Per ulteriori informazioni, guarda un&#39;esercitazione su [creazione di una nuova suite di rapporti](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/intro-to-analytics/analytics-basics/understanding-and-creating-report-suites.html?lang=it). Questo ID suite di rapporti è necessario nel passaggio dello stream di dati seguente.

1. Se hai accesso all&#39;esperienza [!DNL Platform], passa a [Adobe Experience [!DNL Platform] interface](https://platform.adobe.com). Se non hai accesso a tale interfaccia, puoi eseguire tutti i passaggi necessari elencati di seguito nell&#39;interfaccia [!DNL Platform] [Raccolta dati](https://experience.adobe.com/#/data-collection) dell&#39;esperienza Adobe.

1. Crea o aggiorna lo schema XDM con gruppi di campi specifici per [!DNL Commerce]. Per ulteriori informazioni su come creare uno schema, vedere l&#39;esercitazione [&quot;Creare schemi&quot;](https://experienceleague.adobe.com/docs/platform-learn/tutorials/schemas/create-schemas.html?lang=it).
   * Dovrai selezionare questo schema dalle opzioni nel passaggio dello stream di dati seguente. Per creare uno schema, cerca nella colonna sinistra in **Gestione dati** e trova **Schemi**. Ora fai clic su **Crea schema** in alto a destra nell&#39;interfaccia. Seleziona ExperienceEvent XDM.
   * Dopo aver creato un nuovo schema, aggiungerai i gruppi di campi [!DNL Commerce]. Sul lato sinistro dell&#39;interfaccia utente, individua i gruppi di campi e fai clic su **Aggiungi**
      * Nella ricerca, è possibile filtrare immettendo `ExperienceEvent Commerce`
      * Seleziona **Adobe [!DNL Analytics] ExperienceEvent[!DNL Commerce]** selezionando la casella
      * Quindi fai clic su **Aggiungi gruppi di campi** in alto a destra per salvare e continuare

1. Facoltativamente (e solo se ti trovi nell&#39;interfaccia Esperienza [!DNL Platform]) - Crea un nuovo set di dati
   * Questo passaggio ti consente di inserire i dati di [!DNL Commerce] nell&#39;esperienza [!DNL Platform] (separatamente da quelli di Adobe [!DNL Analytics]). Eseguire questo passaggio se si dispone dell&#39;accesso all&#39;esperienza [!DNL Platform] e si prevede di utilizzare i dati di [!DNL Commerce] nelle applicazioni supportate da Experience [!DNL Platform], come Real-Time Customer Data [!DNL Platform], Customer Percorsi [!DNL Analytics] o Journey Optimizer.
   * Dovrai selezionare questo set di dati dalle opzioni nel passaggio dello stream di dati seguente.
   * Nell&#39;intestazione della colonna sinistra **Gestione dati** nel menu di navigazione di sinistra, seleziona **Set di dati**.
   * Fai clic su **Crea set di dati** in alto a destra. Scegli l&#39;opzione **Crea set di dati dallo schema**.
   * Cerca e utilizza lo schema creato nell’ultimo passaggio

1. Crea lo stream di dati per inviare i dati [!DNL Commerce] all&#39;Adobe [!DNL Analytics]
   * Sotto l&#39;intestazione **Raccolta dati** nella colonna sinistra, selezionare **Flussi dati**.
   * Fai clic su **Nuovo flusso di dati** in alto a destra nell&#39;interfaccia.
   * Fornisci un nome e una descrizione facoltativa.
   * Trova e seleziona lo schema creato/identificato nel passaggio precedente.
   * Aggiungi le opzioni avanzate desiderate. Per ulteriori informazioni sulle opzioni avanzate, visita la [documentazione](https://experienceleague.adobe.com/docs/experience-platform/datastreams/configure.html?lang=it).
   * Fai clic su **Salva** per continuare.
   * Fai clic su **Aggiungi servizio** e scegli **Adobe[!DNL Analytics]** nel campo a discesa.
   * Fai clic su **Aggiungi suite di rapporti** e immetti l&#39;ID suite di rapporti creato/identificato in un passaggio precedente. Puoi aggiungere più di una suite di rapporti se desideri che i dati fluiscano in più suite di rapporti.
   * Facoltativamente e se hai creato un set di dati in un passaggio precedente, fai di nuovo clic su **Aggiungi servizio**, scegliendo **Esperienza Adobe[!DNL Platform]** dal campo a discesa. Nel campo Set di dati evento, seleziona il set di dati creato in precedenza.
   * Salva lo stream di dati.

1. Infine, per visualizzare i dati di [!DNL Commerce], devi passare ad Analysis Workspace nell&#39;Adobe [!DNL Analytics], creare un progetto, scegliere la suite di rapporti e aggiungere tabelle a forma libera e altre visualizzazioni per creare rapporti e analizzare i dati di [!DNL Commerce]. L’immagine seguente mostra un esempio di tabella che è possibile creare in Analysis Workspace.

   ![[!DNL Analytics] Schermata di alcuni dati di e-commerce](./assets/analytics-commerce/analytics-screenshot-commerce-items.png)

   Di seguito sono riportate alcune risorse aggiuntive per aiutarti a lavorare in Analysis Workspace:

   * [Panoramica di Analysis Workspace](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/analysis-workspace-basics/analysis-workspace-overview.html?lang=it)
   * [Creazione di un progetto Workspace da zero](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/analysis-workspace-basics/building-a-workspace-project-from-scratch.html?lang=it)
   * [Utilizzo di tabelle, visualizzazioni e pannelli in Analysis Workspace](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/using-panels/using-tables-visualizations-and-panels.html?lang=it)
   * [Casi di utilizzo delle visualizzazioni](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/visualizations/visualization-use-cases.html?lang=it)

   Inoltre, sono disponibili corsi gratuiti su Experience League. Consulta [!DNL Analytics] corsi disponibili [QUI](https://experienceleague.adobe.com/it?lang=en&Solution=Analytics#courses).
