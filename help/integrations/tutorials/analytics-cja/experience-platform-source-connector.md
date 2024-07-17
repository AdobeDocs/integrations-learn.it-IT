---
title: Esercitazione Integrare [!DNL Analytics] e Percorso di clienti [!DNL Analytics] con il connettore di origine di Experience [!DNL Platform]
description: Scopri come integrare Adobe [!DNL Analytics] con il Percorso clienti [!DNL Analytics] utilizzando il connettore di origine Experience [!DNL Platform] source.
solution: Customer Journey [!DNL Analytics], [!DNL Target]
feature: Integrations
topic: Integrations
role: Leader, Architect, Admin, Developer
level: Beginner
index: true
hidefromtoc: true
kt: 13727
thumbnail: null
last-substantial-update: 2023-04-11T00:00:00Z
badgeIntegration: label="Integrazione" type="positive"
exl-id: f0dbd59d-d5e5-40e6-b4a4-e4789e7dd7e3
source-git-commit: d35dc06c56c117cffe70542b6713f275877e4879
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 2%

---

# Integra l&#39;Adobe [!DNL Analytics] e il Percorso clienti [!DNL Analytics] con il connettore di origine dell&#39;esperienza [!DNL Platform]

<ol>
    <li><a href="https://experienceleague.adobe.com/?lang=en#dashboard/learning" _target="_blank" rel="noopener noreferrer">Crea schemi</a> per i dati da acquisire.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/data-ingestion/create-datasets-and-ingest-data.html" _target="_blank" rel="noopener noreferrer">Crea set di dati</a> per i dati da acquisire.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/identities/label-ingest-and-verify-identity-data.html?lang=en" _target="_blank" rel="noopener noreferrer">Configura le identità e gli spazi dei nomi di identità corretti nello schema</a> per assicurarti che i dati acquisiti possano essere uniti in un profilo unificato.</li> 
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/profiles/bring-data-into-the-real-time-customer-profile.html?lang=it" _target="_blank" rel="noopener noreferrer">Abilitare schemi e set di dati per il profilo</a>.</li>
    <li>Acquisisci dati nell'esperienza [!DNL Platform] utilizzando il <a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/sources/ingest-data-from-adobe-analytics.html?lang=it" _target="_blank" rel="noopener noreferrer">connettore di origine Adobe [!DNL Analytics]</a></li>
    <li><i>(facoltativo)</i>. Se utilizzi più set di dati, unisci l'ID della persona per <a href="https://experienceleague.adobe.com/docs/analytics-platform/using/cja-connections/combined-dataset.html" _target="_blank" rel="noopener noreferrer">generare un set di dati combinato</a>. Se utilizzi un singolo set di dati [!DNL Analytics] o se esiste un identificatore comune in tutti i set di dati che intendi utilizzare nel Percorso di clienti [!DNL Analytics], ignora questo passaggio.</li>
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/connections/connecting-customer-journey-analytics-to-data-sources-in-platform.html?lang=it" _target="_blank" rel="noopener noreferrer">Crea una connessione</a> nel Percorso clienti [!DNL Analytics].</li>
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/basic-configuration-for-data-views.html" _target="_blank" rel="noopener noreferrer">Creare una visualizzazione dati</a>, <a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/configuring-component-settings-in-data-views.html" _target="_blank" rel="noopener noreferrer">configurare le impostazioni del componente</a> e <a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/formatting-metrics-in-data-views.html" _target="_blank" rel="noopener noreferrer">formattare le metriche</a> nel Percorso clienti [!DNL Analytics].
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/analysis-workspace/workspace-projects/build-a-new-project.html?lang=it" _target="_blank" rel="noopener noreferrer">Creazione di un progetto nel Percorso di clienti [!DNL Analytics].</a></li>
</ol>

>[!NOTE]
>
>I passaggi standard del flusso di lavoro per il connettore di origine Adobe [!DNL Analytics] creano lo schema e il set di dati utilizzati per acquisire i dati da [!DNL Analytics] &quot;così com&#39;è&quot;. Pertanto, i primi due passaggi vengono gestiti dal sistema. Il flusso di lavoro di mappatura richiede la creazione di attributi personalizzati; pertanto, segui completamente la sequenza di passaggi.
