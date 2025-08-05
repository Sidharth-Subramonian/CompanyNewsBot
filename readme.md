# 📰 Smart Company News Chatbot

An AI-powered chatbot that gives you real-time summaries of the **latest news about any company**. Just type a question like "What's new with Apple and Google?" and get clean, concise updates.

> ✅ Built using only **free, open-source tools**.  
> ✅ No paid APIs.  
> ✅ Web UI powered by **Gradio**.

---

## 🚀 Features

- 🔎 **Real-time news search** using web scraping and Google Search
- 🧠 **Summarized articles** using HuggingFace `distilbart-cnn-12-6`
- 🤖 Handles **greetings**, **casual language**, and **typos**
- ✨ Choose output style: Formal, Casual, or Bullet Points
- 🧩 Modular architecture with multiple AI agents:
  - SearchAgent
  - ScrapeAgent
  - SummarizerAgent
  - ChatAgent (for parsing, NER, fuzzy matching)

---

## 🔧 Tools & Libraries Used

| Component        | Tool/Model                              |
|------------------|------------------------------------------|
| UI               | Gradio                                   |
| Search           | `googlesearch-python`                    |
| Scraping         | `requests`, `beautifulsoup4`             |
| Summarization    | `sshleifer/distilbart-cnn-12-6` (Hugging Face Transformers) |
| NLP / NER        | `spaCy` with `en_core_web_trf`           |
| Fuzzy Matching   | `rapidfuzz`                              |
| Spell Handling   | Built-in fuzzy logic + optional `textblob`|

---

## 🛠️ Installation & Setup

You can run it on **Google Colab** or locally.

### 🔗 Run in Colab

> [Open in Colab](https://colab.research.google.com/)

### 📦 Local Installation

```bash
git clone https://github.com/Sidharth-Subramonian/CompanyNewsBot.git
cd CompanyNewsBot

pip install -r requirements.txt
python app.py
