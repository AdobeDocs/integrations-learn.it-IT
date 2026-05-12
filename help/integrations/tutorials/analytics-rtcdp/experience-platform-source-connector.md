---
title: 'Esercitazione sull''integrazione di [!DNL Analytics] e Real-Time Customer Data [!DNL Platform] con il connettore di origine di Experience [!DNL Platform] '
description: Scopri come integrare Adobe [!DNL Analytics] con Real-Time Customer Data [!DNL Platform] utilizzando il connettore di origine di Experience [!DNL Platform] source.
solution: Real-Time Customer Data Platform, Analytics
feature: Integrations
topic: Integrations
role: Leader, Admin, Developer
level: Beginner
index: true
kt: 13728
thumbnail: null
last-substantial-update: 2023-04-11T00:00:00.000Z
badgeIntegration: label="Integrazione" type="positive"
exl-id: 1e27555d-e609-4a04-91ca-9518898ad699
TQID: https://experienceleague.adobe.com/Uct30-UadP-2Ocwslbk-dMAV0Y2unZlA339hThnofpA
product_v2: id: e55547f1-a1ff-40c6-8978-026e40ab7fa4id: fdddec33-c9cb-4459-b8b6-2664395a6f10
feature_v2: id: eb9732ab-8232-4b21-bc4c-89de86dbe4d7
subfeature_v2: id: e6c28e30-8689-4bf4-8fa8-561343d308a9
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bdid: f8a45b24-4be7-4f1b-909b-60d06b483a20id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
source-git-commit: 2a324011b3d235db3d4642c2797c4fa107267e6a
workflow-type: tm+mt
source-wordcount: 248
ht-degree: 11%

---

# Integrare Adobe [!DNL Analytics] e Real-Time Customer Data [!DNL Platform] con il connettore di origine di Experience [!DNL Platform]

<ol>
    <li><a href="https://experienceleague.adobe.com/?lang=en#dashboard/learning" _target="_blank" rel="noopener noreferrer">Crea schemi</a> per i dati da acquisire.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/data-ingestion/create-datasets-and-ingest-data.html" _target="_blank" rel="noopener noreferrer">Crea set di dati</a> per i dati da acquisire.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/identities/label-ingest-and-verify-identity-data.html?lang=en" _target="_blank" rel="noopener noreferrer">Configura le identità e gli spazi dei nomi di identità corretti nello schema</a> per assicurarti che i dati acquisiti possano essere uniti in un profilo unificato.</li> 
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/profiles/bring-data-into-the-real-time-customer-profile.html?lang=it" _target="_blank" rel="noopener noreferrer">Abilitare schemi e set di dati per il profilo</a>.</li>
    <li>Acquisire dati [!DNL Analytics] in Experience Platform utilizzando il <a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/sources/ingest-data-from-adobe-analytics.html?lang=it" _target="_blank" rel="noopener noreferrer">connettore di origine [!DNL Analytics] di Adobe</a>.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/audiences/create-audiences.html" _target="_blank" rel="noopener noreferrer">Crea segmenti nell'esperienza [!DNL Platform].</a> Il sistema determina automaticamente se il segmento viene valutato come batch (connettore dati) o streaming (rete Edge).</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/destinations/create-destinations-and-activate-data.html" _target="_blank" rel="noopener noreferrer">Configura le destinazioni per la condivisione degli attributi di profilo e delle appartenenze del pubblico nelle destinazioni desiderate.</a></li>   
</ol>

>[!NOTE]
>
>I passaggi standard del flusso di lavoro per il connettore di origine [!DNL Analytics] di Adobe creano lo schema e il set di dati utilizzati per acquisire i dati da [!DNL Analytics] &quot;così come sono&quot;. Pertanto, i primi due passaggi vengono gestiti dal sistema. Il flusso di lavoro di mappatura richiede la creazione di attributi personalizzati; pertanto, segui completamente la sequenza di passaggi.
