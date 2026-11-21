# Retail Store Sales Forecasting

A structured, end-to-end machine learning project to forecast daily retail sales across Rossmann stores. The project focuses on disciplined data preprocessing, feature engineering from temporal and operational store data, and comparing linear vs. tree-based regression models.

---

## Project Overview

- **Dataset:** Rossmann Store Sales (historical daily sales across 1,115 stores)
- **Target Variable:** `Sales` (daily store revenue)
- **Problem Type:** Supervised Regression
- **Core Models:** 
  - **Linear Regression** — baseline linear model evaluating direct feature relationships
  - **Decision Tree Regressor** — non-linear model capturing store interactions, promotions, and seasonality thresholds

---

## Project Workflow
Raw Data ─► 01 EDA ─► 02 Cleaning & Features ─► 03 Missing Values ─► 04 Outliers ─► Preprocessing ─► ML Modeling

1. **`01 - Data Exploration.ipynb`**  
   Exploratory data analysis covering sales distributions, customer behavior, store types, assortments, and promotions.
2. **`02 - Data Cleaning & Feature Engineering.ipynb`**  
   Drops closed store days and invalid records; engineers calendar features (`Quarter`, `IsWeekend`, `IsMonthStart`, `IsMonthEnd`) and calculates competition/promotion duration metrics (`CompetitionOpenMonths`, `Promo2OpenWeeks`).
3. **`03 - Missing Values Handling.ipynb`**  
   Domain-specific imputation: median for skewed numericals (`CompetitionDistance`, `CompetitionOpenMonths`), mode for competitor dates, and explicit zero/None values for non-Promo2 stores.
4. **`04 - Outliers Handling.ipynb`** *(upcoming)*  
   Detection and treatment of anomalies in customer traffic and sales.
5. **Preprocessing & Machine Learning**  
   Final column transformations, train/test splitting, fitting Linear Regression and Decision Tree models, and comparing performance using RMSE and MAE.

---

## Repository Structure
Retail-Store-Sales-Forecasting/ ├── code/ │ ├── 01 - Data Exploration.ipynb │ ├── 02 - Data Cleaning & Feature Engineering.ipynb │ ├── 03 - Missing Values Handling.ipynb │ └── ... ├── data/ │ └── train_no_missing.csv # Latest processed dataset (tracked with Git LFS) ├── README.md └── .gitignore

---

## Tech Stack

- **Python** (Pandas, NumPy)
- **Machine Learning:** Scikit-learn
- **Visualization:** Matplotlib, Seaborn
- **Data Versioning:** Git LFS
