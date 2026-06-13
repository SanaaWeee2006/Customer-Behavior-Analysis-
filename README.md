# Customer Shopping Behavior Analysis

## Overview

Customer Shopping Behavior Analysis is an end-to-end data analytics project focused on understanding customer purchasing patterns, product preferences, spending behavior, and subscription trends. Using Python, SQL, and Power BI, the project transforms raw transactional data into actionable business insights that can support marketing, customer retention, and revenue growth strategies.

---

## Dataset

The dataset contains **3,900 customer purchase records** with **18 features** covering:

### Customer Information

* Customer ID
* Age
* Gender
* Location
* Subscription Status

### Purchase Information

* Item Purchased
* Category
* Purchase Amount (USD)
* Season
* Size
* Color

### Shopping Behavior

* Discount Applied
* Promo Code Used
* Previous Purchases
* Frequency of Purchases
* Review Rating
* Shipping Type

### Data Quality

* Total Records: **3,900**
* Missing Values: **37 records in Review Rating**

---

## Tools & Technologies

### Python

* Pandas
* NumPy

### Database

* SQL Server

### Business Intelligence

* Power BI

### Development Environment

* Jupyter Notebook

---

## Project Workflow

### 1. Data Loading & Exploration

* Imported the dataset using Pandas.
* Examined dataset structure using:
  * `df.info()`
  * `df.describe()`
* Identified missing values and data quality issues.

### 2. Data Cleaning

* Handled missing values in the Review Rating column using median ratings by product category.
* Verified data consistency across fields.

### 3. Feature Engineering

Created additional features to improve analysis:

* **Age Group** classification
* **Purchase Frequency Days**
* Customer behavior indicators

Removed redundant fields after validation:
* Dropped `promo_code_used` due to redundancy with discount information.

### 4. Database Integration

* Connected Python to SQL Server.
* Loaded the cleaned dataset into the database.
* Performed SQL-based business analysis.

---

## SQL Analysis

The following business questions were answered using SQL:

### Revenue Analysis

* Revenue by Gender
* Revenue by Age Group
* Subscribers vs Non-Subscribers Revenue Comparison

### Customer Behavior Analysis

* High-Spending Discount Users
* Repeat Buyers and Subscription Relationship
* Customer Segmentation:
  * New Customers
  * Returning Customers
  * Loyal Customers

### Product Analysis

* Top 5 Products by Average Rating
* Top 3 Products per Category
* Discount-Dependent Products

### Purchase & Logistics Analysis

* Shipping Type Comparison
* Discount Usage Patterns

---

## Power BI Dashboard

An interactive Power BI dashboard was developed to visualize customer shopping behavior and business performance.

### Dashboard Highlights

* Total Customers
* Total Revenue
* Average Purchase Amount
* Revenue by Gender
* Revenue by Age Group
* Product Category Performance
* Customer Segmentation Analysis
* Subscription Status Breakdown
* Discount Usage Analysis
* Shipping Type Insights

---

## Key Insights

* Customer spending varies across demographic groups.
* Subscription status influences overall revenue contribution.
* Certain products rely heavily on discounts to drive sales.
* Loyal customers contribute significantly to repeat purchases.
* Product ratings help identify high-performing products.
* Shipping preferences impact average purchase amounts.

---

## Business Recommendations

### Increase Subscription Adoption

Promote exclusive benefits and loyalty rewards to encourage more customers to subscribe.

### Strengthen Customer Retention

Implement loyalty programs targeting returning customers to convert them into loyal customers.

### Optimize Discount Strategy

Monitor discount-dependent products and balance promotional activities with profit margins.

### Promote High-Performing Products

Highlight top-rated and frequently purchased products in marketing campaigns.

### Improve Targeted Marketing

Focus campaigns on high-revenue age groups and customer segments with stronger purchasing behavior.

---
