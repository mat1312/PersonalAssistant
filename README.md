# GeneralAssistantBot - Test

Questo progetto utilizza [n8n](https://n8n.io/) per creare un bot flessibile e personalizzabile, integrando varie API e strumenti di intelligenza artificiale. È progettato per rispondere a messaggi, generare contenuti e interagire con gli utenti su piattaforme come Telegram.

## Caratteristiche

- **Integrazione con OpenAI**: Supporto per modelli di linguaggio avanzati come GPT-4 per risposte intelligenti e contestualizzate.
- **Memoria contestuale**: Utilizzo di una finestra di memoria per mantenere la coerenza nelle conversazioni.
- **Generazione di immagini**: Creazione di immagini personalizzate su richiesta utilizzando strumenti AI.
- **Supporto multi-tool**: Calcolatrice, ricerca su Wikipedia, query via SerpAPI e altro.
- **Integrazione con Telegram**: Risposte automatiche, trascrizione di messaggi vocali e gestione degli eventi.

## Struttura del Progetto

- **Nodes principali**:
  - **Telegram Trigger**: Rileva messaggi e comandi su Telegram.
  - **OpenAI Chat Model**: Genera risposte basate su GPT.
  - **Window Buffer Memory**: Mantiene il contesto della conversazione.
  - **Vector Store Tool**: Gestisce il recupero di dati da archivi vettoriali.
  - **Pinecone Vector Store**: Integrazione con Pinecone per memorizzare e recuperare embedding.

- **Tool aggiuntivi**:
  - Calcolatrice per calcoli dinamici.
  - Wikipedia per informazioni rapide.
  - SerpAPI per ricerche web avanzate.
  - Generazione di immagini e trascrizioni audio.

## Requisiti

- [n8n](https://n8n.io/)
- API key per:
  - OpenAI
  - Telegram
  - Pinecone (opzionale)
  - SerpAPI (opzionale)

## Come Iniziare

1. Clona questa repository:
   ```bash
   git clone https://github.com/mat1312/GeneralAssistantBot-Test.git
   Installa n8n localmente o su un server.
2. Importa il file .json nel tuo workspace n8n.
3. Configura le credenziali richieste:
4. Configura le credenziali richieste:
OpenAI API key
Telegram API key
5.Avvia il workflow e testa il bot su Telegram.

## Personalizzazioni
Puoi adattare i nodi del workflow alle tue necessità.
Integra altri strumenti o modifica le risposte generate per soddisfare il tuo caso d'uso.
