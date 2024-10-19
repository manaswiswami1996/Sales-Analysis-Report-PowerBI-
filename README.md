[logo] < https://github.com/manaswiswami1996/Sales-Analysis-Report-PowerBI-/blob/508a2a41dce0399eafb472118a3357e44323c897/Sales%20analysis%20image.jpeg > 
# Sales-Analysis-Report-PowerBI-
This Power BI Sales Analysis Report provides insights into sales performance, customer segmentation, and product profitability. The dashboard is designed to assist the client in identifying key growth opportunities and operational improvements by analyzing critical sales metrics.

# Data Model
## Schema
The data model is structured around several interconnected tables that form the backbone of this analysis. The following key tables are part of the data model:


<img width="956" alt="image" src="https://github.com/user-attachments/assets/e8e048d2-a6da-48be-a783-a52321c92496">



- Sales Table: Contains transactional data with fields like Sales ID, Date, Customer ID, Product ID, Sales Amount, and Quantity Sold.
- Customers Table: Includes customer demographic information such as Customer ID, Name, Location, Age, and Gender.
- Products Table: Stores product information such as Product ID, Category, Price, and Supplier details.
- Date Table: A comprehensive date table that helps in performing time-based analysis (e.g., Year, Month, Quarter).
- Geography Table: Geographic regions data to enable regional sales analysis.
  
## Relationships
- Sales to Customers: One-to-Many relationship based on Customer ID.
- Sales to Products: One-to-Many relationship based on Product ID.
- Sales to Date: Many-to-One relationship based on the Date field, which supports time series analysis.
- Sales to Geography: A relationship based on region codes or customer locations.
These relationships enable powerful filtering and cross-analysis across different dimensions, such as time, geography, and customer segments.

# Exploratory Data Analysis (EDA) Steps Using Power Query
## Data Cleaning: 

- Missing values in the Revenue, Profit, or Customer Age columns were handled using appropriate methods like filling or removing rows.
- Duplicate rows in the sales data were removed to ensure the accuracy of transactional records.

## Outlier Detection:

- Extreme values in revenue and profit were checked to identify potential errors in the data or significant anomalies, such as unusually high sales that require attention.

## Descriptive Statistics:

- Basic statistics were computed for numerical columns like revenue, order count, and customer age to understand data distribution using DAX.
- Categorical distributions were analyzed for gender, payment methods, and regions.

## Data Transformation:

- Date columns were transformed into useful time metrics such as Year, Quarter, and Month to enable time series analysis.
Customer ages were binned into groups (as seen in the age-based bar chart) for easier segmentation.


# Dashboard

#### Sales Performance Overview:


<img width="641" alt="image" src="https://github.com/user-attachments/assets/ec2dd28c-4982-4e48-bd82-7b761a05f063">

### Dashboard Insights
#### Key Metrics
- Order Count: **96K orders**.
- Total Revenue: **₹ 15.28M.**
- Total Profit: **₹ 12.22M**.
- Total Cost: **₹ 3.06M**.

## Summary 
- A main report carrying all main visuals with options to move between the years to understand a more crisp picture of the sales.
- A line chart shows the distribution of male and female customers over the years. The number of male customers appears slightly higher than female customers, but both trends follow a similar pattern..
- KPI cards displaying key metrics: Total Revenue, Order Count, Total Profit, and Total Cost.
- The tree map visual breaks down the order count for each year, highlighting peaks in order volume during certain years (such as 2020, 2017, and 2019).
- A bar chart displays the total revenue earned from different regions. The Northeast and West regions show the highest total revenue, indicating these as key areas for the business.
- The horizontal bar chart shows that customers aged between 30-50 years make the majority of orders. This age group is highly engaged in purchasing.
- The matrix shows the breakdown of payments by method (Card, Cash, Voucher) and status (Pending, Shipped, Returned). Voucher and Card payments dominate the transaction types.

## Key Insights
- The TotalRev by Region visual shows that the Northeast and West regions generate the highest revenue, with ₹4.7M and ₹4.3M respectively.
- Customers in the 40-year age group place the highest number of orders, followed by the 30-year and 50-year groups.
- Voucher and Card payments are the most popular payment methods, with over 32K and 31K orders respectively.
- The tree map reveals that 2020 had the highest order count, followed by 2019 and 2017

## Business Recommendations:
- Invest more in marketing efforts in these high-performing regions. Consider region-specific promotions, tailored products, and customer engagement strategies to further maximize sales in these areas.
- Personalized discounts, loyalty programs, or subscription services could help deepen customer loyalty and increase repeat purchases in the 30-40 years age segment.
- Create gender-specific marketing campaigns to re-engage customers and potentially increase customer retention. This could include targeted email campaigns, advertisements, or social media outreach based on product preferences by gender.
- Simplify and promote digital payment methods (Card, Voucher) even further by offering discounts for online transactions or faster checkout options.
-  Implement customer retention programs, such as loyalty rewards, referral bonuses, or personalized offers for returning customers. These strategies could help stabilize or even reverse the downward trend in recent orders.

 ## Next steps:
 - Implement predictive analytics based on the historical order data to forecast demand more accurately. This will help optimize inventory management, ensuring that products are available when needed without overstocking, thereby reducing cost
 - Identify high-margin products or product categories and focus on expanding the product lines or promoting them more aggressively.

# Conclusion
The Sales Analysis Report offers key insights for data-driven decisions. Focusing on high-revenue regions, targeting the 30-50 age group, and implementing gender-specific marketing can boost customer engagement. Enhancing digital payment adoption will streamline operations and improve customer experience. Capitalizing on the 2020 sales surge and expanding high-margin products can drive profitability. Improving order fulfillment and applying predictive analytics for inventory management will enhance efficiency and reduce costs, supporting sustained growth and long-term success.
