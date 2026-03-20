# 📊 E-Commerce Sales Analysis (Excel Capstone Project)

## 🧹 Data Cleaning
- Removed inconsistencies in **Customer ID** and **Country** using *Find & Replace*.
- Standardized **Customer Name** column with `TRIM()` and `PROPER()` functions.
- Corrected inconsistent **Product ID** entries in Sheet 2.
- Ensured clean relationships across sheets for analysis.

## 🔧 Data Imputation
- Filled blanks in **Loyalty Level** with `"Unknown"` using:
  ```excel
  =IF(ISBLANK(cell),"Unknown",cell)
- Imputed missing values in Cost and Stock using AVERAGEIF() based on Sub-category.
- In Sales Fact (Sheet 4), blanks in Quantity, Unit Price, Discount, Total Price were imputed using AVERAGEIF() grouped by Payment Type.
- Applied VLOOKUP to merge details across sheets for pivot table creation.
## 📈 Data Analysis
- Leveraged Data Analysis ToolPak to compute:
- Sum, Average, Median, Mode
- Skewness of sales metrics
- Conducted statistical checks with INDEX(MODE(MATCH())) for gender-based purchase validation.
## 📊 Pivot Tables & Graphs
- Gender-wise purchase count
- Loyalty level distribution
- Region-wise total sales
- Store type vs. total sales
- Payment type vs. total sales (via GPT AI for Excel)
- Added Slicers for interactive visualizations
## 💡 Key Insights
- Gender: Female customers dominate purchases, showing higher shopping interest.
- Loyalty: Platinum membership leads with 606 customers.
- Region: North region tops sales with ₹6,47,300.
- Store Type: Online sales outperform with ₹9,13,898.
- Payment Type: PayPal records the highest sales at ₹7,56,717.
- Note: GPT AI-generated payment type graph is static (no slicer interactivity).

✨ This project demonstrates end-to-end data cleaning, imputation, analysis, and visualization in Excel, providing actionable insights into e-commerce sales trends.

