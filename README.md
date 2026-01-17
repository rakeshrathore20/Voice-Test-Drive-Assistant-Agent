# Rakesh Motor — Voice Test Drive Assistant (n8n)

A simple **voice-based test drive booking system** built in **n8n**.

## What it does

A customer can call the dealership, speak naturally, and the system will:

* Listen to their request
* Understand what they want
* Share car details
* Book a test drive
* Speak back a confirmation

Example:
Customer says: *“I want a test drive for an SUV tomorrow at 11 AM.”*
The system replies in voice: *“Your test drive is scheduled for tomorrow at 11 AM.”*

## How it works (plain language)

* **Voice → Text** (Speech-to-Text)
* AI understands the request
* It checks available cars
* It books a calendar slot
* **Text → Voice reply** (Text-to-Speech)

## Tech Tools Used

* **n8n** – Workflow automation
* **Google Gemini** –

  * Speech-to-Text (STT)
  * Text-to-Speech (TTS)
  * Conversational AI
* **LangChain (inside n8n)** – AI agent and memory
* **In-memory Vector Store** – Knowledge base
* **Google Calendar API** – Test drive booking
* **Webhook + HTTP nodes** – Handling voice input

## Setup (quick)

1. Import the `.json` workflow into n8n
2. Add your:

   * Google Gemini credentials
   * Google Calendar credentials
3. Activate the workflow
4. Send a POST request with `audioUrl` to `/voice-call`

---

Want this in **ultra-minimal one-paragraph GitHub version**?
