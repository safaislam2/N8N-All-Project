**# RxVision AI - Smart Telegram Prescription Analyzer 🩺🤖

**RxVision AI** is an intelligent, automation-driven Telegram Assistant designed to read, analyze, and translate handwritten or printed doctor prescriptions into clean, plain Bengali text. Built using n8n workflows and Vision AI models, it ensures high medical safety standards while delivering interactive and accessible health insights.

---

## 🌟 Key Features

* **Instant Vision Scanning:** Scans uploaded prescription photos via Telegram and extracts patient details, diagnosis, and medicine schedules.
* **80% Safety Confidence Guardrail:** Automatically evaluates image clarity and legibility. If confidence drops below 80%, the bot refrains from guessing and prompts the user to upload a clearer image.
* **Plain Bengali Output:** Converts complex medical terminology and illegible handwriting into clear, everyday Bengali language.
* **Text-to-Speech (TTS) Voice Summary:** Generates concise audio-ready text summaries designed for elderly or visually impaired users.
* **Interactive Follow-up Chat:** Allows users to ask continuous clarification questions about their parsed prescription directly within the Telegram thread.
* **Markdown-Free & Clean Data Pipeline:** Engineered to bypass Telegram API parsing errors by delivering pure, error-free raw text payloads.

---

## 🏗️ System Architecture & Workflow

1. **Telegram Trigger:** User submits a prescription photo or follow-up question.
2. **n8n Automation Engine:** Routes the incoming media payload and manages user session contexts.
3. **AI Core Engine (Vision & Text Models):** 
   - Evaluates legibility (80% confidence threshold test).
   - Extracts structured medicine metadata (Name, Purpose, Dosage, Timing, Duration).
   - Formats localized Bengali summaries and voice outputs.
4. **Telegram Response Node:** Delivers the formatted text and chat responses back to the user seamlessly.

---

## 🛠️ Tech Stack

* **Platform:** Telegram Bot API
* **Workflow Automation:** n8n (Node-based Integration Engine)
* **AI Core:** LLM Vision Models (OpenAI / Gemini Vision Core)
* **Output Format:** Plain Text / Structured Bengali Data Schema

---

## 🚀 Getting Started

1. **Clone & Import Workflow:** Import the provided n8n JSON workflow into your n8n instance.
2. **Configure Credentials:** Add your Telegram Bot Token and AI API Keys in n8n Credentials.
3. **Set Up System Prompt:** Copy the tuned Master System Prompt into the AI Agent node.
4. **Activate & Test:** Start the workflow and send a prescription photo to your Telegram Bot!

---

*Disclaimer: RxVision AI is an assistive tool designed to aid in understanding prescriptions. It does not replace professional medical advice.***
