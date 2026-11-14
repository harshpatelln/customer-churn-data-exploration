# Customer Insight AI – Week 1: Project Planning and Setup

**AI-Powered Customer Segmentation and Churn Prediction System**



## 1. Problem statement
Businesses lose revenue when customers leave, and it is much cheaper to keep an existing customer than to win a new one. Most small businesses do not have a simple tool to group customers by behaviour or to find who is likely to leave. This project builds a system that **segments customers** into meaningful groups and **predicts churn**, so that retention actions can be targeted.

## 2. Objectives
- Group customers into behaviour-based segments using K-means clustering
- Predict which customers are likely to churn using supervised machine learning
- Compare models and choose the best one using proper evaluation metrics
- Present insights and predictions in an easy-to-use Streamlit dashboard
- Suggest retention actions for each customer segment

## 3. Planned modules
| # | Module | Purpose |
|---|--------|---------|
| 1 | Data upload and validation | Accept a CSV file and check that it is usable |
| 2 | Preprocessing | Handle missing values, encode categories, scale features |
| 3 | Customer segmentation | K-means clustering to find customer groups |
| 4 | Churn prediction | Logistic Regression, Decision Tree and Random Forest |
| 5 | Model evaluation | Accuracy, precision, recall, F1, ROC-AUC, confusion matrix |
| 6 | Behaviour insights | Explain what drives churn and what defines each segment |
| 7 | Dashboard and retention support | Streamlit app showing results and suggested actions |

## 4. Technology stack
- **Language:** Python
- **Data handling:** Pandas, NumPy
- **Machine learning:** Scikit-learn
- **Visualisation:** Matplotlib, Seaborn, Plotly
- **Dashboard:** Streamlit
- **Version control:** Git and GitHub
- **Environment:** Jupyter Notebook

## 5. Dataset
Bank Customer Churn dataset from Kaggle, with the target column `Exited` (1 = customer left, 0 = customer stayed). Detailed acquisition, cleaning and analysis are covered in Week 2.

## 6. Planned workflow
```
Data upload -> Preprocessing -> Segmentation (K-means)
                             -> Churn prediction (ML models)
                             -> Evaluation -> Insights -> Streamlit dashboard
```

## 7. Week 1 outcomes
- Project idea, problem statement and objectives defined
- Project synopsis prepared and module plan finalised
- Technology stack selected and development environment set up
- GitHub repository created for the project

## 8. Project structure (planned)
```
.
├── data/            # datasets
├── notebooks/       # Jupyter notebooks
├── app.py           # Streamlit dashboard
├── README.md
└── requirements.txt
```

## 9. Setup
```bash
pip install pandas numpy scikit-learn matplotlib seaborn plotly streamlit jupyter
```

## 10. Next steps
Week 2: data acquisition, cleaning and preliminary exploratory data analysis. After that: segmentation, churn prediction models and the dashboard.
