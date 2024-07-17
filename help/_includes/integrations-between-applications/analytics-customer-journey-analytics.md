---
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 1%

---


# Integrare l&#39;Adobe [!DNL Analytics] con il Percorso clienti [!DNL Analytics]

{{analytics-description}}

{{customer-journey-analytics-description}}

L&#39;integrazione dell&#39;Adobe [!DNL Analytics] con il Percorso di clienti [!DNL Analytics] offre vantaggi chiave:

+ **Informazioni complete** sui comportamenti e le preferenze dei clienti.
+ **Monitoraggio cross-channel perfetto** per una visualizzazione olistica.
+ **Dati unificati e reporting** per analisi accurate.
+ **Personalizzazione avanzata** e coinvolgimento del cliente migliorato.
+ **Informazioni sui dati in tempo reale** per un processo decisionale agile.

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
            <td rowspan="2">[!DNL Analytics] e Percorso di clienti [!DNL Analytics]</td>
            <td><a href="../../integrations/tutorials/analytics-cja/experience-platform-source-connector.md" target="_blank" rel="noreferrer">Connettore di origine dell'esperienza [!DNL Platform]</a></td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Approccio consigliato per i clienti che hanno già implementato l'Adobe [!DNL Analytics] e desiderano che il modo più veloce per acquisire questi dati nell'esperienza [!DNL Platform] sia utilizzato nel Percorso di clienti [!DNL Analytics].</li>
                    <li>Quando la disponibilità dei dati per il profilo cliente può essere compresa tra 2 e 30 minuti dal momento della raccolta dei dati e la disponibilità per il Data Lake può arrivare a 90 minuti.</li>
                </ul>
            </td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Flusso di lavoro semplice e avviato dall'interfaccia utente.</li>
                    <li>Mappatura dell'interfaccia utente per copiare [!DNL Analytics] proprietà ed eVar in nuovi campi XDM.</li>
                    <li>Il modo più rapido per ottenere valore dal profilo cliente in tempo reale e dal Percorso di clienti [!DNL Analytics].</li>
                </ul>
            </td>
        </tr>
        <tr>
            <td><a href="../../integrations/tutorials/analytics-cja/experience-platform-edge.md" target="_blank" rel="noreferrer">Esperienza [!DNL Platform] Edge</a></td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Approccio consigliato per le nuove implementazioni di [!DNL Analytics] o per implementare una strategia a lungo termine.</li>
                    <li>Invia dati direttamente da un dispositivo all'esperienza [!DNL Platform] tramite AEP Web SDK, AEP Mobile SDK o l'API server Edge Network.</li>
                </ul>
            </td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Fornisce il massimo livello di controllo per i dati raccolti da utilizzare per supportare i casi d’uso.</li>
                    <li>I dati lato client vengono facilmente mappati sui campi XDM.</li>
                    <li>Disponibilità dei dati più rapida per Real-Time Customer Profile.</li>
                </ul>
            </td>
        </tr>  
    </tbody>          
</table>
