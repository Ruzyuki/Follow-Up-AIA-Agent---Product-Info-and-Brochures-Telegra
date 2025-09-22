# 🤖 AI-Powered Telegram Assistants (n8n + Google Gemini + Google Sheets)

This repository contains  **AI-powered Telegram assistant** built using [n8n](https://n8n.io/).
They integrate **Google Gemini** for AI-driven natural language understanding, **Google Sheets** for structured data storage, and **Telegram** as the user interface.

**📄 Product Brochure Assistant**

An intelligent assistant that retrieves **product details and brochures** for customers/prospects.

* Takes product requests via Telegram (e.g., `"Send brochure for Mocean 4000"`).
* Looks up product & principal data from **Google Sheets**.
* Returns **product details and brochure link** instantly.
* Helps sales teams share updated brochures on the go.

**Example:**

```
User: Send me details of Mocean 4000  
Bot: 📄 Mocean 4000 is a product from Moptim (Retinal Imaging).  
     🔗 Download Brochure: [PDF Link]
```

---

## 🛠️ Workflow Overview

Both assistants are built with **n8n**:

1. **Telegram Trigger** – Captures user input.
2. **AI Agent (Google Gemini)** – Interprets message intent.
3. **Google Sheets** – Used as a lightweight database for expenses & product data.
4. **Telegram Send Message** – Returns confirmations, totals, or brochure links.

---

## 📦 Setup Instructions

1. Clone this repository:

   ```bash
   git clone https://github.com/yourusername/telegram-ai-assistants.git
   cd telegram-ai-assistants
   ```

2. Create a **Telegram Bot** using [@BotFather](https://t.me/BotFather) and get the API token.

3. Enable the **Google Sheets API** and download credentials.

4. Deploy **n8n** (Docker, local, or cloud).

5. Import the workflow JSON files (provided in `workflows/`).

6. Set environment variables:

   ```env
   TELEGRAM_TOKEN=your_telegram_token
   GOOGLE_API_KEY=your_google_key
   GEMINI_API_KEY=your_gemini_key
   SHEET_ID=your_google_sheet_id
   ```

7. Activate workflows → start logging expenses & sending brochures instantly 🚀

---

## 📊 Use Cases

* **Sales Teams** – Track expenses & share product details while on the move.
* **Managers** – Real-time insights into spending and product demand.
* **Organizations** – Lightweight AI-powered assistants without heavy ERP/CRM.

---

## ⚡ Tech Stack

* [n8n](https://n8n.io/) – Workflow automation
* [Telegram Bot API](https://core.telegram.org/bots/api) – Chat interface
* [Google Sheets API](https://developers.google.com/sheets/api) – Data storage & retrieval
* [Google Gemini](https://ai.google/) – Natural language understanding

---

## 📜 License

MIT License – Free for personal and commercial use.

---
