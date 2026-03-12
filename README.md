## Multilingual Healthcare Voice Assistant

It is a **multilingual voice-based healthcare assistant** that allows users to ask medical questions using natural speech and receive accurate spoken responses powered by **AI, medical NLP, and Retrieval-Augmented Generation (RAG)**.

The system combines **speech recognition, medical entity understanding, vector search, and generative AI** to provide **reliable and low-latency healthcare information**.

This project demonstrates how modern AI systems can integrate **voice interfaces, domain-specific NLP models, and knowledge-grounded LLMs** for real-time medical assistance.

---

# 🚀 Key Features

🎤 **Voice-Based Interaction**
Users can ask healthcare questions using voice.

🌍 **Multilingual Support**
Supports multiple languages using **Sarvam AI speech and language models**.

🧠 **Medical NLP Processing**
Uses **PubMedBERT** to understand medical terms, symptoms, and disease queries.

🔎 **Retrieval-Augmented Generation (RAG)**
Uses **FAISS vector search** to retrieve relevant medical knowledge before generating responses.

⚡ **Low-Latency Voice Pipeline**
Buffers and streaming architecture ensure fast responses.

🔊 **Voice Responses**
AI-generated responses are converted back into speech using **Text-to-Speech (TTS)**.

---

# 🏗 System Architecture

```
User Voice
↓
Audio Buffer
↓
Sarvam Streaming ASR
↓
Text Buffer
↓
Medical NLP Processing (PubMedBERT)
↓
Embedding Generation
↓
FAISS Vector Retrieval (RAG)
↓
Sarvam LLM Response Generation
↓
Response Buffer
↓
Sarvam TTS
↓
Voice Output
```

---

# 🧠 Core Technologies

| Layer                | Technology             |
| -------------------- | ---------------------- |
| Programming Language | Python                 |
| Speech Recognition   | Sarvam ASR             |
| Medical NLP          | PubMedBERT             |
| Embeddings           | Sentence Transformers  |
| Vector Search        | FAISS                  |
| LLM Generation       | Sarvam AI              |
| Speech Output        | Sarvam TTS / Coqui TTS |
| Backend API          | FastAPI                |
| Streaming            | AsyncIO / WebSockets   |
| Deployment           | Docker                 |

---

# 🔎 Retrieval-Augmented Generation (RAG)

RAG improves answer reliability by retrieving trusted medical information before generating responses.

Workflow:

```
User Query
↓
Embedding Model
↓
FAISS Vector Search
↓
Relevant Medical Documents
↓
LLM Response Generation
```

Benefits:

• reduces hallucination
• ensures medically grounded answers
• improves response accuracy

---

# ⚡ Latency Optimization

To ensure real-time responses, the system includes:

• **Streaming speech recognition**
• **Audio and text buffering**
• **FAISS indexed vector retrieval**
• **optimized embedding models**

---

# 📂 Project Structure

```
medvoice-ai
│
├── api
│   ├── speech_service.py
│   ├── nlp_service.py
│   ├── embedding_service.py
│   ├── retrieval_service.py
│   ├── generation_service.py
│   └── tts_service.py
│
├── models
│   ├── pubmedbert
│   └── embedding_models
│
├── rag
│   ├── faiss_index.py
│   └── retriever.py
│
├── utils
│   ├── audio_buffer.py
│   └── streaming.py
│
├── main.py
├── requirements.txt
└── README.md
```

---

# 🔐 Safety & Responsible AI

Healthcare AI must avoid unsafe advice.

Safety mechanisms include:

• medical disclaimers
• emergency symptom detection
• retrieval from verified medical sources
• hallucination reduction using RAG

---

# ⭐ Acknowledgements

Technologies used in this project:

* PubMedBERT
* FAISS
* Sentence Transformers
* Sarvam AI
* FastAPI

---
