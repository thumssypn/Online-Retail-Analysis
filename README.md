
# 📊 Excel Sales & Cohort Analysis Dashboard

This project is an **interactive Excel-based dashboard** that analyzes retail sales performance and customer retention trends over time.  
The dashboard leverages real-world transactional data and Excel features like **PivotTables**, **charts**, and **KPI cards** to provide actionable insights for businesses.

---

## 📁 Project Files

| File Name   | Description                                                    |
|-------------|----------------------------------------------------------------|
| `SalesCohortAnalysis.xlsx` | Excel workbook containing cleaned data, PivotTables, cohort calculations, and dashboards. |

---

## 🔍 Dataset Source

The dataset used in this project is from Kaggle:  
🔗 [Online Retail Dataset by Ersan Y](https://www.kaggle.com/datasets/ersany/online-retail-dataset)  

It contains transactional sales data for a UK-based online retail company.

---

## 🧹 Data Cleaning Process

The dataset was cleaned and prepared using Excel 2016.  
Key cleaning steps included:
- ✅ **Removed duplicate rows.**
- ✅ **Excluded rows where the Country was blank or unspecified.**
- ✅ **Deleted rows with null values in all columns.**
- ✅ Filtered out invalid data such as negative quantities and missing Invoice Numbers.
- ✅ Standardized the **Purchase Month** format as "Month Year" (e.g., “December 2010”).
- ✅ Created helper columns for:
  - **Purchase Month**
  - **Cohort Month**
  - **Cohort Index** (Month number since first purchase)

---

## 🎯 Dashboards Overview

### 1. Sales Analysis Dashboard

Analyzes sales trends and identifies top products, countries, and customers.

#### ✅ KPIs
- **Total Sales**
- **Average Invoice Value**
- **Customer Count**

#### 📊 Visualizations
| Chart Type          | Insights Shown                               |
|---------------------|----------------------------------------------|
| Line Chart          | Sales trend by month                         |
| Column Chart        | Customers acquired by month                  |
| Horizontal Bar Chart| Top 5 Countries by Sales                     |
| Horizontal Bar Chart| Top 10 Products by Quantity                  |
| Pie Chart           | Top 10 Customers by Sales                    |

#### 🎛️ Filters
- Country
- Month-Year
- Product Description

---

### 2. Cohort Analysis Dashboard

Analyzes how customer retention changes over time.

#### ✅ KPIs
| Metric                     | Description                          |
|-----------------------------|--------------------------------------|
| Customer Count              | Total unique customers              |
| Total Sales                 | Total sales across all cohorts     |
| Average Sales per Customer  | Total sales ÷ Customer count       |
| First Month Retention       | % of customers who returned in month 2 |
| Average Cohort Retention    | Average retention rate across months |

#### 📊 Visualizations
| Chart Type           | Insights Shown                            |
|----------------------|--------------------------------------------|
| Line Chart           | Retention trends for each cohort month   |
| 100% Stacked Bar     | Retention breakdown over 13 months       |
| Column Chart         | Customers acquired per month             |
| Heatmap Table        | Retention rates with conditional formatting |

#### 📋 Example Retention Table

| Cohort Month | 1   | 2   | 3   | ... | 13  | First Month Retention | Avg. Retention |
|--------------|-----|-----|-----|-----|-----|----------------------|----------------|
| Dec 2010     |100% | 38% | 33% | ... | 27% | 38%                  | 42%            |
| Jan 2011     |100% | 24% | 28% | ... |     | 24%                  | 34%            |

---

## 📈 Insights Gained
- Sales peak in **November–December**.
- The **United Kingdom** generates the highest sales volume.
- Most customers churn after their first purchase (avg. first-month retention ~30–40%).
- December 2010 and October 2011 cohorts had better retention rates.

---

## ⚙️ Excel Features Used

| Feature                          | Purpose                                   |
|-----------------------------------|-------------------------------------------|
| PivotTables & PivotCharts         | Data summarization and visualization     |
| Slicers                           | Dynamic filtering                        |
| VLOOKUP                           | Map cohort purchase month                |
| Helper Columns                    | Create cohort month/index                |
| Conditional Formatting            | Highlight retention heatmap              |
| KPI Cards in Text Boxes           | Display live metrics                     |
| Stacked Bar & Line Charts         | Show cohort and sales trends             |

---

## 🚀 How to Use the Dashboard

### ✅ Prerequisites
- Excel 2016 or later.

### ✅ Usage Steps
1. Open `Work.xlsx`.
2. Explore the **Sales Analysis Dashboard** and apply slicers to filter by Country, Month, or Product.
3. Switch to the **Cohort Analysis Dashboard** to study customer retention over time.
4. Use slicers to view cohort retention by product category or country.
5. Analyze retention patterns using the heatmap and line/stacked bar charts.

---

## 🔬 Future Improvements

- Automate cohort calculations using **Power Query** or VBA.
- Build a **Power BI** dashboard version.
- Add sales and retention forecasting using Excel’s **Forecast Sheet**.

---

## 📚 Example Use Cases

- **Retail analysts:** Understand product performance and sales trends.
- **Marketers:** Measure customer retention across marketing campaigns.
- **E-commerce managers:** Optimize sales strategies based on customer lifetime value.
- **Data analysts:** Practice cohort analysis and dashboarding in Excel.
