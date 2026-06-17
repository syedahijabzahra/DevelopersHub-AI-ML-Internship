# Context-Aware Chatbot Using RAG (Retrieval-Augmented Generation)

## 📌 Objective
Build a conversational chatbot that retrieves relevant information from a custom knowledge base and generates context-aware answers using Retrieval-Augmented Generation.

## 🛠 Methodology / Approach
- Created a custom knowledge base (company policy document)
- Split the document into overlapping text chunks using LangChain's text splitter
- Generated embeddings using Sentence Transformers (all-MiniLM-L6-v2)
- Built a FAISS vector store for fast similarity-based retrieval
- Retrieved top relevant chunks for each user query
- Used Google Flan-T5-Base to generate context-aware answers combining retrieved context and conversation history
- Maintained conversation memory across multiple turns

## 🛠 Technologies Used
- Python
- LangChain
- FAISS (vector similarity search)
- Sentence Transformers
- Hugging Face Transformers (Flan-T5)

## 📊 Dataset
Custom knowledge base document containing company subscription plans, refund policy, support information and data security details.

## 📈 Key Results
- Successfully retrieved relevant context chunks for 5 different user queries
- Generated accurate, context-grounded answers (e.g., correctly identified Pro plan price, refund policy and Enterprise support hours)
- Demonstrated working RAG pipeline combining retrieval and generation for conversational AI

## 🚀 How to Run
1. Clone the repository
2. Install requirements: pip install langchain langchain-community langchain-text-splitters langchain-huggingface sentence-transformers faiss-cpu transformers
3. Run: context_aware_chatbot_rag.ipynb

## 👩‍💻 Author
Syeda Hijab Zahra
BS Software Engineering — UMT
AI/ML Engineering Intern — DevelopersHub Corporation
