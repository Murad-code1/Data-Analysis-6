Methodology
Loaded the e-commerce dataset (541,909 rows × 8 columns) using pandas with encoding='ISO-8859-1'
Inspected dataset structure, data types, and identified missing values (notably 135,080 missing CustomerID records)
Converted InvoiceDate to datetime format for time-based analysis
Identified cancelled transactions using InvoiceNo starting with "C" and separated them
Removed negative Quantity values from the main dataset to exclude returns from sales analysis
Created a clean dataset for customer-level analysis by dropping missing CustomerID rows
Engineered a new feature: Revenue = Quantity × UnitPrice
Performed aggregations using groupby() for:
Customer-level metrics (revenue, orders, AOV)
Country-level performance
Product-level sales
Built visualizations using matplotlib and seaborn:
Monthly revenue trend
Top countries by revenue
Top products by quantity
Return rate by country
Conducted return rate analysis by comparing cancelled vs total orders
Performed additional analysis on top customers and basket size
Business Insights

UK Market Dominance:
The United Kingdom contributes the majority of total revenue, significantly outperforming all other countries combined (often ~80%+ of total sales).
→ The business is heavily dependent on a single market, creating both strength and risk. Expansion strategies should target high-potential international markets.

Customer Data Loss Impact:
Out of 541,909 records, 135,080 (~25%) transactions lack CustomerID, limiting customer-level analysis accuracy.
→ Improving customer tracking systems (login, CRM integration) can unlock better personalization and retention strategies.

Seasonal Revenue Peaks:
Monthly analysis shows strong spikes in revenue during November and December, indicating clear holiday season demand.
→ Businesses should align inventory, marketing campaigns, and staffing with Q4 demand surges to maximize revenue.

High Return Behavior in Certain Countries:
Return rate analysis reveals some countries have significantly higher cancellation ratios compared to others.
→ This may indicate logistics issues, product mismatches, or customer dissatisfaction. Localized improvements are required to reduce operational losses.

Top Customers Drive Disproportionate Revenue:
A small group of high-value customers contributes a large share of total revenue (Pareto principle effect).
→ Implement loyalty programs, targeted promotions, and personalized offers to retain and grow these high-value customers.
