# 🛒 Electronic Retailer Market Basket Recommender System

### CMPE 256 – Data Science Hackathon | San José State University

The **Market Basket Recommender System** uses **association rule mining** to recommend products that are frequently bought together.  
It simulates an online retail checkout process with dynamic, real-time product recommendations powered by **Apriori** and a **Gradio interface**.

---

## 🎯 Objective
To design and implement a recommender model that analyzes historical purchase data and dynamically suggests relevant items during online checkout.

---

## ⚙️ Technical Overview
- **Data Preprocessing:** Reads and cleans transaction data (Product Name, SKU, Transaction ID).  
- **Transformation:** Converts wide-format transaction data to tall-format using `pandas.melt()`.  
- **Encoding:** Builds a one-hot encoded basket for use with the **Apriori algorithm**.  
- **Rule Generation:** Generates strong association rules using **support, confidence, and lift metrics**.  
- **Fallback Recommendation:** Implements a co-occurrence-based fallback for cases with limited patterns.  
- **UI Integration:** Gradio-based front-end where users can add items to a cart and instantly receive recommendations.

---

## 🧩 Folder Structure
```
Market_Basket_Recommender/
│
├── CMPE256_Market_Basket_Colab.ipynb
├── dataset/
│   └── CMPE256_Hackathon_market_basket_analysis_Release.csv
└── README.md
```

---

## ⚙️ Setup Instructions
1. Open the Colab notebook: `CMPE256_Market_Basket_Colab.ipynb`
2. Upload the dataset (or let the notebook auto-generate a demo dataset)
3. Run all cells in sequence:
   - Install dependencies  
   - Upload and preprocess data  
   - Generate rules using Apriori  
   - Launch Gradio interface
4. Select items → Click **Get Recommendations** → View dynamic product suggestions.

---

## 💻 Tech Stack
- Python  
- Pandas  
- Mlxtend (Apriori, Association Rules)  
- Gradio  
- Google Colab

---

## 🧠 Example Use
If a customer adds a *“Bosch D7050 Detector”* to their cart,  
the system might recommend *“DSC PG9914 Motion Detector”* or *“Bosch B810 Wireless Receiver”* based on frequent item associations.

---

## 👩‍💻 Team
**Team Bro Code**  
- [Add your team members’ names here]

---

## 🏁 Key Outcome
This project demonstrates how **data mining and association rule learning** can enhance online retail platforms by improving cross-selling and customer experience through intelligent, real-time recommendations.
