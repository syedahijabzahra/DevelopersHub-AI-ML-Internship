# 🧠 Mental Health Support Chatbot

An empathetic AI chatbot fine-tuned on mental health dialogues using **DistilGPT2**, trained to provide supportive, compassionate responses for anxiety, stress, loneliness, and sadness.

---

## 📌 Overview

This project fine-tunes a lightweight GPT-2 variant (`distilgpt2`) on a custom-built empathetic dialogue dataset to create a mental health support chatbot. The model is trained using HuggingFace's `Trainer` API with causal language modeling and includes a crisis safety filter for responsible deployment.

---

## ✨ Features

- 🤗 Fine-tuned `distilgpt2` using HuggingFace Transformers
- 📚 Custom empathetic dialogue dataset — 5,000 training + 500 validation examples
- 💬 5 emotional categories: Anxiety, Stress, Loneliness, Sadness, Positive
- 🚨 Crisis safety filter — detects self-harm keywords and returns crisis helpline info
- ⚙️ Configurable generation parameters (temperature, top-p, top-k)
- 💾 Model saved locally after fine-tuning for reuse

---

## 🛠️ Tech Stack

| Library | Purpose |
|---------|---------|
| `transformers` | DistilGPT2, Trainer, DataCollator |
| `datasets` | HuggingFace Dataset API |
| `torch` | PyTorch backend (GPU/CPU) |
| `pandas` | Data handling |
| `accelerate` | Efficient training support |

---

## 📂 Dataset

A **custom synthetic dataset** is generated within the notebook using curated empathetic response templates and context phrases across 5 categories:

| Category | Example User Input |
|----------|--------------------|
| Anxiety | "My anxiety has been keeping me up at night" |
| Stress | "I feel like I'm drowning in responsibilities" |
| Loneliness | "I feel so alone even when I'm around people" |
| Sadness | "Nothing seems to make me happy anymore" |
| Positive | "I finally finished a project I've been working on" |

No external dataset download is required — everything is generated in-notebook.

---

## 🚀 Getting Started

### 1. Install Dependencies

```bash
pip install transformers datasets accelerate torch pandas -q
```

### 2. Run the Notebook

Open `Mental_Health_Chatbot.ipynb` in Google Colab (GPU recommended) or Jupyter and run all cells.

The notebook will:
1. Generate the empathetic training dataset
2. Load and configure DistilGPT2
3. Tokenize and format conversations
4. Fine-tune for 3 epochs (~10–15 minutes on GPU)
5. Save the model to `./empathetic-chatbot-final`
6. Launch an interactive response demo

### 3. GPU Recommendation

Training on CPU is possible but slow. Enable a free GPU runtime in Google Colab:  
`Runtime → Change runtime type → T4 GPU`

---

## ⚙️ Training Configuration

| Parameter | Value |
|-----------|-------|
| Model | `distilgpt2` |
| Epochs | 3 |
| Batch size | 4 (effective: 16 with gradient accumulation) |
| Learning rate | 3e-5 |
| Max token length | 128 |
| Warmup steps | 100 |
| Mixed precision (fp16) | Auto (enabled on GPU) |

---

## 🔒 Safety & Ethics

- Detects crisis-related keywords (`suicide`, `kill myself`, `want to die`, etc.)
- Returns an emergency response with the **988 Suicide & Crisis Lifeline** number
- Does not provide therapy, diagnosis, or clinical advice
- Intended as a supplementary supportive tool only

---

## 💬 Example Output

```
User: I've been feeling really down lately
Assistant: I'm really sorry you're feeling this way. Sadness can be heavy to carry alone. I'm here with you.

User: I have so much to do and not enough time
Assistant: Stress can really take a toll on us. Taking small breaks throughout the day might help.
```

---

## 📁 Project Structure

```
Mental_Health_Chatbot/
│
├── Mental_Health_Chatbot.ipynb       # Main notebook
├── empathetic-chatbot/               # Checkpoints (auto-created during training)
├── empathetic-chatbot-final/         # Final saved model (auto-created)
└── README.md
```

---

## ⚠️ Disclaimer

This chatbot is **not a substitute for professional mental health care**. If you or someone you know is in crisis, please contact a licensed mental health professional or a crisis helpline immediately.

- 🇵🇰 **Pakistan:** Umang Helpline — 0317-4288665
- 🇺🇸 **USA:** 988 Suicide & Crisis Lifeline — call or text **988**

---

## 🙋 Author

Built as part of an AI/ML internship project at **CodeAlpha**.
