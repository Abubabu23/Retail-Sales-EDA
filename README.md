# Sales Performance Analytics - Exploratory Data Analysis (EDA)

## **Project Overview**
This project performs an exploratory data analysis on sales data to understand revenue patterns, identify top-performing products and customers, and uncover trends over time. The goal is to support data-driven business decisions by analyzing monthly, daily, and hourly sales, as well as product and customer behavior.

---

## **Business Objective**
- Analyze sales trends over time (daily, monthly, yearly, hourly).  
- Identify top-selling and least-selling products.  
- Understand customer purchasing behavior and frequent buyers.  
- Examine sales across different countries.  
- Detect returns and anomalies in sales data.  

---

## **Dataset**
The dataset contains transactional sales records for various products sold to customers across multiple countries.

**Key Columns:**
| Column Name     | Description |
|----------------|-------------|
| `InvoiceNo`    | Unique invoice number |
| `StockCode`    | Product code |
| `Description`  | Product name/description |
| `Quantity`     | Number of items sold (negative for returns) |
| `InvoiceDate`  | Date and time of invoice |
| `UnitPrice`    | Price per item |
| `CustomerID`   | Unique customer identifier |
| `Country`      | Country of customer |

---

## **EDA Steps**
1. **Data Cleaning**
   - Removed missing values
   - Removed duplicates
   - Corrected data types (`InvoiceDate` as datetime)
   - Handled negative values (returns)
   - Checked for outliers

2. **Feature Engineering**
   - Created `Total Sales` column (`Quantity * UnitPrice`)  
   - Extracted `year`, `month`, `day`, `Hour` from `InvoiceDate`  
   - Created `InvoiceMonth` for monthly trend analysis  
   - Created `IsReturn` column to flag returned items

3. **Sales Trend Analysis**
   - Month-wise, year-wise, daily, and hourly sales analysis  
   - Visualizations using bar and line charts

4. **Product Sales Analysis**
   - Top 10 products by revenue and quantity  
   - Bottom 10 products by revenue  

5. **Customer Analysis**
   - Top 10 customers by revenue  
   - Top 10 customers by purchase frequency  

6. **Country-based Analysis**
   - Revenue by country  
   - Number of orders by country  

---

## **Visualization Libraries Used**
- Matplotlib  
- Seaborn  
- NumPy  
- Pandas  

---

## **How to Run**
1. Clone the repository:
```bash
git clone https://github.com/<YourUsername>/Sales-Performance-EDA.git
