
# 🧮 Firmable – Data Quality Assessment  
**Prepared by:** *Antony Rohan R*  

---

## 📘 Overview  
This project focuses on evaluating , enhancing the quality of a **“news events”** dataset and building a pipeline using **Python**, **SQL**, and **Tableau**.  
The objective was to identify key data quality issues, apply systematic cleaning and validation steps, and visualize improvements between the **raw** and **cleaned** datasets.  

---

## 🗃️ SQL Data Setup & Cleaning  
SQL scripts were developed to define the database structure, store cleaned data, and track quality metrics.  

### Main Tables  

| Table Name | Description |
|-------------|-------------|
| `news_events_cleaned` | Stores cleaned and standardized event data with metadata. |
| `dq_metrics_run`      | Captures data quality metrics such as duplicates removed, invalid URLs, and missing counts before and after cleaning. |

---

## 🐍 Python Data Cleaning (Jupyter Notebook)  
The notebook **`Firmable_assessment.ipynb`** handled data profiling, cleaning, and validation tasks.  

### Key Steps  
- Profiling for missing values, duplicates, and invalid URLs  
- Standardizing company names, URLs, and phone numbers  
- Handling nulls and ensuring data type consistency  
- Removing duplicate and invalid entries  
- Exporting the cleaned dataset for Tableau visualization  

---

## 📊 Tableau Visualization  
A **bar chart** was created in Tableau to compare data quality metrics between **Raw Data** and **Cleaned Data**.  

### Metrics Compared  
- Total count  
- Missing article URLs  
- Missing company names  
- Duplicate records  
- Invalid URLs  
- Missing product details  

✅ The visualization highlights clear improvements across multiple quality dimensions, demonstrating the impact of the cleaning process.  

---

## 🔍 Key Insights  
- Significant reduction in missing and invalid values  
- Duplicate records successfully identified and removed  
- Consistent formatting across all key fields  
- Cleaned dataset ready for advanced analytics and reporting  

---

## ✅ Conclusion  
This assessment successfully showcases an **end-to-end data quality improvement workflow** using:  
- **SQL** for data structuring  
- **Python** for cleaning and automation  
- **Tableau** for data visualization  

As a result, the **news events** dataset is now cleaner, more consistent, and reliable for downstream analysis and reporting.  
