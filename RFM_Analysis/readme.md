# 🧠 RFM Customer Segmentation Analysis

This project performs **RFM (Recency, Frequency, Monetary)** analysis to segment customers based on their purchasing behavior. It's a commonly used technique in marketing analytics to identify valuable customers and personalize engagement strategies.

---

## 📊 Project Objectives

- Understand customer purchase behavior using Recency, Frequency, and Monetary metrics.
- Segment customers into distinct groups using RFM scores.
- Visualize segment-level differences with grouped bar charts.
- Enable data-driven marketing decisions (e.g., loyalty campaigns, reactivation, etc.).

---

## 📂 Dataset

- **File:** `rfm_data.csv`
- **Fields Used:**
  - `CustomerID`: Unique ID of each customer.
  - `OrderID`: Order identifier (used to compute frequency).
  - `PurchaseDate`: Date of transaction.
  - `TransactionAmount`: Monetary value of the transaction.
  - `purchasedate`: date of purchase.
  - `location`: Order Address

---

## 🔍 Methodology

1. **Data Preprocessing**
   - Converted `PurchaseDate` to datetime format.
   - Removed missing or inconsistent records.

2. **RFM Metrics Calculation**
   - **Recency:** Days since last purchase.
   - **Frequency:** Total number of transactions.
   - **Monetary Value:** Total transaction value.

3. **Scoring**
   - Applied quantile-based scoring (1–5) for each RFM metric.

4. **Customer Segmentation**
   - Combined RFM scores to label customer segments (e.g., Loyal, At Risk, New).

5. **Visualization**
   - Grouped bar chart comparing average R, F, and M scores across segments using Plotly.

---

## 🛠 Tools & Technologies Used
- Python
- Pandas
- Plotly
- Jupyter Notebook

---
## 📌 Use Cases
- Personalized marketing campaigns
- Customer lifecycle management
- Churn prediction
- Loyalty program targeting
