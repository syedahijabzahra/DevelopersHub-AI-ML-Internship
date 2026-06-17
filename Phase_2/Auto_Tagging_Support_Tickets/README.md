# Auto Tagging Support Tickets Using LLM

## 📌 Objective
Automatically tag free-text customer support tickets into relevant categories using a large language model through zero-shot classification.

## 🛠 Methodology / Approach
- Created a sample dataset of free-text support tickets covering various issue types
- Defined candidate tag categories (Billing, Technical, Account Access, Delivery, etc.)
- Used Facebook's BART-Large-MNLI model for zero-shot multi-label classification
- Applied prompt-based classification without any fine-tuning required
- Ranked and extracted the top 3 most probable tags per ticket with confidence scores
- Visualized tag distribution and confidence scores across all tickets

## 🛠 Technologies Used
- Python
- Hugging Face Transformers (zero-shot-classification pipeline)
- BART-Large-MNLI model
- Pandas
- Matplotlib
- Seaborn

## 📊 Dataset
Custom free-text support ticket dataset covering common categories:
- Billing Issues, Technical Issues, Account Access, Product Quality, Subscription Management, Performance Issues, Delivery Issues, General Inquiry

## 📈 Key Results
- Successfully classified all support tickets into top 3 relevant tags using zero-shot learning
- No training/fine-tuning required — leveraged pre-trained LLM's natural language understanding
- Generated confidence scores for each predicted tag to support multi-class ranking
- Average confidence score demonstrates strong zero-shot performance on ticket categorization

## 🚀 How to Run
1. Clone the repository
2. Install requirements: pip install transformers pandas matplotlib seaborn torch
3. Run: auto_tagging_support_tickets.ipynb

## 👩‍💻 Author
Syeda Hijab Zahra
BS Software Engineering — UMT
AI/ML Engineering Intern — DevelopersHub Corporation
