# ecommerce-sales-analysis
Analyzing E-Commerce Sales Data: Cleaning, Revenue Trends, Product &amp; Country Insights
# E-Commerce Sales Analysis 🛍️📈

This project focuses on analyzing an E-Commerce transaction dataset to uncover revenue trends, top-selling products, and geographic performance insights using Python and data visualization libraries.

---

## 📦 Dataset Source

We use a public dataset from Kaggle, which contains transaction-level data for a UK-based online retail store.

🔗 [Dataset: Online Retail Dataset – Kaggle](https://www.kaggle.com/datasets/vijayuv/onlineretail)

---

## 📚 Library Imports and Setup

We begin by importing essential Python libraries:
- `pandas` for data manipulation
- `matplotlib` and `seaborn` for data visualization
- `datetime` for handling date features

---

## 🧾 Data Loading

The dataset (`data.xls`) is loaded into a pandas DataFrame. During this phase:
- Encoding is handled for proper parsing
- Date fields are converted to datetime objects for analysis
- Null values and cancellations are preprocessed

---

## 🧹 Data Preprocessing

Key preprocessing steps include:
- Removing rows with missing `CustomerID`
- Filtering out negative `Quantity` values (likely returns)
- Creating new features:
  - `TotalPrice` = `Quantity × UnitPrice`
  - `Month` = Extracted from `InvoiceDate` for monthly trend analysis
- Standardizing column names

---

## 📊 Visualization & Insights

1. **Monthly Revenue Trend**
   - Line chart showing total sales revenue over time

2. **Top 10 Countries by Revenue**
   - Horizontal bar chart highlighting the highest contributing countries

3. **Top 10 Products by Revenue**
   - Visualization of best-selling products based on total revenue

4. **Correlation Heatmap**
   - Examines relationships between `Quantity`, `UnitPrice`, and `TotalPrice`

5. **Pie Chart: Top 5 Countries by Order Count**
   - Distribution of orders by country

6. **Boxplot of Unit Prices**
   - Analyzes the price range and outliers

7. **Histogram: Total Order Value**
   - Shows the frequency of different sales amounts

8. **Scatter Plot: Quantity vs. Unit Price**
   - Detects pricing anomalies and volume trends

---

## ✅ Output & Findings

- Revenue is highest in certain peak months, indicating seasonal trends.
- A few countries and products dominate the revenue share.
