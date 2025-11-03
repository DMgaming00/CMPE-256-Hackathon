# 🧠 CMPE 256 – Data Science Hackathon (Fall 2025)
### San José State University | Recommender Systems

This repository contains both projects completed by our team for the **CMPE 256 – Recommender Systems** Hackathon.  
Each part focuses on applying data science and machine learning concepts to build real-world, end-to-end systems.

---

## 📁 Repository Structure
```
CMPE256_Hackathon/
│
├── 📁 Market_Basket_Recommender/
│   ├── CMPE256_Market_Basket_Colab.ipynb
│   ├── dataset/CMPE256_Hackathon_market_basket_analysis_Release.csv
│   └── README.md
│
├── 📁 Clinical_AI_Assistant/
│   ├── CMPE256_Clinical_PDF_RAG_Colab_v4_0_T4_GPU.ipynb
│   ├── clinical_pdfs/ (PDF research files by domain)
│   ├── clinical_csvs/ (clinical trial CSV datasets)
│   └── README.md
│
└── README.md (this file)
```

---

## 🧩 Part 1: Market Basket Recommender
A **Market Basket Analysis** model built using the Apriori algorithm and association rule mining to simulate product recommendations during an online checkout process.  
It provides an interactive Gradio interface that dynamically suggests products commonly bought together.

➡️ [View README](Market_Basket_Recommender/README.md)

---

## 🧠 Part 2: Clinical AI Assistant
A **Retrieval-Augmented Generation (RAG)** system designed to answer clinical questions using grounded evidence from medical PDFs and CSV datasets.  
The model runs on Google Colab using a **T4 GPU**, extracts and embeds thousands of document chunks, and delivers evidence-backed answers with citations.

➡️ [View README](Clinical_AI_Assistant/README.md)

---

## 🧑‍💻 Team Members
- **Team Name:** Bro Code  
- **Members:** [Add your team members’ names here]  
- **Professor:** Dr. Chandrasekar Vuppalapati  
- **Course:** CMPE 256 – Recommender Systems (Fall 2025)

---

## 🚀 Tech Stack
- **Python**
- **Google Colab**
- **Pandas**, **mlxtend**, **Gradio**, **SentenceTransformers**, **ChromaDB**
- **T4 GPU** for fast vector embedding

---

## 🏁 How to Run
1. Open the desired `.ipynb` file in Google Colab.
2. Upload or link your dataset and supporting files.
3. Run all cells sequentially.
4. Use the Gradio interface to interact with each system.

---

## 🏅 Hackathon Outcome
Both systems demonstrate how **data-driven recommender systems and retrieval-based AI assistants** can enhance decision-making in real-world domains — retail and healthcare — using machine learning and information retrieval techniques.
