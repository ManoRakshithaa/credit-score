# Credit Score Analysis: Aave V2 Wallets

************************************************************

## Cluster Distribution

The KMeans model grouped wallets into 4 distinct clusters:

| Cluster | Wallet Count |
|---------|--------------|
|   0     |     3223     |
|   1     |      175     |
|   2     |        2     |
|   3     |       97     |

---

## Score Assignment Logic

Credit scores were assigned to each cluster based on behavioral quality:

| Cluster | Assigned Score | Description                            |
|---------|----------------|----------------------------------------|
|   2     | 975            | Elite wallets with perfect behavior    |
|   1     | 800            | Responsible users, low liquidation     |
|   0     | 550            | Average users with mixed behaviors     |
|   3     | 250            | Risky users with liquidations/fraud    |

---

## Score Distribution Insights

- The majority of wallets fall in **Cluster 0**, scoring around 550 — likely casual or average users.
- Cluster 1 wallets (score: 800) represent **stable users**, with active borrowing and repayment patterns.
- Only **2 wallets** belong to Cluster 2, achieving a near-perfect behavior score of **975** — possibly institutional or highly reputable addresses.
- Cluster 3 includes wallets with **high risk or suspicious behavior**, receiving a low score of **250**.

---

## Observations

- Most users show balanced borrowing and repayment patterns.
- Liquidation events are a major signal for risk and are heavily penalized.
- Very few wallets exhibit extremely high performance, which helps in flagging top-tier wallets for benefits (e.g., higher loan limits or incentives).
- Score gaps between clusters are intentionally large to reflect behavioral difference clearly.

---

## Conclusion

This model offers a simple and basic yet interpretable way to assess DeFi wallet behavior.  
It helps distinguish safe borrowers from high-risk users using on-chain activity with potential real-world applications in:

- Decentralized credit risk evaluation
- Airdrop filtering
- Whitelisting for secure protocols

************************************************************
