# 🛒 E-Commerce Market Analysis

## 📌 Project Overview

E-Commerce Market Analysis is a data analytics project that focuses on collecting, cleaning, analyzing, and visualizing e-commerce product data to generate meaningful business insights.

The project analyzes product categories, vendors, prices, discounts, ratings, reviews, and stock availability using Python, SQL, and Power BI.

## 🎯 Project Objectives

- Collect e-commerce product data using web scraping.
- Clean and preprocess the collected dataset.
- Perform Exploratory Data Analysis (EDA) using Python.
- Analyze product data using SQL and MySQL.
- Create interactive dashboards using Power BI.
- Identify useful business insights and recommendations.

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Python | Data collection and analysis |
| Requests | Fetch product webpages |
| BeautifulSoup | Extract information from webpages |
| Pandas | Data cleaning and manipulation |
| NumPy | Numerical operations |
| Matplotlib | Data visualization |
| Seaborn | Statistical visualization |
| MySQL | Store and manage structured data |
| SQL | Query and analyze data |
| Power BI | Interactive dashboard creation |
| GitHub | Project documentation and version control |

## 🔄 Project Workflow

1. **Web Scraping** – Collected product information from Scraping Sandbox.
2. **Data Cleaning** – Removed duplicate records, converted data types, standardized stock values, and checked invalid and missing values.
3. **Exploratory Data Analysis** – Analyzed categories, prices, discounts, ratings, reviews, vendors, and stock availability.
4. **SQL Analysis** – Used MySQL queries to analyze product data.
5. **Data Visualization** – Created charts using Matplotlib and Seaborn.
6. **Power BI Dashboard** – Developed two interactive dashboard pages.
7. **Business Insights** – Identified important patterns and recommendations.

## 📊 Dataset Overview

The final dataset contains **491 products** collected from an e-commerce practice website.

| Metric | Value |
|---|---:|
| Total Products | 491 |
| Total Vendors | 20 |
| Total Categories | 15 |
| Average Product Price | $103.97 |
| Average Rating | 4.02 |
| Products In Stock | 418 |
| Products Out of Stock | 73 |
| Total Reviews | 114,846 |
| Average Available Discount | 30.55% |

**Note:** Some products do not have original-price information. These unavailable values were retained as NULL instead of assuming values.

## 🧹 Data Cleaning

The following preprocessing activities were performed:

- Checked and removed duplicate product records.
- Converted numerical columns to appropriate data types.
- Standardized stock status values.
- Checked for invalid product prices.
- Checked missing values in important columns.
- Retained unavailable original-price and discount values as NULL.

## 📈 Exploratory Data Analysis (EDA)

EDA was performed using Python, Pandas, NumPy, Matplotlib, and Seaborn.

The analysis includes:

- Product distribution by category.
- Average price by category.
- Average discount by category.
- Price distribution.
- Rating distribution.
- Stock availability.
- Price versus rating.
- Price versus reviews.
- Discount distribution.
- Vendor comparison.

## 🗄️ SQL Analysis

The cleaned dataset was imported into MySQL using the table name:

`ecommerce_products_cleaned`

SQL queries were used to:

- Count total products.
- Calculate category-wise product counts.
- Find average, minimum, and maximum prices.
- Calculate average product ratings.
- Analyze stock availability.
- Identify the most-reviewed products.
- Find products with the highest discounts.
- Compare vendors by product count.
- Identify products with a rating of 5.

## 📊 Power BI Dashboard

The project includes two dashboard pages.

### Page 1: Market Overview

- Total Products
- Total Vendors
- Total Categories
- Average Price
- Average Rating
- Products by Category
- Products by Vendor
- Stock Availability
- Price Segment Distribution
- Interactive slicers for Category, Vendor, and Price Segment

### Page 2: Pricing & Product Insights

- Average Price by Category
- Average Discount by Category
- Price vs. Rating Scatter Plot
- Top 10 Most Reviewed Products

## 🔍 Key Findings

- The dataset contains 491 products across 20 vendors and 15 categories.
- Electronics has the highest product count, with 44 products.
- 418 products are in stock, while 73 are out of stock.
- The Premium price segment contains 248 products.
- The average product rating is 4.02.
- The dataset contains 114,846 total reviews.
- The average available discount is 30.55%.
- The price-rating correlation is approximately 0.06, indicating a very weak linear relationship between price and rating.

## 💡 Business Recommendations

- Monitor out-of-stock products to identify potential availability issues.
- Compare prices across categories to understand pricing patterns.
- Analyze highly reviewed products to identify products that attract customer attention.
- Evaluate discount patterns across categories and vendors.
- Use vendor-level analysis to compare product distribution and performance.

## 📁 Project Structure

```text
ecommerce-market-analysis/
│
├── scrape_ecommerce.py
├── clean_data.py
├── eda.py
├── ecommerce_products_cleaned.csv
├── ecommerce Market analysis sql file.sql
├── eda_charts/
├── README.md
└── .gitignore
