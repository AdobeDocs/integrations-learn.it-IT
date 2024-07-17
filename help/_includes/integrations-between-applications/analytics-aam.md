---
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---


# Integrazione di [!DNL Analytics] e Audience Manager

{{analytics-description}}

{{audience-manager-description}}

L&#39;abilitazione di questa integrazione, mediante l&#39;inoltro dei dati Adobe [!DNL Analytics] lato server ad Audience Manager, fornisce ad Audience Manager una delle sue principali origini di dati, ovvero i dati comportamentali dei clienti online. Questi dati possono quindi essere combinati con altri dati, come dati di gestione delle relazioni con i clienti di prima parte o dati di partner di terze parti, per creare segmenti avanzati di clienti. Inoltre, i segmenti di Audience Manager vengono quindi rimandati alla pagina web nella risposta per un’ulteriore analisi dei visitatori. Entrambi questi preziosi casi d’uso sono descritti di seguito.

I vantaggi principali dell&#39;integrazione di Adobe [!DNL Analytics] e Audience Manager sono i seguenti:

+ **Segmentazione migliorata**: combina i dati di Adobe [!DNL Analytics] e Audience Manager per segmenti di pubblico precisi e personalizzati nelle campagne di marketing.
+ **Profili cliente unificati**: integra le origini dati per comprendere le interazioni e i comportamenti, creando profili cliente completi.
+ **Miglioramento dell&#39;efficacia degli annunci**: ottimizzazione degli annunci con targeting basato sui dati dall&#39;integrazione di Adobe [!DNL Analytics] e Audience Manager.
+ **Decisioni basate sui dati**: fornisce informazioni dettagliate sulle scelte effettuate, unendo i dati dell&#39;Adobe [!DNL Analytics] e dell&#39;Audience Manager.
+ **Esperienze personalizzate**: personalizza i contenuti e le offerte, arricchendo le interazioni dei clienti nei diversi punti di contatto tramite entrambe le piattaforme.

Nel complesso, questa integrazione riunisce dati preziosi e approfondimenti sul pubblico. Consente alle aziende di creare campagne di marketing più mirate e rilevanti, comprendendo meglio le preferenze e i comportamenti dei clienti.

## Integrazioni comuni

<table>
    <thead>
        <tr>
            <th>applicazioni Experience Cloud</th>
            <th>Integra tramite</th>
            <th>Quando utilizzare</th>
            <th>Casi d’uso comuni</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>
                <a href="/docs/analytics-learn/tutorials/integrations/audience-manager/enable-server-side-forwarding-in-adobe-launch.html" target="_blank" rel="noreferrer">[!DNL Analytics] invio di dati a Audience Manager</a>
            </td>
            <td>Estensione tag Adobe [!DNL Analytics] o AppMeasurement.js con inoltro lato server abilitato</td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Quando si desidera inviare dati Adobe [!DNL Analytics] ad Audience Manager per creare segmenti che possono essere condivisi con altre destinazioni Adobe Experience Cloud, persone o altre destinazioni personalizzate e basate su dispositivi supportate da Audience Manager.</li>
                </ul>
            </td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Condividere segmenti su piattaforme di annunci che includono attributi comportamentali raccolti in [!DNL Analytics].</li>
                    <li>Arricchisci i segmenti con [!DNL Analytics] dati per creare segmenti cross-channel di alto valore da utilizzare nel targeting nel sito.</li>
                    <li>Crea livelli di dati [!DNL Analytics] in segmenti ricavati da identificatori con hash, ad esempio e-mail, da utilizzare nelle piattaforme di social media.</li>
                </ul>
            </td>
        </tr>        
        <tr>
            <td>
                <a href="https://experienceleague.adobe.com/docs/analytics/integration/audience-analytics/mc-audiences-aam.html" target="_blank" rel="noreferrer">Audience Manager di invio dei dati a [!DNL Analytics]</a>
            </td>
            <td>Estensione tag Adobe [!DNL Analytics] o AppMeasurement.js con inoltro lato server abilitato</td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Quando desideri condividere segmenti da Audience Manager a [!DNL Analytics] per informare l'individuazione, la segmentazione e l'ottimizzazione del pubblico.</li>
                </ul>
            </td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Utilizzare segmenti di Audience Manager che includono dati demografici di provider di terze parti nei report [!DNL Analytics].</li>
                    <li>Utilizzare i segmenti di Audience Manager che includono i dati della campagna dai server di annunci nei report [!DNL Analytics].</li>
                    <li>Utilizzare segmenti Audience Manager che includono dati CRM onboarded nei report [!DNL Analytics].</li>
                </ul>
            </td>
        </tr>
    </tbody>
</table>
