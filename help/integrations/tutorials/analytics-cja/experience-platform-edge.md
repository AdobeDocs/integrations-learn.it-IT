---
title: Integra Adobe [!DNL Analytics] e Percorso clienti [!DNL Analytics] con l'esercitazione di Experience [!DNL Platform] Edge
description: Scopri come integrare Adobe [!DNL Analytics] con il Percorso clienti [!DNL Analytics] utilizzando AEP Web SDK, AEP Mobile SDK o l’API server di Edge Network.
solution: Customer Journey [!DNL Analytics], [!DNL Analytics]
feature: Integrations
topic: Integrations
role: Developer
level: Experienced
index: true
hidefromtoc: true
kt: null
thumbnail: 13728
last-substantial-update: 2023-04-11T00:00:00Z
badgeIntegration: label="Integrazione" type="positive"
exl-id: e39dac5d-6ad5-47c8-94e8-070011233161
source-git-commit: d35dc06c56c117cffe70542b6713f275877e4879
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 3%

---

# Integrare l&#39;Adobe [!DNL Analytics] e il Percorso clienti [!DNL Analytics] con l&#39;esercitazione di Edge sull&#39;esperienza [!DNL Platform]

<ol>
    <li><a href="https://experienceleague.adobe.com/it?lang=en#dashboard/learning" _target="_blank" rel="noopener noreferrer">Crea schemi</a> per i dati da acquisire.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/data-ingestion/create-datasets-and-ingest-data.html?lang=it" _target="_blank" rel="noopener noreferrer">Crea set di dati</a> per i dati da acquisire.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/identities/label-ingest-and-verify-identity-data.html?lang=it" _target="_blank" rel="noopener noreferrer">Configura le identità e gli spazi dei nomi di identità corretti nello schema</a> per assicurarti che i dati acquisiti possano essere uniti in un profilo unificato.</li> 
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/profiles/bring-data-into-the-real-time-customer-profile.html?lang=it" _target="_blank" rel="noopener noreferrer">Abilitare schemi e set di dati per il profilo</a>.</li>
    <li>Acquisire dati nell'esperienza [!DNL Platform] utilizzando uno dei seguenti metodi:</li>
        <ul>
            <li>Experience [!DNL Platform] Web SDK:</li>
                <ul>
                    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/implement-web-sdk/overview.html?lang=it" _target="_blank" rel="noopener noreferrer">Tutorial</a></li>
                    <li><a href="https://experienceleague.adobe.com/docs/analytics/implementation/aep-edge/web-sdk/overview.html?lang=it" _target="_blank" rel="noopener noreferrer">Elenco di controllo</a></li>
                </ul>
            <li>Experience [!DNL Platform] Mobile SDK:</li>
                <ul>
                    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/data-collection/mobile-sdk/create-mobile-properties.html?lang=it" _target="_blank" rel="noopener noreferrer">Tutorial</a></li>
                    <li><a href="https://experienceleague.adobe.com/docs/analytics/implementation/aep-edge/mobile-sdk/overview.html?lang=it" _target="_blank" rel="noopener noreferrer">Elenco di controllo</a></li>
                </ul></li>
            <li>API server Edge Network:</li>
                <ul>
                    <li><a href="https://experienceleague.adobe.com/docs/experience-platform/edge-network-server-api/interacting-other-adobe-solutions/interacting-adobe-analytics.html?lang=it" _target="_blank" rel="noopener noreferrer">Tutorial</a></li>
                </ul>
       </ul>
    <li><i>(facoltativo)</i>. Se utilizzi più set di dati, unisci l'ID della persona per <a href="https://experienceleague.adobe.com/docs/analytics-platform/using/cja-connections/combined-dataset.html?lang=it" _target="_blank" rel="noopener noreferrer">generare un set di dati combinato</a>. Se utilizzi un singolo set di dati [!DNL Analytics] o se esiste un identificatore comune in tutti i set di dati che intendi utilizzare nel Percorso di clienti [!DNL Analytics], ignora questo passaggio.</li>
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/connections/connecting-customer-journey-analytics-to-data-sources-in-platform.html?lang=it" _target="_blank" rel="noopener noreferrer">Crea una connessione</a> nel Percorso clienti [!DNL Analytics].</li>
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/basic-configuration-for-data-views.html?lang=it" _target="_blank" rel="noopener noreferrer">Creare una visualizzazione dati</a>, <a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/configuring-component-settings-in-data-views.html?lang=it" _target="_blank" rel="noopener noreferrer">configurare le impostazioni del componente</a> e <a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/formatting-metrics-in-data-views.html?lang=it" _target="_blank" rel="noopener noreferrer">formattare le metriche</a> nel Percorso clienti [!DNL Analytics].
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/analysis-workspace/workspace-projects/build-a-new-project.html?lang=it" _target="_blank" rel="noopener noreferrer">Creazione di un progetto nel Percorso di clienti [!DNL Analytics].</a></li>
</ol>

>[!NOTE]
>
>I passaggi standard del flusso di lavoro per il connettore di origine Adobe [!DNL Analytics] creano lo schema e il set di dati utilizzati per acquisire i dati da [!DNL Analytics] &quot;così com&#39;è&quot;. Pertanto, i primi due passaggi vengono gestiti dal sistema. Il flusso di lavoro di mappatura richiede la creazione di attributi personalizzati; pertanto, segui completamente la sequenza di passaggi.
