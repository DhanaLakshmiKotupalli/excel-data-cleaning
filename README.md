#  Excel Data Cleaning Project – Raw Dataset Preparation (Excel & Python)

##  Project Overview

This project focuses on cleaning and preparing a raw dataset containing missing values, duplicates, and inconsistent formats. It was completed as part of a data analytics learning task using both **Excel** and **Python (pandas)**.

The original dataset was selected from Kaggle (e.g., Customer Personality Analysis / Sales Data), and the cleaning was performed using:
- Microsoft Excel (manual cleaning with formulas and filters)
- Python (pandas library)

---

##  Tools Used
- Microsoft Excel
- Python 3 (Jupyter Notebook / VSCode)
- pandas library

---

## Tasks Performed

### Excel Data Cleaning
- Used filters and conditional formatting to find missing values
- Replaced or removed nulls using `IF()` and `ISBLANK()`
- Removed duplicate records using "Remove Duplicates"
- Standardized text entries (e.g., gender, category names)
- Cleaned up special characters like ₹ and % in numeric columns
- Formatted dates to `dd-mm-yyyy`
- Renamed columns (e.g., `Product ID` → `product_id`)

### Python (pandas) Data Cleaning
- Checked for missing values with `.isnull().sum()`
- Removed nulls and duplicates using `.dropna()` and `.drop_duplicates()`
- Converted columns like `price`, `discount`, `rating` to numeric
- Standardized text values using `.str.lower()` and `.strip()`
- Cleaned special symbols using regex
- Fixed inconsistent date formats with `pd.to_datetime()`
- Renamed columns to snake_case using `.rename(columns={...})`
- Saved the final cleaned dataset as `amazon_cleaned_pandas.csv`

---

## 🗃️ Datasets Used

- 📄 `raw_data.csv` – Original raw dataset
- 📄 `cleaned_data.csv` – Cleaned version using Excel
- 📄 `cleaned_data_pandas.csv` – Cleaned version using Python

---

## Summary of Changes

| Task                        | Excel                 | Python (pandas)        |
|-----------------------------|------------------------|--------------------------|
| Null handling              | ISBLANK, Filter       | `df.isnull().sum()`, `df.dropna()` |
| Duplicate removal          | Remove Duplicates     | `df.drop_duplicates()`  |
| Text standardization       | Manual Replace, TRIM  | `str.lower()`, `str.strip()` |
| Special symbols (₹, %)     | Find & Replace         | Regex with `str.replace()` |
| Date format correction     | Format Cells → Date   | `pd.to_datetime()`      |
| Column renaming            | Manual Rename          | `df.rename()` with dict |

---

## 🙌 Final Output

The final cleaned datasets are ready for analysis, dashboard creation, or visualization tasks. You can use them for Power BI, Tableau, or Python-based analysis.

---

## 📌 Learnings & Skills Applied

- Real-world data cleaning techniques
- Excel formulas: `IF`, `ISBLANK`, formatting, filters
- Python functions: `.isnull()`, `.drop_duplicates()`, `.str.replace()`, regex
- Consistency checks and standardization

---

## 📁 How to Run the Python Code

1. Clone the repository
2. Navigate to the `python-data-cleaning/code/` directory
3. Run the `data_cleaning.py` script in your IDE or terminal

```bash
python data_cleaning.py

