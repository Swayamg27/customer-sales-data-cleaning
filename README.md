# 🧹 E-Commerce Sales Data Cleaning Project

## 📌 Project Overview
This project involves cleaning a real-world messy e-commerce sales dataset sourced from Kaggle.
The dataset contained multiple data quality issues including duplicates, missing values, invalid entries,
inconsistent formatting, and incorrect calculations. The goal was to transform raw, unusable data into
a clean, analysis-ready dataset.

---

## 🛠️ Tools Used
- **Microsoft Excel** — final cleaned output and presentation
- **Python (Pandas)** — data analysis and cleaning logic
- **openpyxl** — Excel file generation with formatting

---

## 📁 Files in This Repository

| File | Description |
|---|---|
| `messy_ecommerce_sales_data.csv` | Original raw dataset from Kaggle (untouched) |
| `Ecommerce_Data_Cleaning_Project.xlsx` | Final Excel workbook with 4 sheets (see below) |
| `README.md` | Project documentation |

### Excel Workbook Sheets
| Sheet | Description |
|---|---|
| `Raw_Data` | Original messy data for comparison |
| `Cleaned_Data` | Fully cleaned and formatted dataset |
| `Cleaning_Log` | Documents every issue found and action taken |
| `Summary` | Project stats and key business insights |

---

## 🔍 Issues Found & Fixed

| # | Issue Type | Count | Action Taken |
|---|---|---|---|
| 1 | Column name spaces | 2 | Stripped leading spaces from column headers |
| 2 | Duplicate rows | 1 | Removed, kept first occurrence |
| 3 | Inconsistent Category casing | 8 | Standardized (electronic → Electronics, etc.) |
| 4 | Missing Category values | 8 | Filled with 'Unknown' |
| 5 | Invalid Price values | 6 | Fixed parseable values ('300$', 'four hundred'); rest filled with median |
| 6 | Missing Price values | 5 | Filled with median price |
| 7 | Alphanumeric Quantity ('4a') | 1 | Stripped letters, converted to numeric |
| 8 | Negative Quantity (-2, -5) | 2 | Converted to absolute values |
| 9 | Missing Quantity | 5 | Filled with 1 (minimum order assumption) |
| 10 | Mixed/Invalid Date formats | 2 | Standardized all to YYYY-MM-DD |
| 11 | Missing/Incorrect Total | 14 | Recalculated as Quantity × Price |

**Total Issues Resolved: 56**

---

## 📊 Dataset Before vs After

| Metric | Before | After |
|---|---|---|
| Rows | 103 | 102 |
| Null values | 32+ | 0 |
| Invalid entries | 10+ | 0 |
| Consistent formatting | ❌ | ✅ |
| Accurate Totals | ❌ | ✅ |

---

## 💡 Key Insights (Post-Cleaning)
- **Books** is the top product category by order volume
- **PayPal** is the most commonly used payment method
- All Total values are now accurately calculated as `Quantity × Price`
- Dataset is now ready for dashboarding or further analysis

---

## 🚀 How to Use
1. Download `Ecommerce_Data_Cleaning_Project.xlsx`
2. Open in Microsoft Excel
3. Review `Raw_Data` tab to see original issues
4. Compare with `Cleaned_Data` tab
5. See `Cleaning_Log` for full documentation of changes

---

## 👤 Author
**[Swayam Gupta]**  
Aspiring Data Analyst | [https://www.linkedin.com/in/swayam-gupta-2a7174251/] | [swayamg27@gmail.com]
