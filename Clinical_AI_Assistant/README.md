# 🩺 Clinical AI Assistant (RAG System)

### CMPE 256 – Data Science Hackathon | San José State University

The **Clinical AI Assistant** is a Retrieval-Augmented Generation (RAG) system built to answer clinical research questions using **medical PDFs and CSV datasets**.  
It extracts information from uploaded documents, embeds it using **Sentence Transformers**, and retrieves evidence-based answers grounded directly in the data.

---

## 🎯 Objective
To enable researchers and clinicians to query thousands of pages of clinical research data and receive concise, context-aware answers supported by citations.

---

## ⚙️ Technical Overview
- **Text Extraction:** Uses `pypdf` to recursively extract text from PDFs stored in Google Drive.  
- **Chunking & Embedding:** Splits text into ~1800-token chunks and embeds them using **MiniLM SentenceTransformer (GPU)**.  
- **Vector Storage:** Stores embeddings, metadata, and documents in a **ChromaDB** collection on Drive.  
- **Query Retrieval:** Encodes the user’s question and retrieves semantically similar chunks using cosine similarity.  
- **Interface:** Gradio web app that accepts natural language questions and displays results with **PDF file name + page citations**.

---

## 🧩 Folder Structure
```
Clinical_AI_Assistant/
│
├── CMPE256_Clinical_PDF_RAG_Colab_v4_0_T4_GPU.ipynb
├── clinical_pdfs/         # PDF folders (Covid, Diabetes, Heart Attack, Knee Injuries)
├── clinical_csvs/         # CSV datasets
├── clinical_store/        # Persistent ChromaDB vector database
└── README.md
```

---

## ⚙️ Setup Instructions
1. **Mount Google Drive** inside Colab.
2. Upload all PDFs and CSVs into their respective Drive folders.
3. Run all cells in order:
   - Install dependencies  
   - Mount Drive and define paths  
   - Extract text and build embeddings  
   - Launch Gradio UI  
4. Use the web app to ask questions like:  
   *“Which models were used for heart attack prediction and their accuracy?”*

---

## 🧠 Example Questions
- “What deep learning models were used for COVID-19 detection?”  
- “List studies related to diabetes management using AI.”  
- “What datasets are used for knee injury detection research?”

---

## 💻 Tech Stack
- Python  
- SentenceTransformers (MiniLM)  
- ChromaDB  
- PyPDF  
- Gradio  
- Google Colab (T4 GPU)

---

## 👩‍💻 Team
**Team Bro Code**  
- [Add your team members’ names here]

---

## 🏁 Key Outcome
The project successfully demonstrates a **scalable RAG pipeline** that can process thousands of PDF pages efficiently on Colab GPU and return **grounded, evidence-based responses** for healthcare research.
