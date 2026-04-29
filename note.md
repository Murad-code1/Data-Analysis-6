Methodology
Imported the UK-based e-commerce dataset containing 541,909 transactions and 8 features using pandas with appropriate encoding.
Conducted an initial data audit to examine structure, data types, and missing values, identifying 135,080 missing CustomerID entries (~25% of total data).
Converted the InvoiceDate column into datetime format to enable accurate time-series analysis.
Identified cancelled transactions using Invoice numbers starting with "C" and separated them for return analysis.
Removed records with negative Quantity values from the main dataset to ensure sales metrics reflect actual purchases.
Created a clean subset for customer-level analysis by excluding rows with missing CustomerID.
Engineered a key business metric:
Revenue = Quantity × UnitPrice
Performed aggregation using groupby() to derive insights across multiple dimensions:
Customer-level (Total Revenue, Order Count, Average Order Value)
Country-level (Revenue contribution, order distribution)
Product-level (Top-selling items by volume)
Built clear and interpretable visualizations using matplotlib and seaborn, including:
Monthly revenue trends
Top-performing countries
Best-selling products
Return rate by country
Calculated return rates by comparing cancelled transactions against total orders per country.
Extended the analysis with advanced metrics such as top customer behavior and average basket size.
Business Insights

1. Strong Dependence on the UK Market
The United Kingdom overwhelmingly dominates sales, contributing approximately 80% or more of total revenue.
→ While this highlights a strong domestic market presence, it also exposes the business to geographic concentration risk. Expanding into underperforming international markets presents a clear growth opportunity.

2. Significant Loss of Customer-Level Visibility
Approximately 135,080 transactions (~25% of the dataset) lack CustomerID information, restricting the ability to perform accurate customer segmentation and lifetime value analysis.
→ Strengthening data collection mechanisms (e.g., mandatory accounts, improved CRM systems) would significantly enhance data-driven decision-making.

3. Clear Seasonal Sales Pattern (Q4 Surge)
Revenue trends reveal pronounced peaks during November and December, aligning with holiday shopping behavior.
→ Strategic planning around Q4—such as inventory scaling, targeted marketing campaigns, and logistics optimization—can substantially boost annual performance.

4. Elevated Return Rates in Specific Regions
Return analysis indicates that certain countries experience disproportionately high cancellation rates compared to others.
→ This suggests potential issues in logistics, product-market fit, or customer expectations. Addressing these gaps can reduce revenue leakage and improve customer satisfaction.

5. Revenue Concentration Among Top Customers
A relatively small segment of customers contributes a disproportionately large share of total revenue, reflecting a classic Pareto (80/20) distribution.
→ Retention strategies such as loyalty programs, personalized offers, and VIP engagement should be prioritized to maximize long-term profitability.
