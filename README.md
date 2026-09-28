# used-car-dataset-eda
Exploratory Data Analysis (EDA) on a used car dataset, including data cleaning, duplicate checking, numerical analysis, outlier detection, and data quality assessment.

# Used Car Dataset – EDA

Exploratory Data Analysis (EDA) of a used car dataset using Python and Pandas.

## About the Project

This project focuses on understanding and cleaning a used car dataset through basic Exploratory Data Analysis techniques.

**Student:** Gautami Balaso Kamble
**Batch:** September Batch 1
**Dataset Source:** Kaggle

## Objectives

* Understand the structure of the used car dataset
* Check and handle duplicate values
* Select and analyze numerical columns
* Check data quality
* Identify potential outliers
* Understand relationships between different car attributes

## EDA Process

### 1. Duplicate Checking

The dataset was checked for duplicate records using:

```python
df.duplicated().sum()
```

Duplicate records were removed using the `drop` method and the dataset was checked again.

### 2. Numerical Column Selection

Numerical columns were selected using:

```python
numeric_cols = df.select_dtypes(include="number")
print(numeric_cols)
```

### 3. Data Quality

The analysis included:

* Missing-value checking
* Duplicate-value checking
* Outlier identification
* Data-type checking

The presentation reports **0 missing values** in the analyzed columns. Outliers were identified using the **99th percentile method**.

### 4. Outlier Handling

The identified outliers were not automatically removed because they may represent actual high-priced or high-mileage vehicles and could contain useful information.

## Files

* 📊 **Dataset:** [Used Car Dataset](./used_car_dataset.csv)
* 📓 **Google Colab Notebook:** [EDA Notebook](./used_car_eda.ipynb)
* 📄 **Project Presentation:** [Used Car EDA Analysis](./used-car-eda-analysis.pdf)
by gautami k
