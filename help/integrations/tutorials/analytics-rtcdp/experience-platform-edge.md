---
title: Integra [!DNL Analytics] e Real-Time Customer Data [!DNL Platform] con l'esercitazione di Experience [!DNL Platform] Edge
description: Scopri come integrare Adobe [!DNL Analytics] con Real-Time Customer Data [!DNL Platform] utilizzando AEP Web SDK, AEP Mobile SDK o l'API server di Edge Network.
solution: Real-Time Customer Data Platform, Analytics
feature: Integrations
topic: Integrations
role: Developer
level: Experienced
index: true
kt: 13732
thumbnail: null
last-substantial-update: 2023-04-11T00:00:00.000Z
badgeIntegration: label="Integrazione" type="positive"
exl-id: 07c2c329-0810-4f66-a91a-e315695f3fb4
TQID: https://experienceleague.adobe.com/K1CpRtUekl5jQNDMGswJpexC9fv9uVmgraLlNFXUIr8
product_v2:
  - id: e55547f1-a1ff-40c6-8978-026e40ab7fa4
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
feature_v2:
  - id: eb9732ab-8232-4b21-bc4c-89de86dbe4d7
  - id: fd307ce7-56f5-4ee3-af68-a7833ff6e85e
subfeature_v2:
  - id: e6c28e30-8689-4bf4-8fa8-561343d308a9
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
source-git-commit: 2a324011b3d235db3d4642c2797c4fa107267e6a
workflow-type: tm+mt
source-wordcount: 317
ht-degree: 8%

---

# Esercitazione sull&#39;integrazione di Adobe [!DNL Analytics] e Real-Time Customer Data [!DNL Platform] con Experience [!DNL Platform] Edge

<ol>
    <li><a href="https://experienceleague.adobe.com/it?lang=en#dashboard/learning" _target="_blank" rel="noopener noreferrer">Crea schemi</a> per i dati da acquisire.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/data-ingestion/create-datasets-and-ingest-data.html?lang=it" _target="_blank" rel="noopener noreferrer">Crea set di dati</a> per i dati da acquisire.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/identities/label-ingest-and-verify-identity-data.html?lang=it" _target="_blank" rel="noopener noreferrer">Configura le identità e gli spazi dei nomi di identità corretti nello schema</a> per assicurarti che i dati acquisiti possano essere uniti in un profilo unificato.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/profiles/bring-data-into-the-real-time-customer-profile.html?lang=it" _target="_blank" rel="noopener noreferrer">Abilitare schemi e set di dati per il profilo</a>.</li>
    <li>Acquisire dati nell'esperienza [!DNL Platform] utilizzando uno dei seguenti metodi:</li>
        <ul>
           <li>Esperienza [!DNL Platform] Web SDK:</li>
                <ul>
                    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/implement-web-sdk/overview.html?lang=it" _target="_blank" rel="noopener noreferrer">Tutorial</a></li>
                    <li><a href="https://experienceleague.adobe.com/docs/analytics/implementation/aep-edge/web-sdk/overview.html?lang=it" _target="_blank" rel="noopener noreferrer">Elenco di controllo</a></li>
                </ul>
            <li>Esperienza [!DNL Platform] Mobile SDK:</li>
                <ul>
                    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/data-collection/mobile-sdk/create-mobile-properties.html?lang=it" _target="_blank" rel="noopener noreferrer">Tutorial</a></li>
                    <li><a href="https://experienceleague.adobe.com/docs/analytics/implementation/aep-edge/mobile-sdk/overview.html?lang=it" _target="_blank" rel="noopener noreferrer">Elenco di controllo</a></li>
                </ul></li>
            <li>API server di Edge Network:</li>
                <ul>
                    <li><a href="https://experienceleague.adobe.com/docs/experience-platform/edge-network-server-api/interacting-other-adobe-solutions/interacting-adobe-analytics.html?lang=it" _target="_blank" rel="noopener noreferrer">Tutorial</a></li>
                </ul>
       </ul>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/segments/create-segments.html?lang=it" _target="_blank" rel="noopener noreferrer">Crea segmenti nell'esperienza [!DNL Platform].</a> Il sistema determina automaticamente se il segmento viene valutato come batch (connettore dati) o streaming (rete Edge).</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/destinations/create-destinations-and-activate-data.html?lang=it" _target="_blank" rel="noopener noreferrer">Configura le destinazioni per la condivisione degli attributi di profilo e delle appartenenze del pubblico nelle destinazioni desiderate.</a></li>
</ol>

>[!NOTE]
>
>I passaggi standard del flusso di lavoro per il connettore di origine [!DNL Analytics] di Adobe creano lo schema e il set di dati utilizzati per acquisire i dati da [!DNL Analytics] &quot;così come sono&quot;. Pertanto, i primi due passaggi vengono gestiti dal sistema. Il flusso di lavoro di mappatura richiede la creazione di attributi personalizzati; pertanto, segui completamente la sequenza di passaggi.
