---
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '305'
ht-degree: 0%

---


# Integrare l&#39;Adobe [!DNL Analytics] con Real-Time Customer Data [!DNL Platform]

{{analytics-description}}

{{real-time-cdp-description}}

L&#39;integrazione di Adobe [!DNL Analytics] con Adobe Real-Time Customer Data [!DNL Platform] (Real-Time CDP) può offrire diversi vantaggi alle aziende che desiderano migliorare le esperienze dei clienti e le attività di marketing. Di seguito sono riportati alcuni dei principali vantaggi:

+ **Personalizzazione e targeting del pubblico migliorati**: marketing preciso su dispositivi e canali, messaggi personalizzati per un coinvolgimento ottimizzato.
+ **Miglioramento dell&#39;ottimizzazione della pagina di destinazione**: esperienze personalizzate in base al dispositivo e al comportamento, che migliorano la soddisfazione e la conversione degli utenti.
+ **Perfetta attivazione del pubblico**: utilizza i profili dei clienti per un targeting efficace attraverso i canali preferiti, distribuendo messaggi pertinenti.

Combinando Adobe [!DNL Analytics] e Real-Time CDP, le aziende possono portare le loro attività di marketing a un livello superiore, offrendo esperienze personalizzate, aumentando il coinvolgimento dei clienti e ottimizzando le conversioni in vari punti di contatto digitali.

<table>
    <thead>
        <tr>
            <th>applicazioni Experience Cloud</th>
            <th>Integra tramite</th>
            <th>Quando utilizzare</th>
            <th>Casi d’uso comuni</th>
        </tr>
    </thead>
    <tr>
        <td rowspan="2">[!DNL Analytics] con Real-Time CDP</td>
        <td><a href="../../integrations/tutorials/analytics-rtcdp/experience-platform-source-connector.md" target="_blank" rel="noreferrer">Connettore di origine dell'esperienza [!DNL Platform]</a></td>
        <td>
            <ul style="margin-top: 0;">
                <li>Approccio consigliato per i clienti che hanno già implementato l'Adobe [!DNL Analytics] e desiderano che il modo più veloce per acquisire questi dati nell'esperienza [!DNL Platform] sia utilizzato nel profilo cliente in tempo reale.</li>
                <li>Quando la disponibilità dei dati per Real-Time Customer Profile può essere compresa tra 2 e 30 minuti dal momento della raccolta dei dati e la disponibilità per Data Lake può arrivare a 90 minuti.</li>
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
       <td><a href="../../integrations/tutorials/analytics-rtcdp/experience-platform-edge.md" target="_blank" rel="noreferrer">Esperienza [!DNL Platform] Edge</a></td>
        <td>
            <ul style="margin-top: 0;">
                <li>Approccio consigliato per le nuove implementazioni di [!DNL Analytics] o per implementare una strategia a lungo termine.</li>
                <li>Invia dati direttamente da un dispositivo all'esperienza [!DNL Platform] tramite AEP Web SDK, AEP Mobile SDK o l'API server Edge Network.</li>
                <li>Clienti nuovi o esistenti che necessitano della disponibilità dei dati [!DNL Analytics] per Real-Time Customer Profile per supportare casi d'uso per la personalizzazione della pagina corrente e successiva.</li>
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
</table>
