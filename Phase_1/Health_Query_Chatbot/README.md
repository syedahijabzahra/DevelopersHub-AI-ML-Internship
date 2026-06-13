# 🏥 Health Query Chatbot

A general-purpose health information chatbot powered by **Google's Flan-T5-Large** model, built with prompt engineering and a safety filter for responsible use.

---

## 📌 Overview

HealthBot is an AI-powered assistant that answers general health-related questions in simple, friendly language. It uses the `flan-t5-large` model from HuggingFace Transformers and is designed with safety-first principles — it never diagnoses, prescribes, or recommends dosages, and includes a crisis-response filter for sensitive queries.

---

## ✨ Features

- 💬 Conversational health Q&A using Flan-T5-Large
- 🛡️ Safety filter that blocks harmful/crisis-related queries and returns emergency contact information
- ⚠️ Automatic medical disclaimer appended to every response
- 🧠 Persona-based prompt engineering for consistent, warm responses
- 🔁 Interactive chat loop + demo mode with example queries

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| `transformers` | Load and run Flan-T5-Large |
| `torch` | PyTorch backend for inference |
| `sentencepiece` | Tokenizer support |
| Google Flan-T5-Large | Base language model |

---

## 🚀 Getting Started

### 1. Install Dependencies

```bash
pip install transformers torch sentencepiece -q
```

### 2. Run the Notebook

Open `Health_Query_Chatbot.ipynb` in Jupyter or Google Colab and run all cells.

The notebook will:
1. Load the Flan-T5-Large model (first run: ~1–2 minutes)
2. Run a **demo** with 6 sample queries
3. Launch an **interactive chat loop** — type your health question and press Enter

### 3. Exit the Chat

Type `quit`, `exit`, or `q` to end the session.

---

## 💡 Example Queries

```
🙋 You: What causes a sore throat?
🤖 Bot: A sore throat is usually caused by a viral infection...

🙋 You: How much water should I drink daily?
🤖 Bot: The general recommendation is about 8 glasses (2 litres) per day...
```

---

## 🔒 Safety & Ethics

- Blocked keywords related to self-harm or overdose trigger an **emergency response** with helpline numbers (Pakistan & USA)
- The bot never provides personalized medical advice, diagnoses, or prescriptions
- All responses include a disclaimer: *"This is general health information only, not medical advice."*

---

## ⚠️ Disclaimer

This chatbot provides **general health information only**. It is **not** a substitute for professional medical advice, diagnosis, or treatment. Always consult a qualified healthcare provider for personal medical concerns.

---

## 📁 Project Structure

```
Health_Query_Chatbot/
│
├── Health_Query_Chatbot.ipynb   # Main notebook
└── README.md
```

---

## 🙋 Author

Built as part of an AI/ML internship project at **DevelopersHub Coorporation**.
