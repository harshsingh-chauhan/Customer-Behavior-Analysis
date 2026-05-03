# Customer Shopping Behavior Analysis

## 📊 Project Overview
This project involves an end-to-end analysis of customer shopping behavior using transactional data from 3,900 purchases across various product categories. The primary objective is to uncover actionable insights into spending patterns, customer segments, product preferences, and subscription behaviors to drive strategic business decisions.

## 🗄️ Dataset Summary
* **Records:** 3,900 rows
* **Features:** 18 columns
* **Key Data Points:**
  * **Customer Demographics:** Age, Gender, Location, Subscription Status
  * **Purchase Details:** Item Purchased, Category, Purchase Amount, Season, Size, Color
  * **Shopping Behavior:** Discount Applied, Promo Code Used, Previous Purchases, Frequency of Purchases, Review Rating, Shipping Type

## 🛠️ Methodology & Tech Stack
The analysis was conducted in three main phases using a robust modern data stack:

### 1. Exploratory Data Analysis & Cleaning (Python/Pandas)
* **Data Imputation:** Handled 37 missing values in the `Review Rating` column by imputing the median rating of each respective product category.
* **Standardization:** Converted all column names to snake_case for database compatibility.
* **Feature Engineering:** Created new features such as `age_group` (via binning) and `purchase_frequency_days`.
* **Data Integration:** Loaded the cleaned dataset into a PostgreSQL database using Python.

### 2. Business Logic & Querying (PostgreSQL)
Structured SQL queries were developed to answer critical business questions, including:
* Revenue comparisons by gender (Male customers generated $157,890 vs. Female customers at $75,191).
* Identification of high-spending discount users.
* Profiling subscribers vs. non-subscribers (Subscribers have a slightly lower average spend but represent a critical loyalty segment).
* Customer segmentation into "New", "Returning", and "Loyal" categories.
* Revenue breakdowns by age group, highlighting "Young Adults" as the highest revenue-driving demographic ($62,143).

### 3. Data Visualization (Power BI)
Developed an interactive Power BI dashboard to present KPIs and insights to stakeholders. Features include:
* Top-level KPIs: Total Customers (3.9K), Average Purchase Amount ($59.76), Average Review Rating (3.75).
* Breakdown of customer subscription base (27% Subscribers vs. 73% Non-Subscribers).
* Revenue and Sales distributions categorized by Product Category (Clothing, Accessories, Footwear, Outerwear) and Age Group.

## 💡 Key Business Recommendations
Based on the data analysis, the following strategic actions are recommended:
1. **Boost Subscriptions:** Promote exclusive benefits for subscribers to increase the current 27% adoption rate, as repeat buyers are highly correlated with subscription status.
2. **Customer Loyalty Programs:** Reward repeat buyers to transition them into the "Loyal" segment (currently at 3,116 customers).
3. **Review Discount Policy:** Re-evaluate discount strategies on highly discount-dependent items (e.g., Hats, Sneakers) to balance sales velocity with profit margins.
4. **Product Positioning:** Feature top-rated items (Gloves, Sandals, Boots) and best-selling categories (Clothing, Accessories) prominently in upcoming marketing campaigns.
5. **Targeted Marketing:** Focus acquisition and retention efforts on high-revenue age groups (Young Adults and Middle-Aged) and optimize promotions for Express shipping users.

## 👨‍💻 Author
**Professional Data Analyst** *Specializing in Data Preparation, SQL Analytics, and Business Intelligence Visualization.*
