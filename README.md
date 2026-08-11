# 📊 Food Delivery Sales Performance & Operations Analysis (MS Excel)

## 📌 Executive Summary
An end-to-end Data Analytics project executed in **Microsoft Excel** analyzing over **15,000+ raw order records** from a multi-city food delivery aggregator. The project spans raw data ingestion, comprehensive multi-stage data cleaning, automated pivot aggregations, data quality summaries, and an interactive Executive Dashboard.

---

## 🛠️ Project Architecture & Workflow

The analysis is structured across **12 specialized spreadsheet modules**:

1. **`01_RAW_DATA`**: Unprocessed backend dump (15,300 records).
2. **`02_DUPLICATE_CHECK`**: Deduplication layer using Excel data tools.
3. **`03_MISSING_RATINGS`**: Null-value imputation for missing customer ratings.
4. **`04_STANDARDIZATION`**: Text standardization via `=PROPER()` functions.
5. **`05_ANOMALY_DETECTION`**: Outlier filtering for invalid financial entries.
6. **`06_CLEANED_DATA`**: Production-ready dataset (14,781 records).
7. **`07_DATA_QUALITY_SUMMARY`**: Audit trail summarizing records processed vs purged.
8. **`08_REVENUE_PIVOT`**: Restaurant revenue aggregation and ranking.
9. **`09_PAYMENT_PIVOT`**: Order distribution across payment channels.
10. **`10_DELIVERY_PIVOT`**: Category-wise average delivery latency analysis.
11. **`11_DASHBOARD`**: Executive KPI Dashboard & operational insights.
12. **`12_PROJECT_README`**: Internal project documentation.

---

## 🧹 Data Cleaning & Quality Audit Summary

| Metric / Check | Issues Found | Action Taken | Final Status |
| :--- | :--- | :--- | :--- |
| **Total Raw Records** | 15,300 | Ingested baseline backend data | 15,300 Rows |
| **Duplicate Rows** | 300 | Removed completely duplicate entries | 300 Rows Removed |
| **Missing Ratings** | 1,588 | Imputed blank `Customer_Rating` cells with `0` | 1,588 Cells Updated |
| **Text Inconsistency** | Mixed casing | Applied `=PROPER()` to `Restaurant_Name` & `Payment_Mode` | 100% Standardized |
| **Numeric Anomalies** | 219 | Purged rows where `Order_Value_INR` < 0 or > ₹10,000 | 219 Rows Purged |
| **Final Clean Dataset** | — | **Production-Ready Dataset** | **14,781 Rows** |

---

## 📈 Key Business Insights

* **🏆 Top Revenue Driver:** **Maa Veg Kabab** led all partner restaurants, generating **₹3,73,868** in total order value over H1 2026.
* **💳 Payment Preferences:** **UPI** emerged as the most preferred payment method (**3,004 orders**), closely followed by **Cash On Delivery (2,905 orders)**.
* **⏱️ Delivery Speed Bottleneck:** The **Indo-Chinese** category recorded the highest average delivery latency (**40.07 mins**), highlighting a potential operational bottleneck in kitchen preparation or dispatch.

---

## 💻 Technical Skills Demonstrated
* **Data Cleansing:** Handling missing values, deduplication, text casing normalization, and financial outlier filtering.
* **Excel Formulas:** `=PROPER()`, `=SUM()`, `=AVERAGE()`, `=COUNTIF()`, and Logical Conditioning.
* **Data Visualization & Reporting:** Pivot Tables, Data Summarization, and Dashboard Layout Design.
