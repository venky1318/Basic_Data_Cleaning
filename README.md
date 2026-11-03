# Task 25 — Basic Data Cleaning Using Pandas

## Project Overview

This project demonstrates a complete basic data-cleaning workflow using Python and Pandas.

A student performance dataset is used to identify and remove duplicate records, handle missing values, and correct inappropriate data types.

The objective is to improve data quality and prepare the dataset for further analysis and machine-learning applications.

## Objectives

- Inspect the original dataset.
- Identify and remove duplicate records.
- Detect missing values.
- Handle missing numerical and categorical values.
- Convert columns into appropriate data types.
- Compare original and cleaned datasets.
- Export the cleaned dataset and cleaning summary.

## Technologies Used

- Python
- Pandas
- NumPy
- Google Colab
- Jupyter Notebook

## Dataset Description

The project uses a manually created student performance dataset.

The original dataset contains 12 records and seven columns:

- student_id
- student_name
- department
- age
- marks
- attendance
- joining_date

The dataset intentionally includes two duplicate records, missing values, and an incorrectly formatted age entry.

All student records are fictional.

## Data Cleaning Operations

### 1. Duplicate Removal

- Identified duplicates using `duplicated()`.
- Removed repeated records using `drop_duplicates()`.
- Compared record counts before and after removal.

### 2. Missing-Value Handling

- Identified missing values using `isnull()`.
- Replaced invalid numerical values with missing values during type conversion.
- Used median imputation for numerical columns.
- Replaced the missing department with `Unknown`.

### 3. Data-Type Correction

- Converted age into integer format.
- Converted marks into integer format.
- Converted attendance into integer format.
- Converted department into a categorical type.
- Converted joining_date into datetime format.
- Retained student IDs and names as strings.

## Cleaning Results

| Metric | Result |
|---|---:|
| Original records | 12 |
| Duplicate records removed | 2 |
| Records after duplicate removal | 10 |
| Missing cells after type correction | 4 |
| Missing cells after treatment | 0 |
| Remaining duplicate records | 0 |
| Final cleaned records | 10 |

## Project Files

- `Task_25_Basic_Data_Cleaning.ipynb` — Complete Colab notebook.
- `student_data_raw.csv` — Original dataset.
- `student_data_cleaned.csv` — Final cleaned dataset.
- `duplicate_records.csv` — Duplicate-related records.
- `cleaning_summary.csv` — Before-and-after cleaning summary.
- `requirements.txt` — Required Python libraries.
- `README.md` — Project documentation.
- `project_report.pdf` — Formal project report.
- `screenshots/` — Actual execution evidence.

## Key Learning Outcomes

- Identifying duplicate records.
- Handling missing values.
- Converting incorrect data types.
- Using Pandas for structured data cleaning.
- Comparing dataset quality before and after cleaning.
- Preparing data for further analysis.

## Conclusion

This project demonstrates how multiple fundamental data-cleaning techniques can be combined into one workflow. The final dataset contains 10 records with no missing values or exact duplicate rows and with appropriately converted data types.
