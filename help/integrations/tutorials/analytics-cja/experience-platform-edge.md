---
title: Integra Adobe [!DNL Analytics] e Percorso di clienti [!DNL Analytics] con l’esperienza [!DNL Platform] Esercitazione su Edge
description: Scopri come integrare Adobe [!DNL Analytics] con il Percorso del cliente [!DNL Analytics] tramite AEP Web SDK, AEP Mobile SDK o l’API del server di rete Edge.
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
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 20%

---


# Integra Adobe [!DNL Analytics] e Percorso di clienti [!DNL Analytics] con l’esperienza [!DNL Platform] Esercitazione su Edge

<ol>
    <li><a href="https://experienceleague.adobe.com/?lang=it#dashboard/learning" _target="_blank" rel="noopener noreferrer">Creare schemi</a> per i dati da inserire.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/data-ingestion/create-datasets-and-ingest-data.html?lang=it" _target="_blank" rel="noopener noreferrer">Creare set di dati</a> per i dati da inserire.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/identities/label-ingest-and-verify-identity-data.html?lang=en" _target="_blank" rel="noopener noreferrer">Configurare le identità e gli spazi dei nomi delle identità corretti nello schema</a> assicurati che i dati acquisiti possano essere uniti a un profilo unificato.</li> 
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/profiles/bring-data-into-the-real-time-customer-profile.html?lang=it" _target="_blank" rel="noopener noreferrer">Abilitare schemi e set di dati per il profilo</a>.</li>
    <li>Inserire dati in Experience [!DNL Platform] utilizzando uno dei seguenti metodi:</li>
        <ul>
            <li>Esperienza [!DNL Platform] SDK per web:</li>
                <ul>
                    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/implement-web-sdk/overview.html?lang=it" _target="_blank" rel="noopener noreferrer">Tutorial</a></li>
                    <li><a href="https://experienceleague.adobe.com/docs/analytics/implementation/aep-edge/web-sdk/overview.html" _target="_blank" rel="noopener noreferrer">Elenco di controllo</a></li>
                </ul>
            <li>Esperienza [!DNL Platform] SDK per dispositivi mobili:</li>
                <ul>
                    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/data-collection/mobile-sdk/create-mobile-properties.html" _target="_blank" rel="noopener noreferrer">Tutorial</a></li>
                    <li><a href="https://experienceleague.adobe.com/docs/analytics/implementation/aep-edge/mobile-sdk/overview.html" _target="_blank" rel="noopener noreferrer">Elenco di controllo</a></li>
                </ul></li>
            <li>API del server di rete Edge:</li>
                <ul>
                    <li><a href="https://experienceleague.adobe.com/docs/experience-platform/edge-network-server-api/interacting-other-adobe-solutions/interacting-adobe-analytics.html?lang=it" _target="_blank" rel="noopener noreferrer">Tutorial</a></li>
                </ul>
       </ul>
    <li><i>(Facoltativo)</i>. Se utilizzi più set di dati, unisci l’ID della persona a <a href="https://experienceleague.adobe.com/docs/analytics-platform/using/cja-connections/combined-dataset.html" _target="_blank" rel="noopener noreferrer">generare un set di dati combinato</a>. Se si utilizza un singolo [!DNL Analytics] set di dati o se esiste un identificatore comune in tutti i set di dati che intendi utilizzare nel Percorso di clienti [!DNL Analytics], salta questo passaggio.</li>
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/connections/connecting-customer-journey-analytics-to-data-sources-in-platform.html?lang=it" _target="_blank" rel="noopener noreferrer"></a>Creare una connessione in Customer Journey [!DNL Analytics].</li>
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/basic-configuration-for-data-views.html" _target="_blank" rel="noopener noreferrer">Creare una visualizzazione dati</a>, <a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/configuring-component-settings-in-data-views.html" _target="_blank" rel="noopener noreferrer">configurare le impostazioni del componente</a>, e <a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/formatting-metrics-in-data-views.html" _target="_blank" rel="noopener noreferrer">formattare le metriche</a> nel Percorso di clienti [!DNL Analytics].
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/analysis-workspace/workspace-projects/build-a-new-project.html" _target="_blank" rel="noopener noreferrer">Creazione di un progetto nel Percorso di clienti [!DNL Analytics].</a></li>
</ol>

>[!NOTE]
>
>Passaggi standard del flusso di lavoro per l’Adobe [!DNL Analytics] connettore di origine crea lo schema e il set di dati utilizzati per acquisire i dati da [!DNL Analytics] &quot;così com&#39;è&quot;. Pertanto, i primi due passaggi vengono gestiti dal sistema. Il flusso di lavoro di mappatura richiede la creazione di attributi personalizzati; pertanto, segui completamente la sequenza di passaggi.
