# Aave V2 Wallet Credit Scoring [Project Overview]

************************************************************

## 📌 Project Overview

This project builds a machine learning model to assign **credit scores (0–1000)** to wallets interacting with the Aave V2 protocol.  
Higher scores indicate reliable and responsible users; lower scores reflect risky, bot-like, or exploitative behavior.

---

## 📁 Dataset Description

- 100,000 raw transaction-level records from the Aave V2 protocol  
- Actions include: `deposit`, `borrow`, `repay`, `redeemunderlying`, `liquidationcall`  
- Format: JSON

---

## 💾 Data Download

The main dataset (~87MB) is **not included** in this repository due to size limits.

You can download the dataset here:  
[Download Aave V2 transaction data (Google Drive)](https://drive.google.com/file/d/1ISFbAXxadMrt7Zl96rmzzZmEKZnyW7FS/view)

After downloading, place the file in the `data/` folder before running the notebook or scripts.

---

## 🧠 Methodology

1. **Feature Engineering**  
   - Aggregated per-wallet stats: total borrow, total deposit, repay ratio, liquidation count, active days, etc.

2. **Clustering**  
   - Used KMeans to group wallets by behavioral patterns.

3. **Scoring**  
   - Assigned credit scores to each cluster based on trustworthiness.

4. **Validation**  
   - Analyzed behaviors and score distributions across clusters for consistency.

---

## 📂 Repository Structure

credit-score/
├── data/ # Raw and sample datasets (https://drive.google.com/file/d/1ISFbAXxadMrt7Zl96rmzzZmEKZnyW7FS/view?usp=sharing)
├── notebooks/ # Jupyter notebooks with exploration and modeling code
├── outputs/ # Final scored wallet outputs (e.g., CSV files)
├── README.md # Project overview and methodology (this file)
├── ANALYSIS.md # Detailed analysis and score distribution


---

## 🚀 How to Run

1. Download the JSON dataset from Google Drive and place it inside the `data/` folder.  
2. Open and run the notebook(s) inside the `notebooks/` folder.  
3. Follow the steps to process data, engineer features, and run clustering.  
4. Credit scores for wallets will be generated and saved in `outputs/`.

---

## 🔭 Future Improvements

- Use advanced ML models for better scoring accuracy.  
- Analyze time-series patterns in transaction behavior.  
- Build a real-time scoring dashboard or API.

---

Do feel free to reach out for questions or feedback! Would love to hear from you! :)





