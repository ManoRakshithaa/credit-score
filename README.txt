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

## 🧠 Methodology

1. **Feature Engineering**  
   - Aggregated per-wallet stats: total borrow, total deposit, repay ratio, liquidation count, active days, etc.

2. **Clustering**  
   - Used KMeans to group wallets by behavioral patterns.

3. **Scoring**  
   - Assigned credit scores to each cluster based on trustworthiness.

4. **Validation**  
   - Analyzed behaviors and distributions across clusters for consistency.

---

## 📂 Repository Structure

credit-score/
--- data/  (Raw and sample datasets)
--- notebooks/  (Jupyter notebooks with exploration and modeling code)
--- outputs/ (Final scored wallet outputs)
--- README.txt (Project overview and methodology)
--- analysis.md  (Detailed analysis and score distribution)


---

## 🚀 How to Run

1. Load the provided JSON file into your notebook.
2. Execute the data processing and clustering steps.
3. Credit scores will be generated for each wallet.
4. Export the scores to CSV for downstream use.

---

## 🔭 Future Improvements

- Use advanced ML models for better scoring accuracy.
- Analyze time-series patterns in transactions.
- Build a real-time dashboard or scoring API.

---

Do feel free to reach out for questions or feedback! Would love to hear it!!!




