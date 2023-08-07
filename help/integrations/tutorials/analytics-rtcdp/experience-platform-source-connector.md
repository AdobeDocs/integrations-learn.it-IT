---
title: Integrare [!DNL Analytics] e dati dei clienti in tempo reale [!DNL Platform] con esperienza [!DNL Platform] esercitazione sul connettore di origine
description: Scopri come integrare Adobe [!DNL Analytics] con Real-Time Customer Data [!DNL Platform] utilizzo dell’esperienza [!DNL Platform] connettore di origine.
solution: Real-Time Customer Data [!DNL Platform], [!DNL Analytics]
feature: Integrations
topic: Integrations
role: Leader, Architect, Admin, Developer
level: Beginner
index: true
hidefromtoc: true
kt: 13728
thumbnail: null
last-substantial-update: 2023-04-11T00:00:00Z
badgeIntegration: label="Integrazione" type="positive"
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 19%

---


# Integra Adobe [!DNL Analytics] e dati dei clienti in tempo reale [!DNL Platform] con esperienza [!DNL Platform] connettore di origine

<ol>
    <li><a href="https://experienceleague.adobe.com/?lang=it#dashboard/learning" _target="_blank" rel="noopener noreferrer">Creare schemi</a> per i dati da inserire.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/data-ingestion/create-datasets-and-ingest-data.html?lang=it" _target="_blank" rel="noopener noreferrer">Creare set di dati</a> per i dati da inserire.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/identities/label-ingest-and-verify-identity-data.html?lang=en" _target="_blank" rel="noopener noreferrer">Configurare le identità e gli spazi dei nomi delle identità corretti nello schema</a> assicurati che i dati acquisiti possano essere uniti a un profilo unificato.</li> 
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/profiles/bring-data-into-the-real-time-customer-profile.html?lang=it" _target="_blank" rel="noopener noreferrer">Abilitare schemi e set di dati per il profilo</a>.</li>
    <li>Acquisisci [!DNL Analytics] dati in Experience Platform utilizzando <a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/sources/ingest-data-from-adobe-analytics.html?lang=it" _target="_blank" rel="noopener noreferrer">Adobe [!DNL Analytics] connettore di origine</a>.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/audiences/create-audiences.html" _target="_blank" rel="noopener noreferrer">Creare segmenti in Experience [!DNL Platform].</a> Il sistema determina automaticamente se il segmento viene valutato come batch (connettore dati) o streaming (rete Edge).</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/destinations/create-destinations-and-activate-data.html" _target="_blank" rel="noopener noreferrer">Configura le destinazioni per la condivisione degli attributi di profilo e delle appartenenze del pubblico nelle destinazioni desiderate.</a></li>   
</ol>

>[!NOTE]
>
>Passaggi standard del flusso di lavoro per l’Adobe [!DNL Analytics] connettore di origine crea lo schema e il set di dati utilizzati per acquisire i dati da [!DNL Analytics] &quot;così com&#39;è&quot;. Pertanto, i primi due passaggi vengono gestiti dal sistema. Il flusso di lavoro di mappatura richiede la creazione di attributi personalizzati; pertanto, segui completamente la sequenza di passaggi.
