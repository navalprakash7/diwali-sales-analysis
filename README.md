# Diwali Sales Analysis

Exploratory data analysis of Diwali sales data to understand customer demographics, purchasing behavior, and top-performing states, occupations, and product categories.

## Dataset

**File:** `Diwali_Sales_Data.csv`
**Rows:** 11,251 | **Columns:** 15

| Column | Description |
|---|---|
| User_ID | Unique customer identifier |
| Cust_name | Customer name |
| Product_ID | Unique product identifier |
| Gender | Customer gender |
| Age Group | Customer age bracket |
| Age | Customer age |
| Marital_Status | 0 = Unmarried, 1 = Married |
| State | Customer's state |
| Zone | Geographic zone |
| Occupation | Customer's profession |
| Product_Category | Category of purchased product |
| Orders | Number of orders |
| Amount | Sale amount (₹) |
| Status, unnamed1 | Empty/unused columns (dropped during cleaning) |

## Notebook

**File:** `sales_analysis.ipynb`

### Steps performed
1. **Data Loading & Cleaning**
   - Load CSV with `unicode_escape` encoding
   - Drop empty columns (`Status`, `unnamed1`)
   - Drop null rows
   - Convert `Amount` to integer

2. **Exploratory Data Analysis**
   - Gender distribution and total spend by gender
   - Age group distribution by gender and spend by age group
   - Top 10 states by orders and by total sales
   - Marital status distribution and spend by marital status & gender
   - Occupation distribution and spend by occupation
   - Product category distribution and spend by category
   - Top 10 best-selling products

## Key Findings
- **Gender:** Majority of buyers are **female**, and women have higher purchasing power than men.
- **Age:** Most buyers fall in the **26–35 years** age group, predominantly female.
- **State:** Top sales come from **Uttar Pradesh, Maharashtra, and Karnataka**.
- **Marital Status:** **Married women** are the dominant high-spending segment.
- **Occupation:** Buyers mostly work in **IT, Healthcare, and Aviation**.
- **Product Category:** Top-selling categories are **Food, Clothing, and Electronics**.

## Conclusion
Married women aged 26–35 from Uttar Pradesh, Maharashtra, and Karnataka, working in IT, Healthcare, and Aviation, are the most likely customer segment to purchase Food, Clothing, and Electronics products.

## Requirements
```
numpy
pandas
matplotlib
seaborn
```

## Usage
```bash
jupyter notebook sales_analysis.ipynb
```
