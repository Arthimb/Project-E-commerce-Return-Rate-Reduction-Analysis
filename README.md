E-commerce Return Rate Reduction Analysis
📌 Objective
The objective of this project is to analyze product return patterns in an e-commerce business to identify:

Key factors contributing to product returns.

Return rates by product category, geography, and marketing channel.

High-risk products using predictive modeling.

🛠️ Tools Used
Python: Data cleaning, analysis, and logistic regression modeling.

SQL: (Assumed for initial data extraction or querying if needed).

Power BI: Visualization dashboard for presenting return risk insights.

📊 Mini Guide
1. Data Cleaning and Preprocessing
Dataset: superstore_return.xlsx

Cleaned null values in critical columns (RETURN_STATUS, PRODUCT_ID, etc.).

Converted ORDER_DATE and SHIP_DATE to datetime.

One-hot encoded categorical variables: SHIP_MODE, SEGMENT, REGION, CATEGORY, and SUB_CATEGORY.

2. Return Rate Analysis
Analyzed return percentage across various product categories and suppliers.

Derived insights on how return rates vary regionally and by customer segments.

3. Predictive Modeling
Used logistic regression from scikit-learn to estimate return probabilities.

Trained the model with 80/20 train-test split.

Evaluated with Classification Report and ROC-AUC score.

4. High-Risk Product Identification
Predicted return probability for each product.

Flagged top 5% as high-risk (High_Risk_Flag).

Exported high-risk product details into high_risk_products.csv.

5. Power BI Dashboard
Created a dynamic dashboard with:

Return rate metrics by category, region, segment.

Drill-through filters for deeper insights.

Visualizations of high-risk products based on prediction model.

✅ Deliverables
return_prediction.py: Python codebase for prediction.

superstore_return.xlsx(high_risk_products.csv): List of products with high return risk.

arthi-dashboard4.pbix: Power BI dashboard with navigation and insights.
