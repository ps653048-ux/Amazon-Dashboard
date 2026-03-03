## 📌 Project Overview
This project analyzes Amazon product listing data to understand pricing strategy, discount patterns, and customer perception using Power BI.

The goal was to explore whether discount strategies influence customer ratings and engagement, and to identify high-performing and underperforming product categories.

---

## 📂 Dataset Description

The dataset contains product-level information including:

- Product ID
- Product Name
- Main Category
- Sub Category
- Actual Price
- Discounted Price
- Discount Percentage
- Rating
- Rating Count

This is NOT transactional sales data.  
It is product listing and review-based data.

---

## 🛠 Tools Used

- Power Query (Data Cleaning & Transformation)
- Power BI (Data Modeling & Visualization)
- DAX (Measures & Calculated Columns)

---

## 🧹 Data Cleaning Process (Power Query)

The following steps were performed:

- Removed null and duplicate records
- Corrected data types (Price → Decimal, Rating → Decimal, Rating Count → Whole Number)
- Standardized discount percentage format
- Cleaned text columns (Product Name & Category)
- Created calculated columns where necessary

The cleaned dataset was then loaded into Power BI for analysis.

---

## 📊 Key Measures Created (DAX)

### Pricing Metrics
- Average Actual Price
- Average Discounted Price
- Average Discount %
- Discount Amount (Actual - Discounted)

### Customer Perception Metrics
- Average Rating
- Total Rating Count
- Weighted Rating (Rating adjusted by rating_count)

### Product Distribution Metrics
- Total Products
- Products per Category
- Price Band Classification (Low / Medium / High)

---

## 📈 Dashboard Structure

Includes:

- KPI Cards (Avg Price, Avg Discount %, Avg Rating, Total Products, Total Rating Count)
- Products by Category (Bar Chart)
- Average Rating by Category
- Scatter Plot:
  - X-axis → Average Discount %
  - Y-axis → Average Rating
  - Size → Total Rating Count
  - Legend → Main Category

This page answers:
- Does higher discount improve customer satisfaction?
- Which categories rely heavily on discounting?
- Which categories have the highest engagement?

---

Includes:

- Price Band Distribution
- Category-wise Discount & Rating Comparison
- Top 10 Most Reviewed Products
- Engagement Analysis using Rating Count

This page identifies:
- High-rated but low-visibility products (Hidden Gems)
- Over-discounted but low-rated categories
- Highly engaged product categories
- Premium vs Budget product performance

---

## 🔍 Key Insights Generated

1. Some categories maintain high ratings even with low discounts, indicating strong product-market fit.
2. Heavy discounting does not always correlate with higher ratings.
3. Certain categories generate significantly higher customer engagement (rating_count).
4. High-discount categories with low ratings may indicate overpricing or product quality issues.
5. Premium-priced products tend to have stable ratings but lower engagement volume.

---

## 💡 Business Recommendations

- Avoid over-discounting low-rated products.
- Increase visibility of high-rated, low-engagement products.
- Focus on categories that perform well without heavy discounting.
- Use rating_count as a proxy for prod# 📌 
