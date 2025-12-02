# 🛒 Walmart Store Sales Analysis  
**Comprehensive data analysis of Walmart's multi-year retail performance using SQL, Python, and Tableau**

---

## 📌 Project Overview  
This project analyzes historical weekly sales data from 45 Walmart stores across different regions.  
The goal is to understand the drivers of store performance, the impact of holidays and markdown events, and trends across time.  

This project demonstrates skills in:
- Data cleaning & feature engineering  
- SQL querying (joins, aggregations, window functions)  
- Exploratory data analysis (EDA)  
- Time-series and seasonal analysis  
- Business insights & data storytelling  
- Interactive dashboard development in Tableau  

---

## 📂 Project Structure

walmart-sales-analysis/
│
├── data_raw/        # Raw CSVs from Kaggle
├── data_clean/      # Cleaned and combined datasets
├── sql/             # All SQL queries (joins, cleaning, analysis)
├── notebooks/       # Python EDA notebooks (Colab or Jupyter)
├── dashboard/       # Tableau workbook and exports
├── docs/            # Documentation & notes
└── images/          # Charts & visuals used in README

---

## 📊 Dataset Description

This project uses 4 datasets provided by Walmart:

### **1. train.csv**
Weekly department-level sales from 2010–2012  
**Columns:** Store, Dept, Date, Weekly_Sales, IsHoliday

### **2. features.csv**
Store-level economic & promotional data  
**Columns:** Temperature, Fuel_Price, CPI, Unemployment, MarkDown1–5, IsHoliday

### **3. stores.csv**
Store metadata  
**Columns:** Store, Type, Size

### **4. test.csv**
Future records without Weekly_Sales (used for forecasting tasks)

---

## 🤖 Tools Used

- **SQL** — data cleaning, joins, window functions  
- **Python (Pandas, Matplotlib, Seaborn)** — EDA, feature exploration  
- **Tableau** — interactive dashboards and KPIs  
- **GitHub** — version control & project organization  

---

## 🧹 Data Cleaning Summary
Steps completed during cleaning:

- Joined `train`, `stores`, and `features` into a unified dataset  
- Converted Date column to datetime format  
- Handled missing values in MarkDown fields  
- Verified uniqueness of Store/Dept/Date combinations  
- Removed duplicate rows  
- Checked for outliers in Weekly_Sales  
- Created holiday flags and time-based features (Year, Month, Week)  

Full cleaning documentation:  
➡️ `docs/cleaning_steps.md` *(to be added)*

---

## 🔍 Exploratory Analysis (EDA)

Key questions explored:

1. **Which stores and departments have the highest sales?**  
2. **How do holidays impact sales performance?**  
3. **How do fuel prices, temperature, CPI, and unemployment relate to sales?**  
4. **Which store types generate the most revenue?**  
5. **What long-term seasonal patterns exist in the data?**  
6. **Do markdown events increase sales during holiday weeks?**

Examples of visuals included:  
- Weekly sales trend line  
- Year-over-year comparison  
- Store performance bar chart  
- Holiday vs non-holiday boxplots  
- Correlation heatmaps  
- Markdown impact charts  

Visuals stored in `images/`.

---

## 📈 Dashboard

An interactive Tableau dashboard highlights:

- Total & average weekly sales  
- Store-level and department-level performance  
- Holiday event analysis  
- Economic feature correlations  
- Time-series trends  

🔗 **Tableau Dashboard:** *[ADD LINK HERE]*  
*(Will be published after dashboard is complete)*

---

## 💡 Key Insights (to be filled as you complete analysis)

A few examples you may uncover:

- Holiday weeks show **5× spikes** in several high-performing departments  
- Store Type A may outperform Type B due to larger average size  
- Markdown promotions have measurable impact during November/December  
- Unemployment and CPI trends align with dips in customer spending  
- Seasonal patterns peak in late November and early December each year  

You will fill in real insights when analysis is done.

---

## 🛠 SQL Files Included  
- `sql/01_join_tables.sql`  
- `sql/02_cleaning.sql`  
- `sql/03_aggregations.sql`  
- `sql/04_time_series_analysis.sql`  
- `sql/05_holiday_analysis.sql`  

---

## 🧠 What I Learned
This project strengthened my skills in:

- Joining large relational datasets  
- Designing a clean, repeatable project workflow  
- Analyzing time-series data  
- Building business insights from retail sales  
- Creating dashboards aligned with stakeholder needs  
- Working with real-world messy data (missing values, incomplete records)

---

## 🚀 Next Steps
Future improvements may include:

- Forecasting future sales using ARIMA or XGBoost  
- Store-level predictive models  
- Clustering stores by performance patterns  

---

## 📎 Dataset Source  
Walmart Recruiting Store Sales Forecasting  
https://www.kaggle.com/competitions/walmart-recruiting-store-sales-forecasting/data

---