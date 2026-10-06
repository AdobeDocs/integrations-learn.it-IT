---
title: Integrare [!DNL Analytics] e Real-Time Customer Data [!DNL Platform] con l'esercitazione di Experience [!DNL Platform] Edge
description: Scopri come integrare Adobe [!DNL Analytics] con Real-Time Customer Data [!DNL Platform] utilizzando AEP Web SDK, AEP Mobile SDK o l'API server di Edge Network.
solution: Real-Time Customer Data Platform, Analytics
feature: Integrations
topic: Integrations
role: Developer
level: Experienced
index: true
kt: 13732
thumbnail:
last-substantial-update: 2023-04-11T00:00:00.000Z
badgeIntegration: label="Integrazione" type="positive"
exl-id: 07c2c329-0810-4f66-a91a-e315695f3fb4
TQID: 'https://experienceleague.adobe.com/K1CpRtUekl5jQNDMGswJpexC9fv9uVmgraLlNFXUIr8'
product_v2:
  - id: e55547f1-a1ff-40c6-8978-026e40ab7fa4
    internal-label: Analytics
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
    internal-label: Real-Time Customer Data Platform
feature_v2:
  - id: eb9732ab-8232-4b21-bc4c-89de86dbe4d7
    internal-label: Integrations
  - id: fd307ce7-56f5-4ee3-af68-a7833ff6e85e
    internal-label: API
subfeature_v2:
  - id: e6c28e30-8689-4bf4-8fa8-561343d308a9
    internal-label: Experience Cloud integration
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
level_v2:
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
    internal-label: Experienced
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
    internal-label: Implementation
source-git-commit: 4c51eef6f89060dc633dede5ea23e0f3ab445d0b
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 8%
---
# Esercitazione sull&#39;integrazione di Adobe [!DNL Analytics] e Real-Time Customer Data [!DNL Platform] con Experience [!DNL Platform] Edge

<ol>
    <li><a href="https://experienceleague.adobe.com/?lang=en#dashboard/learning" _target="_blank" rel="noopener noreferrer">Crea schemi</a> per i dati da acquisire.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/data-ingestion/create-datasets-and-ingest-data.html" _target="_blank" rel="noopener noreferrer">Crea set di dati</a> per i dati da acquisire.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/identities/label-ingest-and-verify-identity-data.html?lang=en" _target="_blank" rel="noopener noreferrer">Configura le identità e gli spazi dei nomi di identità corretti nello schema</a> per assicurarti che i dati acquisiti possano essere uniti in un profilo unificato.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/profiles/bring-data-into-the-real-time-customer-profile.html?lang=it" _target="_blank" rel="noopener noreferrer">Abilitare schemi e set di dati per il profilo</a>.</li>
    <li>Acquisire dati nell'esperienza [!DNL Platform] utilizzando uno dei seguenti metodi:</li>
        <ul>
           <li>Esperienza [!DNL Platform] Web SDK:</li>
                <ul>
                    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/implement-web-sdk/overview.html?lang=it" _target="_blank" rel="noopener noreferrer">Tutorial</a></li>
                    <li><a href="https://experienceleague.adobe.com/docs/analytics/implementation/aep-edge/web-sdk/overview.html" _target="_blank" rel="noopener noreferrer">Elenco di controllo</a></li>
                </ul>
            <li>Esperienza [!DNL Platform] Mobile SDK:</li>
                <ul>
                    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/data-collection/mobile-sdk/create-mobile-properties.html" _target="_blank" rel="noopener noreferrer">Tutorial</a></li>
                    <li><a href="https://experienceleague.adobe.com/docs/analytics/implementation/aep-edge/mobile-sdk/overview.html" _target="_blank" rel="noopener noreferrer">Elenco di controllo</a></li>
                </ul></li>
            <li>API server di Edge Network:</li>
                <ul>
                    <li><a href="https://experienceleague.adobe.com/docs/experience-platform/edge-network-server-api/interacting-other-adobe-solutions/interacting-adobe-analytics.html" _target="_blank" rel="noopener noreferrer">Tutorial</a></li>
                </ul>
       </ul>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/segments/create-segments.html" _target="_blank" rel="noopener noreferrer">Crea segmenti nell'esperienza [!DNL Platform].</a> Il sistema determina automaticamente se il segmento viene valutato come batch (connettore dati) o streaming (rete Edge).</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/destinations/create-destinations-and-activate-data.html" _target="_blank" rel="noopener noreferrer">Configura le destinazioni per la condivisione degli attributi di profilo e delle appartenenze del pubblico nelle destinazioni desiderate.</a></li>
</ol>

>[!NOTE]
>
>I passaggi standard del flusso di lavoro per il connettore di origine [!DNL Analytics] di Adobe creano lo schema e il set di dati utilizzati per acquisire i dati da [!DNL Analytics] &quot;così come sono&quot;. Pertanto, i primi due passaggi vengono gestiti dal sistema. Il flusso di lavoro di mappatura richiede la creazione di attributi personalizzati; pertanto, segui completamente la sequenza di passaggi.
