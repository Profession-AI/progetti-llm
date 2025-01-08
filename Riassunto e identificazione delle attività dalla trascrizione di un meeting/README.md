# Riassunto e Identificazione delle Attività dalla Trascrizione di un Meeting

## Introduzione
La capacità di analizzare le trascrizioni dei meeting aziendali è fondamentale per organizzare il lavoro e identificare le azioni chiave. In questo progetto, lo studente implementerà un sistema basato su modelli di linguaggio di grandi dimensioni (LLM) come GPT o LLama per processare una trascrizione e generare un riassunto e un elenco strutturato delle attività.

## Obiettivo del Progetto
Realizzare uno script in Python che:
1. Analizzi una trascrizione di un meeting fornita (disponibile al link: [https://raw.githubusercontent.com/Profession-AI/progetti-llm/refs/heads/main/Riassunto%20e%20identificazione%20delle%20attivit%C3%A0%20dalla%20trascrizione%20di%20un%20meeting/meeting_transcription.txt](https://raw.githubusercontent.com/Profession-AI/progetti-llm/refs/heads/main/Riassunto%20e%20identificazione%20delle%20attivit%C3%A0%20dalla%20trascrizione%20di%20un%20meeting/meeting_transcription.txt)).
2. Generi un riassunto conciso dei punti principali discussi.
3. Identifichi e strutturi le attività assegnate a ciascun partecipante.

## Requisiti
- **Input:** Un file di testo contenente la trascrizione del meeting (es. `meeting_transcription.txt`).
- **Output:**
  - Un riassunto dei punti chiave del meeting.
  - Un elenco di attività assegnate, con indicazione della persona responsabile.
  
## Linee Guida Tecniche
1. **Scelta del Modello:**
   - Utilizzare un modello di linguaggio LLM come GPT o LLama. Si consiglia l'uso di API di OpenAI o un'implementazione open-source di LLaMA.

2. **Pipeline del Progetto:**
   - **Pre-processing:** Caricare il file di trascrizione.
   - **Riassunto:** Utilizzare il modello LLM per generare un riassunto dei contenuti principali.
   - **Estrazione delle Attività:** Analizzare il testo per identificare frasi che indicano compiti assegnati, azioni future o responsabilità.

3. **Struttura dell'Output:**
   - **Riassunto:**
     ```
     Riassunto del Meeting:
     - Punto 1...
     - Punto 2...
     ```
   - **Elenco delle Attività:**
     ```
     Attività Identificate:
     - Mario Rossi: Redigere un piano tecnico basato sui requisiti emersi.
     - Andrea Monti: Implementare un modulo per le notifiche e il server SMTP.
     ```

4. **Testing e Validazione:**
   - Verificare che il sistema sia in grado di identificare correttamente attività e responsabilità, con un livello di accuratezza accettabile.

## Consegna
- Uno script Python documentato.
- Il riassunto generato e l'elenco delle attività basati sul file di trascrizione fornito.
- Un breve report che descriva:
  - Il funzionamento dello script.
  - I risultati ottenuti.
  - Le eventuali limitazioni del sistema.


