


# Telegram AI Personal Assistant

A project powered by **n8n**, leveraging artificial intelligence to create a versatile personal assistant integrated with Telegram and various advanced APIs.

## Features

- **Audio and Text Processing**: Uses OpenAI APIs to process and respond to both voice and text messages.
- **Internet Search**: Integrates Perplexity API for quick and accurate online searches.
- **Calendar Management**: Connects to Google Calendar for creating, editing, and deleting events effortlessly.
- **Image Generation**: Utilizes DALL-E to create custom images for visual projects.
- **Personal Data Access**: Integrates Pinecone as a vector database to manage contacts and personal information.

## Project Architecture

The workflow is built using **n8n**, an open-source platform for process automation. Each feature is implemented as an independent node:

1. **Telegram Trigger**: The bot is triggered by messages sent via Telegram.
2. **AI Processing**: OpenAI provides contextual responses for text and audio queries.
3. **Internet Search**: Perplexity API enables online information retrieval.
4. **Calendar Management**: Connects with Google Calendar for event management.
5. **Image Generation**: Generates images on demand via DALL-E.
6. **Vector Database**: Pinecone stores and retrieves contacts and personalized data.

## How It Works

1. The user sends a message (text or voice) to the bot on Telegram.
2. The message is processed by the workflow in n8n, which identifies the required action (e.g., search, calendar management, or image generation).
3. The bot interacts with APIs like OpenAI, Perplexity, Google Calendar, or Pinecone to deliver the requested output.
4. Responses are sent back to the user on Telegram.

## Workflow Visualization

The following image shows the entire workflow in **n8n**, combining all the functionalities:

![image](https://github.com/user-attachments/assets/e991270f-c7f8-45d2-a4fc-e4f306877af6)


_Note: Errors visible in the workflow diagram are due to combining multiple functionalities for demonstration purposes. Each node is tested and works perfectly in practice._

## Prerequisites

- [n8n](https://n8n.io) installed locally or on a server.
- A Telegram bot token from [BotFather](https://core.telegram.org/bots).
- API keys for:
  - [OpenAI](https://platform.openai.com)
  - [Perplexity](https://www.perplexity.ai)
  - [Google Calendar](https://console.cloud.google.com)
  - [Pinecone](https://www.pinecone.io)
- A configured Google Cloud project with Calendar API enabled.

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/PersonalAssistant.git
   ```
2. Import the `n8n` workflow file into your instance.
3. Configure environment variables or credentials in n8n for Telegram, OpenAI, Perplexity, Google Calendar, and Pinecone.
4. Start n8n and test the workflow.

## Usage

- Send a text or voice message to the bot on Telegram.
- Use natural language queries for actions like:
  - "Search the web for the latest news."
  - "Create a meeting for tomorrow at 10 AM."
  - "Generate an image of a futuristic city."
- The bot will process the request and respond in real-time.



