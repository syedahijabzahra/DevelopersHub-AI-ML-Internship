# BERT News Classifier

A news topic classifier built using BERT (bert-base-uncased) fine-tuned on the AG News dataset to classify news articles into 4 categories: **World**, **Sports**, **Business**, and **Sci/Tech**.

---

## 📌 Objective
Fine-tune a transformer model (BERT) to classify news headlines into topic categories.

---

## Dataset
- **Name:** AG News
- **Source:** Hugging Face (`fancyzhx/ag_news`)
- **Classes:** World, Sports, Business, Sci/Tech
- **Training samples used:** 4,000
- **Test samples used:** 1,000

---

## Model
- **Base Model:** `bert-base-uncased`
- **Task:** Sequence Classification
- **Fine-tuned for:** 2 epochs
- **Framework:** HuggingFace Transformers + PyTorch

---

## 🛠 Technologies Used
- Python
- Hugging Face Transformers
- PyTorch
- Datasets
- Scikit-learn
- Matplotlib
- Seaborn

---

## Results
| Metric | Score |
|--------|-------|
| Accuracy | 91.30% |
| F1 Score | 91.31% |

Strong performance was observed across all 4 news categories, as shown in the confusion matrix.

---

## How to Run
1. Open the notebook in Google Colab
2. Set runtime to **GPU** (`Runtime` → `Change runtime type` → `GPU`)
3. Run all cells (`Runtime` → `Run all`)

---

## Requirements
- transformers
- torch
- datasets
- scikit-learn
- pandas
- matplotlib
- seaborn

---

## 👩‍💻 Author
Syeda Hijab Zahra
BS Software Engineering — UMT
AI/ML Engineering Intern — DevelopersHub Corporation
