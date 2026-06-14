# News Topic Classifier using BERT

## 📌 Objective
Fine-tune a transformer model (BERT) to classify news headlines into topic categories.

## 🛠 Methodology / Approach
- Loaded the AG News dataset from Hugging Face
- Tokenized text data using BERT tokenizer (max length 128)
- Fine-tuned bert-base-uncased model for sequence classification on 4 news categories
- Trained for 2 epochs using Hugging Face Trainer API with GPU acceleration
- Evaluated using Accuracy and F1 Score
- Visualized results using a confusion matrix

## 🛠 Technologies Used
- Python
- Hugging Face Transformers
- PyTorch
- Datasets
- Scikit-learn
- Matplotlib
- Seaborn

## 📊 Dataset
AG News Dataset (Hugging Face)
- 4 categories: World, Sports, Business, Sci/Tech
- 4,000 training samples, 1,000 test samples used

## 📈 Key Results
- Accuracy: 90.4%
- F1 Score: 90.4%
- Strong performance across all 4 news categories shown in confusion matrix

## 🚀 How to Run
1. Clone the repository
2. Install requirements: pip install transformers torch datasets scikit-learn pandas matplotlib seaborn
3. Run on GPU runtime: bert_news_classifier.ipynb

## 👩‍💻 Author
Syeda Hijab Zahra
BS Software Engineering — UMT
AI/ML Engineering Intern — DevelopersHub Corporation
