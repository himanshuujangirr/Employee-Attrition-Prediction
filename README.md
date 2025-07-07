# Employee Attrition Analysis & Prediction

## Project Overview

This project is built to analyze employee attrition behavior and predict which employees are likely to leave the organization. The aim is to help HR and leadership teams take proactive steps to improve retention. The analysis is based on a real-world HR dataset and includes both deep exploratory insights and predictive machine learning modeling.

The notebook contains two major sections:

1. **Exploratory Data Analysis (EDA)** — to understand key drivers of attrition.
2. **Machine Learning Modeling** — to build and evaluate classification models.

---

## Dataset Used

- **Source**: IBM HR Analytics Employee Attrition dataset
- **Format**: Excel file — `WA_Fn-UseC_-HR-Employee-Attrition.xlsx`
- **Records**: 1,470 employees
- **Target Variable**: `Attrition` (Yes/No)

---

## Exploratory Data Analysis (EDA)

A thorough exploratory analysis was conducted to understand the distribution of attrition across various factors:

### Key Areas Analyzed:

- **Department-wise attrition** — R&D had the highest attrition despite being the largest department.
- **Business Travel** — Frequent travelers showed higher attrition.
- **Work-Life Balance & Job Satisfaction** — Poor scores in these led to increased attrition.
- **Years Since Last Promotion** — Long gaps between promotions correlated with employee exits.
- **Distance From Home** — Employees with long commutes were more likely to leave.
- **Income Analysis** — Violin plots and scatterplots were used to analyze salary vs. other variables.
- **Outlier Detection** — Using z-score and IQR, with reasoning whether outliers are valid.

The goal was not just to visualize, but to extract **actionable insights** that can support HR decisions.

---

## Business Impact of EDA

- Identified high-risk segments such as frequent travelers and employees with long tenure but no promotion.
- Highlighted the influence of low work-life balance and poor satisfaction scores.
- Demonstrated that attrition is not random — it follows certain behavioral and structural patterns.
- These findings can help design retention strategies targeted at the right employee groups.

---

## Machine Learning Models Used

The following models were implemented and compared for predicting attrition:

- Logistic Regression
- Random Forest Classifier
- XGBoost Classifier

### Additional Techniques:

- **SMOTE (Synthetic Minority Over-sampling Technique)**: Used to handle class imbalance in the target variable.
- **Feature Scaling**: StandardScaler used for numerical features.
- **Label Encoding & One-Hot Encoding**: For categorical preprocessing.
- **Feature Selection**: Heatmaps and domain logic used to remove redundant columns.

---

## Model Evaluation Metrics

Each model was evaluated on:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

The results were compared to understand which model performs better under both balanced and imbalanced data.

> ✅ All comparison outputs are shown clearly inside the notebook using classification reports.

---

## Technical Stack

- Python
- NumPy, Pandas
- Matplotlib, Seaborn
- scikit-learn
- XGBoost
- imbalanced-learn

---

## File Structure

```bash
├── attrition_analysis_model.ipynb    # Main notebook with EDA and model training
├── WA_Fn-UseC_-HR-Employee-Attrition.xlsx    # Dataset file
├── requirements.txt                  # Python dependencies
```

How to Run
Clone the repository

Install dependencies
pip install -r requirements.txt


Open the Jupyter Notebook
jupyter notebook main.ipynb


Final Note
This project is designed not only to showcase technical skills in data cleaning and modeling, but also to demonstrate real-world business problem solving. The EDA provides insights HR teams can act on, while the predictive models offer a foundation for building early warning systems for attrition.

If you're reviewing this for a Business/Data Analyst role, I encourage you to look at the EDA section — it's built to extract practical meaning from data, not just graphs.




