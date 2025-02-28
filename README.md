# Sales Analysis and Forecasting

## Project Overview
This project analyzes and forecasts sales data using SQL, Python (Prophet Model), and Tableau. The aim is to uncover insights about customer behavior, product demand, and sales trends, and to make predictions for future sales.

## Objectives
- Extract and transform data using SQL.
- Analyze purchasing behavior, product performance, and sales trends.
- Forecast future sales using time-series analysis with Prophet.

## Data
The dataset includes:
- **Transaction Details**: Invoice ID, Branch, City, Customer_type, Gender, Product_line, Date, and Time.
- **Financials**: Unit_price, Quantity, Tax, Total, Cost of Goods Sold (cogs), gross_margin_percentage, gross_income.
- **Customer Feedback**: Payment method and Rating.

## Key Analyses
1. **Customer Purchasing Behavior**: Comparison by Customer_type and Gender.
2. **Product Demand**: Average quantity sold per Product_line.
3. **Sales Trends**: Monthly and quarterly patterns.
4. **Revenue by Location**: Analysis by Branch and City.
5. **Payment Preferences**: Breakdown by payment method.
6. **Customer Satisfaction**: Ratings per Product_line.

## Tools Used
- **SQL**: Data extraction, transformation, and cleaning.
- **Tableau**: Visualizing sales trends and customer behavior.
- **Python (Prophet)**: Forecasting future sales trends.


## Results
1. **Seasonal Sales Trends**: Peaks in January, lows in February.
2. **High-Demand Products**: Food and Beverages generate the most revenue.
3. **Customer Demographics**: Female Members contribute most to sales.
4. **Payment Preferences**: Cash is most popular.
5. **Customer Satisfaction**: Highest ratings for Fashion Accessories, lowest for Health and Beauty.

## Data Extraction  
**Question**:
1.	Extract all information on the table
Insight: To retrieve all information on the table 
2.	Calculate the average purchase amount, total sales, and number of purchases for each combination of Customer_type (Member vs. Normal) and Gender.
Insight: Understanding differences in purchasing behavior between customer types and genders will guide us to know the targeted marketing or customer loyalty initiatives.
3.	Calculate the average quantity sold per transaction for each Product_line. Identify high-demand products by setting a threshold on this average quantity.
Insight: Knowing which products have higher demand can guide stocking and inventory management.
Ans: With threshold of 5, quantity demand for all product line does not have much difference.  Fashion accessories has the lowest demand of 5.0659 while Electronic accessories has highest demand of 5.756
4.	Extract Branch and Rating distribution 
Insight: Rating distribution by branch enable us to know the most rated branch. 
5.	Identify Product_line with the highest unit price
Insights: Understanding unit price distribution to get product with highest unit price
Ans: Fashion Accessories has highest unit price 

## Data Transformation
**Question**
1.	Convert the Date and Time columns into a standard timestamp format for consistency and ease of use in analysis.
Insight: Standardizing date and time formats allows for efficient time-based analysis and trend reporting. 
Outcome: New column was created for the date normal transformation 
## Data cleaning and preprocessing
**Question**
1.	Identify any rows with missing values, particularly in critical columns like Quantity, Unit_price, or Total, and replace missing values with an appropriate default (like average or median) if necessary.
Insight: Ensuring that essential columns have no missing values is crucial for accurate sales analysis and reporting.
Ans: No missing values in the crucial column for analysis
2.	Identify and exclude transactions where the Rating column has extreme outliers (e.g., ratings below 2 or above 9.5)
Insight: To ensure data quality for customer satisfaction analysis.
Ans: 71 rows of outliers were removed to ensure data integrity

## Dashboard Interpretation
This dashboard provides a complete picture of sales performance across different dimensions. 
1.	Sales Trends: The Bar chart highlights seasonal sales trends, providing an overview of high and low-demand periods.
2.	Product Performance: Product lines with high revenue stand out, guiding the company to focus on the most profitable products.
3.	Customer Insights: Customer type and gender analyses reveal purchase behaviors, suggesting areas to adjust marketing focus.
4.	Payment Preferences: The payment method chart informs the most popular payment types which is cash helping improve transaction convenience for customers.
5.	Customer Satisfaction: Product lines with lower customer ratings are highlighted, pinpointing areas for quality improvements.



## Conclusion and Recommendations
The analysis reveals key patterns and insights:
1.	Specific months show peak sales, highlighting potential seasonal influences.
2.	Certain product lines drive profitability, suggesting a strong alignment with customer demand.
3.	There is a diverse range of payment preferences
4.	Customer satisfaction varies across product lines, with potential areas for improvement.

## Forecasting with Prophet
Using Prophet, we forecasted sales for 60 days. The model reveals a stable initial period, followed by a peak and drop, potentially due to seasonal demand or events.

## Recommendations
1. Increase marketing efforts during peak sales months.
2. Focus on high-revenue product lines.
3. Enhance loyalty programs for Normal customers.
4. Expand in high-revenue locations.
5. Improve customer satisfaction in low-rated product lines.

## Clone the GitHub Repository
https://github.com/Irfankhan1q/sales-data.git

## Run the code in Sales Dashboard.ipynb and Sales Forecast.ipynb to get the result

If you find any issue while installing this, you can contact me at [irfankhanmd117@gmail.com](mailto:irfankhanmd117@gmail.com).



