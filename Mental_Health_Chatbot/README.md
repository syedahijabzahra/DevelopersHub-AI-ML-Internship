# 🧠 MindfulMate - Mental Health Support Chatbot

A compassionate AI chatbot fine-tuned on Facebook AI's EmpatheticDialogues dataset to provide supportive responses for stress, anxiety, and emotional wellness.

## 📋 Overview

This project fine-tunes DistilGPT2 using Hugging Face's Trainer API to create an empathetic conversational agent. The model is trained on real human dialogues to recognize emotional contexts and respond with gentle, supportive language.

## ✨ Features

- **Empathetic Responses**: Trained on Facebook AI's EmpatheticDialogues dataset
- **Mental Health Focus**: Specialized for stress, anxiety, loneliness, and emotional wellness
- **Safety First**: Built-in crisis response filters and resource referrals
- **Multiple Interfaces**: Command-line interface and Streamlit web app
- **GPU Optimized**: Fine-tunes efficiently on Google Colab T4 GPU

## 🚀 Quick Start

### Prerequisites

- Google Colab 
- Python 3.8+
- CUDA-capable GPU (optional but recommended)

### Installation

```bash
# Install dependencies
pip install transformers datasets accelerate torch pandas streamlit
