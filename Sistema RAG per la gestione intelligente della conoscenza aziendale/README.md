# Sistema RAG per la gestione intelligente della conoscenza aziendale

## Descrizione del progetto

L'azienda **DataPulse S.p.A.** è una media impresa tecnologica che fornisce soluzioni software per il settore finanziario. DataPulse gestisce una grande quantità di documentazione interna: manuali operativi, policy di compliance, report di progetto, email tecniche, FAQ e knowledge base dei team di prodotto. Spesso i dipendenti impiegano tempo significativo per trovare risposte aggiornate e verificate, con rischio di decisioni basate su informazioni obsolete o non tracciate.

Il progetto "Sistema RAG per la gestione intelligente della conoscenza aziendale" ha l'obiettivo di progettare e sviluppare un backend in Python che permetta di interrogare la documentazione aziendale in linguaggio naturale. Il sistema dovrà prevedere ingestion, indicizzazione e retrieval ibrido dei documenti e una pipeline che costruisce dinamicamente richieste a un LLM per generare risposte sintetiche, affidabili e tracciabili alle fonti.

## Caso d'uso realistico

Scenario: un product manager chiede via chat "Qual è la procedura aggiornata per la richiesta di accesso ai dati dei clienti e quali normative dobbiamo rispettare?"  
Il sistema deve:
- recuperare i documenti aziendali pertinenti (policy, guide operative, registro dei consensi),
- combinare il materiale rilevante e generare una risposta sintetica che riassuma la procedura e le normative applicabili,
- fornire riferimenti tracciabili alle sezioni di documento (o ai documenti stessi) usate per costruire la risposta,
- indicare il livello di confidenza e le date di validità delle fonti.

Questo flusso riduce i tempi di ricerca, aumenta la conformità normativa e migliora l'affidabilità delle decisioni aziendali.

## Importanza per l'azienda

- Riduzione del tempo impiegato per reperire informazioni critiche.
- Diminuzione del rischio operativo e legale grazie a risposte tracciabili e basate su fonti verificate.
- Migliore sfruttamento del patrimonio informativo aziendale (documenti non strutturati).
- Supporto alle attività di onboarding e formazione interna.
- Incremento della produttività e della qualità delle decisioni.

## Benefici e valore aggiunto

- Risposte sintetiche e mirate: consentono agli utenti di ottenere rapidamente le informazioni essenziali.
- Tracciabilità delle fonti: ogni risposta è accompagnata da riferimenti che permettono la verifica manuale.
- Consolidamento della conoscenza aziendale: un’unica interfaccia per interrogare diversi repository documentali.
- Abilitazione di workflow automatizzati (es. ticketing, escalation) basati su informazioni affidabili.
- Valore strategico: dati e documenti diventano asset utilizzabili per analytics e miglioramento continuo.

## Ambito del progetto (scope)

Il progetto comprende le seguenti aree funzionali ad alto livello:
- Raccolta e ingestion dei documenti aziendali (file, repository, archivi).
- Normalizzazione e arricchimento meta-dati (senza specificare tecniche).
- Indicizzazione e organizzazione per retrieval ibrido (testo + metadati).
- Motore di retrieval che supporta query in linguaggio naturale.
- Pipeline di generazione della richiesta verso un LLM che costruisce risposte sintetiche.
- Sistema di tracciamento delle fonti e di reporting della confidenza.
- Interfaccia di demo (documentazione e notebook) per mostrare il funzionamento.

## Requisiti funzionali 

1. Ingestion
   - Accettare insiemi di documenti eterogenei (per questo esempio didattico vanno bene dei semplici file di testo).
   - Conservare metadati essenziali (data, origine).

2. Indicizzazione
   - Consentire l'accesso ai contenuti per retrieval efficiente su base testuale e meta-informativa.

3. Retrieval ibrido
   - Supportare ricerche che combinano pertinenza semantica e segnali strutturati (metadati, data).

4. Pipeline di generazione
   - Costruire dinamicamente richieste verso un LLM utilizzando i risultati del retrieval.
   - Generare risposte sintetiche, includendo riassunti e punti chiave.

5. Tracciabilità e provenienza
   - Allegare a ogni risposta l'elenco delle fonti utilizzate.
   - Fornire un indicatore di confidenza relativo alla risposta.



## Criteri di accettazione

- Il sistema risponde a query in linguaggio naturale restituendo:
  - testo sintetico di risposta,
  - elenco delle fonti utilizzate con riferimenti chiari,
  - metrica di confidenza e timestamp delle fonti.
- La documentazione spiega come eseguire e validare i principali flussi.
- Test di esempio coprono i casi d'uso principali descritti nel progetto.



## Valore commerciale e impatto operativo

- Miglioramento dell’efficienza operativa e riduzione dei tempi di ricerca.
- Riduzione dei rischi legati a informazioni non aggiornate o non tracciate.
- Miglioramento della qualità del servizio interno e dell’esperienza dei dipendenti.
- Potenziale per trasformare il progetto in un prodotto interno riutilizzabile per altri team o per clienti.
