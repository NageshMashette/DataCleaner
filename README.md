# dataCleaner

[![PyPI version](https://badge.fury.io/py/dataCleaner.svg)](https://badge.fury.io/py/dataCleaner)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

**dataCleaner** is a Python package designed to help data scientists clean and preprocess datasets effectively before feeding them into machine learning models. The package provides a comprehensive suite of tools for handling missing data, removing duplicate rows, normalizing numerical columns, and removing outliers.

---

## **Features**

- **Handle Missing Data**: Automatically handle missing values using mean, median, or by dropping rows.
- **Drop Duplicate Rows**: Identify and remove duplicate rows in your dataset.
- **Normalize Numerical Columns**: Scale numerical columns to a range of 0 to 1 using Min-Max normalization.
- **Remove Outliers**: Remove outliers using Z-score or IQR (Interquartile Range) methods.
- **Get Cleaned Data**: Retrieve the cleaned DataFrame after applying the cleaning methods.

---

## **Installation**

Install the package from PyPI using pip:

```bash
pip install datacleaners==0.4.0
from datacleaners import DataCleaner
cleaner = DataCleaner(df)
cleaner.handle_missing_data()
cleaner.drop_duplicates()
cleaner.normalize_columns()
print(cleaner.get_cleaned_data())
