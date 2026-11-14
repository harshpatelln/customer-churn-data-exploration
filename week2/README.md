# Customer Insight AI – Week 2: Data Acquisition and Preliminary Analysis

Part of the **AI-Powered Customer Segmentation and Churn Prediction System** project.
This week covers acquiring a public dataset, cleaning it with Python, and running a preliminary exploratory data analysis (EDA).

## Dataset
- **Bank Customer Churn Modelling** (`Churn_Modelling.csv`) from Kaggle
- 10,000 customers, 14 columns, target column `Exited` (1 = churned)
- Download: https://www.kaggle.com/datasets/shrutimechlearn/churn-modelling
- The raw file is **not edited**; place it in `data/raw/`

## Project structure
```
.
├── data/
│   ├── raw/            # original Churn_Modelling.csv (download it here)
│   └── processed/      # bank_churn_clean.csv (created by the script)
├── figures/            # EDA plots (created by the script)
├── week2_analysis.py   # acquisition, cleaning and EDA
├── Week2_Report.docx   # full written report
└── README.md
```

## How to run
```bash
pip install pandas numpy matplotlib seaborn
python week2_analysis.py
```

## What the script does
1. **Acquisition** – loads the raw CSV and inspects shape, types and first rows
2. **Cleaning** – checks missing values and duplicates, drops identifier columns, standardises text, checks ranges, flags outliers (IQR), fixes data types, saves the cleaned file
3. **EDA** – descriptive statistics, churn rate by Geography / Gender / NumOfProducts / IsActiveMember, and six plots (class balance, histograms, box plot, scatter plot, churn by category, correlation heatmap)

## Key findings
- About 20% of customers churn (imbalanced target)
- Churn is higher in Germany, among older customers, among inactive members and among customers with only one product or three or more products

## Next steps
Customer segmentation with K-means, churn prediction models (Logistic Regression, Decision Tree, Random Forest) and a Streamlit dashboard.
