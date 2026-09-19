## Project Overview
This project presents an interactive retail sales analysis developed in Microsoft Excel. It analyzes sales performance from 2022 to 2025 across products, customer segments, sales channels, returns, promotions, and delivery methods.

The project contains two dashboards:
- Executive Dashboard, which provides a high-level view of overall sales, profitability, orders, returns, customer ratings, delivery performance, products, channels, and promotions.
- Year-over-Year Analysis Dashboard, which examines annual sales changes and investigates the factors associated with the decline in 2024 and the recovery in 2025.

The analysis was completed using Power Query, PivotTables, PivotCharts, the Excel Data Model, DAX measures, slicers, and a timeline.

## Project Objectives
- Evaluate overall sales and profitability.
- Monitor annual and monthly sales trends.
- Identify high-performing product categories and products.
- Analyze customer segments and sales channels.
- Measure return rates and examine return reasons.
- Evaluate delivery performance and customer ratings.
- Compare transactions with and without promotions.
- Build interactive Excel dashboards for business reporting.

## Dataset Description
The project uses a retail sales dataset containing approximately 18,000 transaction records from 2022 to 2025.

Major Data Areas:
- Transaction details: Transaction ID, Order ID, Order Date, Order Status
- Product details: Product Name, Product Category, Product Subcategory
- Customer details: Customer ID, Customer Segment, Age, Gender, Rating
- Sales details: Quantity, Sales Amount, Cost Amount, Profit, Discount Percentage
- Channel details: Sales Channel, Store, Country, Region
- Return details: Return Flag, Return Reason
- Promotion details: Promotion Code
- Delivery details: Shipping Method, Delivery Days

Dataset Source:
The dataset was obtained from Kaggle: https://www.kaggle.com/datasets/danielsowah123/retail-sales-dataset

## Tools & Techniques Used
- Microsoft Excel
- Power Query
- PivotTables
- PivotCharts
- Excel Data Model and Power Pivot
- DAX Measures
Used to calculate dynamic KPIs such as: Average Order Value and Return Rate Percentage
- Slicers
- Timeline
- Data Cleaning
- Data Analysis
- Dashboard Design

## Data Cleaning Process
The data was cleaned and transformed using Power Query before analysis.

### Cleaning Steps Performed
- Imported the source dataset into Power Query.
- Removed duplicate records.
- Removed completely blank rows.
- Checked and corrected column data types.
- Reviewed empty and null percentages using data-profiling tools.
- Applied Trim and Clean transformations to text columns.
- Standardized inconsistent text values, including payment methods and city names.
- Replaced missing `Return_Reason` values with `No Return` where appropriate.
- Replaced missing `Promotion_Code` values with `No Promotion`.
- Retained blank `Customer_Rating` values because they represent customers who did not submit ratings.
- Checked numeric columns for negative and invalid values.
- Retained realistic negative profit values because they represent genuine loss-making transactions.
- Verified that no invalid negative values were present in fields such as quantity, unit price, delivery days, and inventory level.
- Added analysis fields such as `Profit_Status` and `Promotion_Status`.
- Loaded the cleaned data into Excel and the Data Model.

### Data-Quality Decisions
- Missing ratings were not replaced with zero or an average because doing so would distort the actual rating analysis.
- Negative profit transactions were retained instead of being treated as errors.
- Business-related nulls were interpreted according to their meaning rather than deleting valid sales records.

## Key Performance Indicators (KPIs) Evaluated
The following KPIs were evaluated in the project:

### Primary KPIs
| Metric | Value |
|-------|-------|
| Total Sales | ₹82.34 Lakh |
| Total Profit | ₹16.45 Lakh |
| Profit Margin % | 20% |
| Total Orders | 14541 |
| Return Rate % | 13% |
| Average Customer Rating | 4.0 |
| Average Delivery Days | 2.3 |

### Secondary KPIs
| Metric | Value |
|-------|-------|
| Total Quantity Sold | 38277 |
| Total Customers | 4882 |
| Average Order Value | ₹566.27 |
| Number of Ratings | 14570 |
| Average Discount Percentage | 6.25% |
| Promotion Usage Rate | 40.7% |
| Number of Loss-Making Transactions | 231 |
| Loss-Making Transaction Rate | 1% |
| Order Completion Rate | 69.1% |
| Cost-to-Sales Ratio | 80.04% |

