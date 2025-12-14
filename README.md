# Healthcare Hospital Information Chatbot (RAG)

A domain-specific healthcare chatbot built using a Retrieval-Augmented Generation (RAG) approach.  
The chatbot provides hospital-related information such as OPD timings, emergency services, and admission requirements while enforcing strict privacy and compliance rules.

---

## 🔍 Project Overview

This project demonstrates how to build a **compliant, domain-specific chatbot** for the healthcare domain.  
Instead of giving medical advice or revealing personal data, the chatbot is limited to **safe hospital information** and includes guardrails to prevent privacy violations.

The project was developed and tested using **Google Colab** and is suitable as a beginner-to-intermediate **AI / GenAI portfolio project**.

---

## ✨ Key Features

- Healthcare domain–specific chatbot
- Retrieval-Augmented Generation (RAG) style architecture
- Semantic search using **ChromaDB**
- Sentence-Transformer embeddings
- Privacy & compliance guardrails
  - Blocks personal names
  - Redacts PII (phone numbers, IDs, emails)
- Safe refusal for non-compliant queries

---

## 🧠 Technologies Used

- Python
- Sentence-Transformers
- ChromaDB (Vector Database)
- spaCy (NER for compliance)
- Pandas
- Google Colab

---

## 📂 Project Files

- `Healthcare_—_Hospital_Information_Chatbot_(RAG)_Project.ipynb`  
  → Complete notebook with implementation and outputs

- `healthcare_—_hospital_information_chatbot_(rag)_project.py`  
  → Python script version of the chatbot logic

---

## ▶️ How It Works

1. Hospital FAQs are stored as a small knowledge base
2. Text data is converted into embeddings using Sentence-Transformers
3. Embeddings are stored in ChromaDB
4. User queries are embedded and matched using vector similarity
5. A compliance layer checks for:
   - Personal names
   - PII patterns
6. Safe answers are returned, unsafe queries are refused

---

## 🔐 Compliance Rules

The chatbot **will NOT**:
- Share any patient-specific or personal information
- Provide medical diagnosis or treatment advice
- Answer queries about specific individuals

For such queries, the bot returns a safe refusal message.

---

## 🧪 Example Queries

**Allowed**
- What are Cardiology OPD timings?
- Is emergency service available 24/7?
- What documents are needed for admission?

**Blocked**
- Tell me Rahul Rawat’s ward number
- Share patient phone number
- Suggest medicine for fever

---

## 🚀 Future Improvements

- Integration with an LLM (OpenAI / Gemini)
- Web-based chat UI
- Larger hospital knowledge base
- Authentication-based access control

---

## 👤 Author

Built as part of a learning project for AI / GenAI and portfolio development.

---

## 📌 Note

This project is for **educational purposes only** and does not provide medical advice.
