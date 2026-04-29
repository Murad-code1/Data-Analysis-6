# 🛒 UK E-Commerce Data Analysis

## 📌 Project Overview
This project performs an end-to-end exploratory data analysis (EDA) on a UK-based online retail dataset to understand customer behavior, sales performance, and business trends.

The dataset contains **541,909 transactions across 8 features**, including product details, customer information, and geographic data.

The main objective is to identify:

- Customer purchasing behavior
- Revenue distribution across countries
- Product performance and best-sellers
- Seasonal sales trends
- Return patterns and operational inefficiencies

---

## 🧹 Data Cleaning
The following preprocessing steps were applied:

- Removed **135,080 rows with missing CustomerID (~25% of dataset)** for accurate customer-level analysis
- Identified cancelled transactions using InvoiceNo starting with `"C"` and separated them
- Removed negative `Quantity` values from the main dataset (handled as returns)
- Converted `InvoiceDate` to datetime format
- Verified dataset integrity after cleaning

---

## 📊 Exploratory Data Analysis
The analysis includes:

- Customer-level metrics (Total Revenue, Total Orders, Average Order Value)
- Country-level revenue and order distribution
- Monthly revenue trends and seasonality analysis
- Top 20 products by quantity sold
- Return rate analysis across countries
- Top 10 customers by revenue contribution
- Basket size (average number of unique products per order)

---

## 🌍 Country-Level Analysis
A detailed country-level analysis was performed to compare revenue contribution and order behavior.

### Key Findings

- The **United Kingdom dominates the dataset**, contributing approximately **80%+ of total revenue**
- Other countries contribute significantly smaller portions, indicating untapped growth potential
- Customer purchasing behavior varies across regions

This highlights a strong domestic market presence with opportunities for international expansion.

---

## 📈 Time-Series Analysis

- Monthly revenue trends reveal clear **seasonality patterns**
- Sales peak during **November and December**, driven by holiday demand
- Lower activity is observed during early months of the year

This indicates the importance of aligning business strategies with seasonal demand cycles.

---

## 📦 Product Analysis

- Identified top-selling products based on quantity sold
- High-volume items tend to be low-cost, frequently purchased goods
- Product demand distribution is highly skewed toward a small subset of items

---

## 🔁 Return Analysis

- Return rates were calculated by comparing cancelled vs total orders
- Certain countries exhibit **higher return rates**, indicating potential issues in:
  - Logistics
  - Product expectations
  - Customer satisfaction

Reducing return rates can significantly improve profitability.

---

## 👥 Customer Insights

- A small group of customers generates a large portion of total revenue (**Pareto Principle**)
- High-value customers show consistent purchasing behavior over time
- Average basket size provides insight into cross-selling opportunities

---

## 📊 Visualizations

The project includes:

- Line chart for monthly revenue trends
- Bar charts for top countries and return rates
- Horizontal bar chart for top products
- Multi-line charts for top customer spending behavior

---

## 🛠️ Technologies Used

- Python
- pandas
- matplotlib
- seaborn

---

## 🚀 Conclusion

This analysis provides actionable business insights into customer behavior, market concentration, and operational performance. 

Key opportunities include:

- Expanding beyond the UK market
- Improving customer data tracking
- Leveraging seasonal demand patterns
- Reducing return rates
- Focusing on high-value customers

---