## Executive Dashboard
The Executive Dashboard provides a high-level view of retail performance and allows users to interact with the analysis using slicers and a date timeline.
### Dashboard Visuals
- Monthly Sales Trend
- Sales by Product Category
- Top 10 Products by Sales
- Sales by Sales Channel
- Return Rate by Customer Segment
- Profit Impact by Return Reason
- Average Delivery Days by Shipping Method
- Sales and Profit With vs Without Promotions
### Interactive Filters
- Product Category slicer
- Sales Channel slicer
- Customer Segment slicer
- Order Date timeline

## YOY Analysis Dashboard
The Year-over-Year Analysis Dashboard was created separately to explain annual sales changes in greater depth.
### Dashboard Purpose
The dashboard answers the following questions:
- How did annual sales change from 2022 to 2025?
- Which months contributed to yearly fluctuations?
- Which product categories supported or weakened annual sales?
- Did annual performance change because of order volume, Average Order Value, or both?
- Did revenue growth also result in profitable growth?
### Dashboard Visuals
- Annual Sales and YoY Growth
- Monthly Sales Trend by Year
- Product Category Performance by Year
- Order Volume and Average Order Value by Year
- Profitability Trend by Year
### YoY Results
- 2023: Sales increased by 0.63% compared with 2022.
- 2024: Sales decreased by 5.75% compared with 2023.
- 2025: Sales recovered strongly, increasing by 20.66% compared with 2024.

## Key Insights
- Total sales reached ₹82.34 Lakh, generating ₹16.45 Lakh in profit at an overall profit margin of approximately 20%.
- Sales remained stable in 2023 (+0.63%), declined in 2024 (-5.75%), and recovered strongly in 2025 (+20.66%).
- Electronics was the highest-performing product category, while Furniture ranked second in sales contribution.
- Online was the leading sales channel, contributing approximately 38% of total sales.
- The overall return rate was approximately 13%, with Small Business customers recording the highest return rate among customer segments.
- Average customer rating was 4.0/5, indicating generally positive customer satisfaction.
- Standard Shipping had the longest average delivery time, while Next Day delivery was the fastest shipping option after Pickup.
- Transactions without promotions generated higher sales and profit than transactions using promotions, suggesting the need to evaluate promotional effectiveness  more closely.

## Business Recommendations
### Prioritize high-performing product categories  
Maintain sufficient inventory and targeted marketing for Electronics, while investigating opportunities to improve Appliances and Office Supplies.
### Investigate the 2024 sales decline  
Review monthly trends, channels, product categories, order volume, and Average Order Value to identify the main factors associated with the 5.75% decline.
### Build on the 2025 recovery  
Identify the categories, channels, and customer segments that contributed most to the 20.66% growth and determine whether the improvement is sustainable.
### Reduce returns among high-return segments  
Examine products and return reasons associated with Small Business customers, who recorded the highest segment return rate.
### Improve standard-shipping performance  
Review carrier, region, and product-level delivery performance because Standard shipping recorded the longest average delivery time.
### Evaluate promotional effectiveness carefully  
Assess promotions using sales, profit margin, Average Order Value, and return rate instead of measuring success only through sales volume.
### Strengthen high-performing sales channels  
Continue investing in Online and Retail Store channels while investigating the low contribution from Phone Orders.

## Skills Demonstrated
- Data Preparation
- Data Cleaning
- Data Transformation
- Data Modeling
- Data Analysis
- Data Visualization
- Business Intelligence Reporting
- Excel Dashboard Development
- KPI Tracking
- Analytical Thinking
- Business Communication

## Project Files
- Retail_Sales_Analysis.xlsx
- README.md
- Executive_Dashboard.png
- YOY_Analysis_Dashboard.png
- Dashboard_Assets/Executive_Dashboard_Icon.webp
- Dashboard_Assets/YOY_Analysis_Dashboard_Icon.png
- Dataset/Sales_transactions_2022_2025.csv
