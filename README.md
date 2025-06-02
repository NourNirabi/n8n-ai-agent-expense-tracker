# n8n AI Agent - Expense Tracker 💸

A smart automation using n8n and Groq LLM that logs expenses from Telegram messages (text or voice) into Google Sheets using AI Agent.

## ✨ Features
- Supports text and voice messages
- Transcribes voice with Whisper (HuggingFace)
- Uses Groq's LLaMA 3 to extract structured data
- Saves output to Google Sheets
- Fully automated and scalable

## 🧠 Tech Stack
- [n8n.io](https://n8n.io/)
- [Groq + LLaMA 3](https://groq.com/)
- [Hugging Face Whisper ASR](https://huggingface.co/openai/whisper-large-v3)
- [Telegram Bot API](https://core.telegram.org/bots/api)
- Google Sheets API

## ⚙️ Setup
1. Import `workflow.json` into n8n
2. Add Telegram Bot Token and Google Sheets credentials to `.env`
3. Deploy the workflow (can be self-hosted or on n8n cloud)

## 📂 Files
- `workflow.json`: main automation logic
- `scripts/extractDate.js`: JavaScript for parsing human dates
- `.env.example`: environment variables you need

## 📸 Demo Screenshot
![screenshot](./screenshot.png)

## 📜 License
MIT
