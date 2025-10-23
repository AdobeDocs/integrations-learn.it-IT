---
title: Integrazioni di applicazioni per la personalizzazione su larga scala
description: Rendi le esperienze personalizzate parte di ogni momento.
exl-id: 6d18813d-950c-40ae-8d5b-80bf389358fc
source-git-commit: 132c892723d29d415d07093ef8514ff8c9b7b1db
workflow-type: tm+mt
source-wordcount: '533'
ht-degree: 1%

---

# Personalization su larga scala

In un panorama altamente competitivo e guidato dalla tecnologia digitale di oggi, i clienti si aspettano esperienze personalizzate in base alle loro preferenze ed esigenze specifiche. Sfruttando le funzionalità di Adobe Experience Cloud possiamo raccogliere e analizzare numerosi dati sui clienti, fornendo informazioni preziose su comportamenti, interessi e preferenze. Questa profonda comprensione facilita la consegna di esperienze personalizzate attraverso vari punti di contatto, garantendo interazioni significative e coinvolgenti. Sfruttare la potenza di Adobe Experience Cloud sfrutta appieno il potenziale della personalizzazione, promuovendo connessioni più solide con i clienti, coltivando la fedeltà e guidando la crescita del business.

<table>
 <thead>
    <tr>
      <th>Caso d’uso</th>
      <th>Descrizione</th>
      <th>Esempi</th>
      <th>Applicazioni</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>Creazione di documenti PDF personalizzati</strong></td>
      <td>
        Genera documenti di comunicazione per la firma in base all'utente
        selezioni/preferenze.
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>
            Presentare un NDA generato in modo dinamico in base ai dati provenienti da un’AEM
            Invio Forms per la firma
          </li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/experience-manager/experience-manager-acrobat-sign.md"
          target="_blank"
          rel="noopener noreferrer"
          >AEM Forms e Sign</a
        >
      </td>
    </tr>
    <tr>
      <td rowspan="2"><strong>Analisi dei dati e reporting</strong></td>
      <td>
        Analizza dati comportamentali da esperienze digitali <br />Usa Adobe
        [!DNL Analytics] dati comportamentali in Analysis Workspace nel Percorso clienti
        [!DNL Analytics].
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>Analisi dei percorsi di conversione superiore/inferiore</li>
          <li>Analizzare il coinvolgimento e la conversione dei canali</li>
          <li>Comprendere il contenuto visualizzato più in alto</li>
          <li>Comprendere le categorie e i prodotti principali</li>
          <li>
            Eseguire analisi dell’utilizzo degli strumenti per ottimizzare le esperienze self-service
          </li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/analytics/analytics-customer-journey-analytics.md"
          target="_blank"
          rel="noopener noreferrer"
          >[!DNL Analytics] e Percorso clienti [!DNL Analytics]</a
        >
      </td>
    </tr>
    <tr>
      <td>
        Generazione di rapporti per le attività di personalizzazione<br />Analisi dell'ottimizzazione
        risultati di test, inclusi test A/B, utilizzando Adobe [!DNL Target] e
        generazione di report completi tramite Adobe [!DNL Analytics].
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>Mostrare i risultati del test A/B nei rapporti di analisi avanzati</li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/analytics/analytics-target.md"
          target="_blank"
          rel="noopener noreferrer"
          >[!DNL Analytics] e [!DNL Target]</a
        >
      </td>
    </tr>
    <tr>
      <td><strong>Personalizzare le consegne e-mail</strong></td>
      <td>
        Personalizzare le consegne e-mail con contenuti dinamici sfruttando
        funzionalità di Adobe [!DNL Target].
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>Aggiungere offerte personalizzate alle e-mail dei clienti</li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/campaign//campaign-target.md"
          target="_blank"
          rel="noopener noreferrer"
          >[!DNL Campaign] e [!DNL Target]</a
        >
      </td>
    </tr>
    <tr>
      <td rowspan="2">
        <strong>Espandi tipi di pubblico per piattaforme di personalizzazione e annunci</strong>
      </td>
      <td>
        Utilizzare i segmenti di Audience Manager per creare tipi di pubblico in Real-Time CDP per
        da utilizzare nelle tattiche di personalizzazione e remarketing.
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>
            Eseguire il targeting e la personalizzazione anonimi del pubblico digitale su
            sul sito web, sull’app mobile o sui canali pubblicitari supportati
          </li>
          <li>
            Ottimizza la pagina di destinazione e le esperienze di preautenticazione in base a
            caratteristiche note del dispositivo e del comportamento
          </li>
          <li>
            Sfruttare la rete dati di terze parti di Audience Manager per ulteriori
            perfeziona ed espandi i tipi di pubblico per il targeting
          </li>
          <li>Condividere segmenti di Audience Manager con RTCDP</li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/aam/aam-rtcdp.md"
          target="_blank"
          rel="noopener noreferrer"
          >Dati dei clienti in tempo reale e Audience Manager [!DNL Platform]</a
        >
      </td>
    </tr>
    <tr>
      <td>
        Utilizza i dati di [!DNL Analytics] per creare tipi di pubblico da utilizzare nella personalizzazione o
        tattiche di remarketing.
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>
            Eseguire il targeting e la personalizzazione del pubblico digitale su dispositivi o
            canali pubblicitari supportati.
          </li>
          <li>
            Ottimizzare le pagine di destinazione note dei clienti ed esperienze anonime
            in base agli attributi del dispositivo e del comportamento.
          </li>
          <li>Attiva i tipi di pubblico su canali noti, ad esempio e-mail e SMS.</li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/analytics/analytics-customer-journey-analytics.md"
          target="_blank"
          rel="noopener noreferrer"
          >[!DNL Analytics] e dati cliente in tempo reale [!DNL Platform]</a
        >
      </td>
    </tr>
    <tr>
      <td rowspan="2"><strong>Personalizzare le esperienze web</strong></td>
      <td>
        Personalizzare le esperienze delle applicazioni a pagina singola (SPA) in modo efficace
        utilizzo di AEM Headless in combinazione con Adobe [!DNL Target].
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>Personalizzazione di applicazioni a pagina singola e app mobile</li>
          <li>Risposte API personalizzate.</li>
          <li>[!DNL Target]Consegna di contenuti end-to-end.</li>
          <li>Variazioni del test A/B.</li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/experience-manager/experience-manager-target.md"
          target="_blank"
          rel="noopener noreferrer"
          >AEM Headless e [!DNL Target]</a
        >
      </td>
    </tr>
    <tr>
      <td>
        Fornire esperienze web personalizzate utilizzando in modo efficace AEM Sites
        e Adobe [!DNL Target] per la personalizzazione.
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>Personalizzazione del sito web AEM.</li>
          <li>Variazioni del test A/B.</li>
          <li>Targeting comportamentale basato sul comportamento dell’utente.</li>
          <li>Personalizzazione utente nota mediante l’unione dei dati utente provenienti da più sistemi per fornire una visualizzazione a 360 gradi del cliente.</li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/experience-manager/experience-manager-target.md"
          target="_blank"
          rel="noopener noreferrer"
          >AEM Sites e [!DNL Target]</a
        >
      </td>
    </tr>
    <tr>
      <td><strong>Personalizzare le esperienze digitali</strong></td>
      <td>
        Utilizza profili cliente in tempo reale e segmenti [!DNL Platform] gestiti centralmente
        per personalizzare la messaggistica su web, dispositivi mobili e altri canali digitali
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>Personalizzazione dei contenuti per i visitatori noti</li>
          <li>Aumentare l’iscrizione e la partecipazione dei clienti fidelizzati</li>
          <li>Identificare e coinvolgere i clienti a rischio di abbandono</li>
          <li>Personalizzazione delle offerte in tempo reale</li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/rtcdp/rtcdp-target.md"
          target="_blank"
          rel="noopener noreferrer"
          >Dati cliente in tempo reale [!DNL Platform] e [!DNL Target]</a
        >
      </td>
    </tr>
    <tr>
      <td><strong>Migliora la generazione di lead</strong></td>
      <td>
        Utilizza profili cliente in tempo reale e segmenti [!DNL Platform] gestiti centralmente
        per personalizzare la messaggistica su web, dispositivi mobili e altri canali digitali
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>Personalizzazione dei contenuti per i visitatori noti</li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/rtcdp/rtcdp-target.md"
          target="_blank"
          rel="noopener noreferrer"
          >Dati cliente in tempo reale [!DNL Platform] e [!DNL Target]</a
        >
      </td>
    </tr>
  </tbody>
</table>
