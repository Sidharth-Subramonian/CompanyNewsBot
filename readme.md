# 🧠 Company News Chatbot

A smart, AI-powered chatbot that finds and summarizes the latest news about any company in real-time—using only free and open-source tools. No paid APIs. No ChatGPT. Just reliable and fresh news delivered in your chosen style via an interactive web interface.

---

## 🚀 Problem Statement

Build a smart chatbot that can:

✅ Take one or more company names from user input  
✅ Search the internet in real-time for the latest news about those companies  
✅ Scrape news article content and summarize it using open-source AI  
✅ Return summaries with source links in your chosen style  
✅ Handle typos, greetings, off-topic questions like a conversational agent  
✅ Use no paid APIs (like NewsAPI or Google News API)  
✅ Run with an easy-to-use web UI (Gradio, Streamlit, Chainlit or Reflex)

---

## 🎯 Features

- 🔍 Real-time company news via Google search
- 🕸️ Article content scraped with BeautifulSoup
- 🤖 Summarization using Hugging Face Transformers (distilbart-cnn-12-6)
- ✍️ Choose your style: Formal, Casual, or Bullet Points
- 🧠 Fuzzy matching to handle typos and incorrect company names
- 💬 Chatbot mode handles general questions and greetings
- ✅ Fully free: no API keys, no paywalls, no dependencies on commercial LLMs
- 🖥️ Built using Gradio (can be extended to Streamlit or Chainlit)

---

## 🔧 Tech Stack

| Component       | Tool / Library                      |
|----------------|--------------------------------------|
| Web Interface   | Gradio                              |
| Web Search      | googlesearch-python                 |
| Scraping        | requests, BeautifulSoup4            |
| Summarization   | distilbart-cnn-12-6 from 🤗 Transformers |
| Typo Handling   | RapidFuzz                           |
| Chat Logic      | Rule-based with basic NLP           |
| Language        | Python 3.x                          |

---

## 📦 Installation

Clone this repo and install dependencies:

```bash
git clone https://github.com/yourusername/company-news-chatbot.git
cd company-news-chatbot
pip install -r requirements.txt
