## Methodology

- Loaded the `ecommerce_data.csv` dataset using **pandas** (`541,909 rows × 8 columns`)
- Inspected dataset structure and identified missing values, including **135,080 missing CustomerID records (~25%)**
- Converted `InvoiceDate` to datetime format for accurate time-series analysis
- Identified cancelled transactions using InvoiceNo starting with `"C"` and separated them for return analysis
- Removed negative `Quantity` values from the main dataset to ensure only valid sales are analyzed
- Created a clean dataset for customer-level analysis by excluding missing `CustomerID` values
- Engineered a new feature: `Revenue = Quantity × UnitPrice`
- Performed aggregations using `groupby()` for customer, country, and product-level insights
- Built visualizations to analyze trends, patterns, and comparisons
- Calculated return rates by comparing cancelled vs total orders across countries

---

## Business Insights

**UK Market Dominance:**  
The United Kingdom generates approximately **80%+ of total revenue**, significantly outperforming all other countries.  
→ Heavy reliance on a single market introduces risk, but also highlights strong domestic performance. Expanding internationally can drive future growth.

---

**Customer Data Gap:**  
Around **135,080 transactions (~25% of total data)** are missing `CustomerID`, limiting customer-level analysis.  
→ Improving customer tracking systems can unlock better segmentation, personalization, and retention strategies.

---

**Seasonal Revenue Peaks:**  
Revenue shows strong spikes during **November and December**, indicating clear holiday-driven demand.  
→ Businesses should align inventory, marketing campaigns, and operations with Q4 seasonality to maximize performance.

---

**High Return Rates in Specific Countries:**  
Certain countries exhibit noticeably higher return rates compared to others.  
→ This may indicate logistics issues, product mismatches, or unmet customer expectations that require localized improvements.

---

**Revenue Concentration (Pareto Effect):**  
A small group of customers contributes a disproportionately large share of total revenue.  
→ Focusing on high-value customers through loyalty programs and personalized marketing can significantly boost long-term profitability.
