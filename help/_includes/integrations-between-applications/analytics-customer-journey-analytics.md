---
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 2%

---


# Integra Adobe [!DNL Analytics] con il Percorso del cliente [!DNL Analytics]

{{analytics-description}}

{{customer-journey-analytics-description}}

Integrazione dell’Adobe [!DNL Analytics] con il Percorso del cliente [!DNL Analytics] offre i seguenti vantaggi:

+ **Informazioni complete** nei comportamenti e nelle preferenze del cliente.
+ **Tracciamento cross-channel perfetto** per una visione olistica.
+ **Dati e reporting unificati** per analisi accurate.
+ **Personalizzazione avanzata** e un maggiore coinvolgimento dei clienti.
+ **Informazioni sui dati in tempo reale** agile processo decisionale.

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
            <td><a href="../../integrations/tutorials/analytics-cja/experience-platform-source-connector.md" target="_blank" rel="noreferrer">Esperienza [!DNL Platform] connettore di origine</a></td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Approccio consigliato per i clienti che hanno già implementato Adobe [!DNL Analytics]e desideri il modo più veloce per acquisire tali dati in Experience [!DNL Platform] da utilizzare nel Percorso di clienti [!DNL Analytics].</li>
                    <li>Quando la disponibilità dei dati per il profilo cliente può essere compresa tra 2 e 30 minuti dal momento della raccolta dei dati e la disponibilità per il Data Lake può arrivare a 90 minuti.</li>
                </ul>
            </td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Flusso di lavoro semplice e avviato dall'interfaccia utente.</li>
                    <li>Mappatura dell'interfaccia utente da copiare [!DNL Analytics] proprietà ed eVar per nuovi campi XDM.</li>
                    <li>Il modo più rapido per ottenere valore dal profilo cliente in tempo reale e dal Percorso di clienti [!DNL Analytics].</li>
                </ul>
            </td>
        </tr>
        <tr>
            <td><a href="../../integrations/tutorials/analytics-cja/experience-platform-edge.md" target="_blank" rel="noreferrer">Esperienza [!DNL Platform] Bordo</a></td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Approccio consigliato per le nuove [!DNL Analytics] o quando desideri implementare una strategia a lungo termine.</li>
                    <li>Invia dati direttamente da un dispositivo all'esperienza [!DNL Platform] tramite AEP Web SDK, AEP Mobile SDK o l’API del server di rete Edge.</li>
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
