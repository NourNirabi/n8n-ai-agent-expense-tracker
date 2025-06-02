# 💸 Telegram Finance Tracker Bot

This n8n workflow acts as a smart financial assistant, allowing users to send their expense details via **Telegram text or voice**, which are then parsed using an AI model and logged automatically into a **Google Sheets** file.

---

## 🧠 Features

- Telegram Bot integration (text and voice)
- Voice-to-text conversion using Whisper API from Hugging Face
- NLP processing with LangChain or Groq
- Smart parsing and extraction of:
  - Date
  - Item
  - Amount
  - Location
- Auto logging into Google Sheets

---

## ⚙️ Setup

1. Clone this repo and import the `workflow.json` into your [n8n](https://n8n.io/) instance.

2. Create `.env` file based on `.env.example`:

```bash
cp .env.example .env
```

3. Add your credentials inside `.env`:
- Telegram bot token
- HuggingFace token
- Google Sheets ID and Sheet Name
- Groq API token

---

## 🔐 Security Notice

Do **not** commit `.env` or sensitive credentials to your repo. Ensure your workflow never exposes tokens in hardcoded URLs.

---

## 🛠 Tech Stack

- n8n
- Telegram Bot API
- Hugging Face Whisper API
- LangChain / Groq
- Google Sheets API

---

## 📄 License

MIT