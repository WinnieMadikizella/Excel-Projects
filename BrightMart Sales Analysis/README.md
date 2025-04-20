# Sales Performance Analysis for BrightMart: A Data-Driven Journey

## 1. Introduction
Understanding sales performance, customer behavior, and product trends is crucial for growth and profitability in today’s competitive business environment. This analysis explores the sales data of BrightMart, a multinational retail company, from 2011 to 2016 through a structured data transformation, modeling, and visualization approach, key insights were derived to enhance sales performance and customer engagement.

## 2. Objectives
The primary objectives of this analysis were to:
1. Evaluate overall sales performance and profitability trends.
2. Understand customer demographics and purchasing behavior.
3. Identify top-performing products and categories.
4. Analyze sales distribution across different regions.
5. Uncover seasonal trends and revenue growth patterns.
6. Provide data-backed recommendations for business growth.

## 3. Tools Used
To conduct this analysis, the following tools and techniques were utilized in Microsoft Excel:
- **Power Query** — For data extraction, transformation, and loading (ETL).
- **M-Code** — Used in Power Query to automate data transformation.
- **Power Pivot** — For data modeling and creating relationships between tables.
- **DAX Functions** — To perform advanced calculations using measures and calculated columns.
  
## 4. Data Sourcing — ETL
The sales data from 2011 to 2016 was sourced from @myDataClique and processed in Excel. The data underwent extensive ETL (Extract, Transform, Load) processes:
### **Raw Sales Data** → **Data Import and Formatting**
1. Imported sales data from 2011–2014 and 2015–2016 into Power Query.
2. Cleaned the data by removing unnecessary rows and standardizing column formats.
3. Split location details into separate columns: **Location ID, Country, and State**.
4. Used "Extract Text Between Delimiters" to clean product categories by removing unnecessary characters.
5. Merged both datasets into a single table using the Append Function, creating a **Sales 2011–2016 dataset**.

## 5. Data Modeling
To enable effective analysis, the data was structured using the **Star Schema approach**:

### **Fact Table:**
- **SalesFact** — Contains all transaction records, including Customer ID, Product ID, Location ID, and Sales Amount.
- Includes foreign keys linking to dimension tables.

### **Dimension Tables:**
- **DimCustomer** — Stores customer attributes (Customer ID, Age, Gender).
- **DimProduct** — Contains product details (Product ID, Category, Subcategory, Product Name).
- **DimLocation** — Holds location data (Location ID, Country, State).
- **DimDate** — Created using M-Code to analyze sales across years, months, weeks, and days.

### **Data Relationships:**
- Imported the data into **Power Pivot** to manage relationships.
- Established **one-to-many** relationships between the **dimension tables** and the **SalesFact** table using **primary and foreign keys**.

![Data Relationships](./images/Data%20Relationship.JPG)

## 6. Analysis & Key Metrics
The analysis focused on **key performance indicators (KPIs)** and deeper insights into **revenue trends, customer behavior, and regional and product performance**.

### **Key Performance Indicators (KPIs)**
- **Total Revenue:** $95,176,318
- **Total Profit:** $42,126,410
- **Total Customers:** 8,232
- **Total Products Sold:** 130
- **Average Order Value:** $842
- **Average Revenue per Customer:** $11,562

### **Revenue Growth Analysis**
- Revenue continuously increased and peaked in 2015 at $22.4M before a slight decline to $19.7M in 2016.
- The strongest growth period was 2013–2015, indicating effective sales expansion.

### **Customer Demographics**
- The majority of customers fall within ages 25–34 (3,441) and 35–44 (2,778).
- Gender distribution is nearly equal: 4,066 female customers vs. 4,166 male customers.

### **Regional Sales Performance**
- United States leads with $30.8M revenue and 2,358 customers.
- Australia follows with $25.4M in revenue and 1,849 customers.
- The UK has the highest revenue per customer ($17,087), followed by Canada ($12,015) but both have the lowest number of customers at 649 and 667 respectively.

### **Product Performance Analysis**
- Mountain-200 and Road-150 models are the most profitable.
- Accessories have the highest profit margin (62.6%).

## 7. Key Insights and Recommendations

### **Key Insights**
#### **Revenue and Profitability**
1. Strong revenue growth from $10.1M (2011) to $22.4M (2015), with a slight dip to $19.7M (2016).
2. Healthy profit margins (44.2%) driven by high-margin product categories.
3. Accessories lead in profitability (62.6% margin), while Bikes generate the most revenue ($69.3M).

#### **Product Performance**
1. Mountain-200 and Road-150 series dominate sales.
2. The Mountain-200 Black, 38 variant alone brought in $1.7M in profit.

#### **Customer Demographics**
1. The majority of customers fall into 25–34 (3,441 customers) and 35–44 (2,778 customers) age groups.
2. Balanced gender distribution: 4,066 female customers vs. 4,166 male customers.

#### **Geographic Distribution**
1. United States leads in revenue ($30.8M, 2,358 customers).
2. The United Kingdom has the highest revenue per customer ($17,087).
3. Canada shows potential for improvement, with similar customer numbers to the UK but lower revenue per customer.

### **Recommendations**
#### **Product Strategy**
- Expand high-margin accessories with bike-specific bundles.
- Phase out underperforming bike models.
- Invest in size-specific features based on sales data.

#### **Market Development**
- Investigate UK’s higher revenue per customer for potential best practices.
- Develop targeted marketing campaigns for the 25–44 age group.
- Improve strategies for Canada, which has untapped potential.

#### **Customer Engagement**
- Implement a loyalty program targeting top spenders.
- Create age-specific product bundles to enhance value propositions.
- Develop retention programs for older demographics to expand customer lifetime value.

## 8. Conclusion
BrightMart’s sales data reveals a thriving business with strong revenue and profit margins. The insights gained from this analysis highlight key opportunities for growth, including product diversification, targeted marketing, and regional strategy optimization. By leveraging these findings, BrightMart can continue to refine its product offerings and marketing efforts, positioning itself for sustained success in the competitive retail industry.
