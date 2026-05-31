# 🔍 BCG X Data Science – Customer Churn Prediction

> **BCG X (Boston Consulting Group) | Forage Virtual Experience Program**
> `June 2025 – July 2025` · Certificate issued July 2, 2025

---

## 📌 Overview

This project simulates the work of a **Data Scientist at BCG X**, BCG's tech build and design unit. The client, **PowerCo** — a major utility provider serving SMEs — was experiencing above-average customer churn in a highly competitive energy market.

The goal: **identify the key drivers of churn and build a predictive model** to flag at-risk customers before they leave.

---

## 🧩 Business Problem

PowerCo was losing customers at an accelerating rate due to:
- Increased competition from new energy providers
- Flexible pricing models offering customers more choice
- A market shift toward renewable energy alternatives

Without a predictive solution, PowerCo was only identifying churners **after they had already left** — missing critical intervention windows.

---

## 🗂️ Project Structure

```
bcg-x-churn-prediction/
│
├── notebooks/
│   ├── Task_2_EDA_Part1.ipynb          # Exploratory Data Analysis – Part 1
│   ├── Task_2_EDA_Part2.ipynb          # Exploratory Data Analysis – Part 2
│   ├── Task_3_Feature_Engineering.ipynb # Feature Engineering
│   ├── Task_4_Modeling.ipynb            # Random Forest Model & Evaluation
│   └── PowerCo_EDA_Analysis.ipynb       # Full EDA walkthrough (custom)
│
├── data/
│   └── price_data.csv                   # Energy pricing data by period
│
├── executive_summary/
│   └── Executive_Summary.pdf            # 1-page BCG-style executive brief
│
├── certificate/
│   └── BCG_X_Certificate.pdf            # Forage completion certificate
│
└── README.md
```

---

## 🔬 Methodology

Following BCG X's 5-step data science framework:

| Step | Task | Description |
|------|------|-------------|
| 1 | **Business Framing** | Understood PowerCo's churn problem and defined the analytical objective |
| 2 | **EDA & Data Cleaning** | Explored 14,600+ customer records; analyzed distributions, missing values, and correlations |
| 3 | **Feature Engineering** | Engineered pricing sensitivity features, consumption patterns, and tenure-based signals |
| 4 | **Modeling & Evaluation** | Built and evaluated a Random Forest classifier (1,000 trees) |
| 5 | **Insights & Recommendations** | Delivered a strategic 1-page executive summary with actionable recommendations |

---

## 📊 Dataset

Two primary datasets were used:

**`client_data.csv`** — 14,600+ customer records including:
- Energy consumption (12-month, last month, forecasted)
- Contract details (activation date, renewal date, end date)
- Financial metrics (net margin, gross margin, power subscription)
- Churn label (binary: churned in next 3 months)

**`price_data.csv`** — Time-series pricing data including:
- Off-peak, peak, and mid-peak variable/fixed energy prices
- Per-period pricing breakdown by customer ID

---

## 🤖 Model Results

| Metric | Score |
|--------|-------|
| **Accuracy** | 90.3% |
| **Precision** | 77.3% |
| **Recall** | 4.6% |
| **Model** | Random Forest (1,000 estimators) |
| **High-Risk Customers Flagged** | 0.6% of customer base |

**Key finding:** The model achieves high precision — when it flags a churner, it's right ~77% of the time — enabling PowerCo to target interventions efficiently. The low recall reflects a class imbalance challenge, which was addressed in the executive summary with recommendations for threshold tuning and resampling.

---

## 💡 Key Insights & Recommendations

- **Price sensitivity** was identified as a primary driver of churn — customers on inflexible or higher-priced contracts churned at higher rates
- **Tenure** was inversely correlated with churn — newer customers were significantly more likely to leave
- Recommended: **proactive discount targeting** for flagged high-risk customers during the renewal window
- Recommended: **threshold tuning and SMOTE resampling** to improve recall without sacrificing precision
- Recommended: **integrating the model into CRM/customer success workflows** for real-time churn scoring

---

## 🛠️ Tech Stack

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=flat&logo=scikit-learn&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-4C72B0?style=flat)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=flat)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat&logo=jupyter&logoColor=white)

- **Languages:** Python
- **Libraries:** Pandas, NumPy, Scikit-learn, Seaborn, Matplotlib
- **Model:** Random Forest Classifier
- **Tools:** Jupyter Notebook, Excel (supporting analysis)

---
## 🚀 How to Run

```bash
# Clone the repository
git clone https://github.com/sayemkhandaker17/bcg-x-churn-prediction.git

# Install dependencies
pip install pandas numpy scikit-learn seaborn matplotlib jupyter

# Launch notebooks
jupyter notebook
```

Open the notebooks in order (Task 2 → Task 3 → Task 4) to follow the full project workflow.

---

## 📁 About BCG X

BCG X is the tech build and design unit of Boston Consulting Group, combining management consulting expertise with data science, engineering, and product capabilities to deliver high-impact digital solutions for major organizations worldwide.

---

*This project was completed as part of the BCG X Data Science Virtual Experience Program on Forage. All data used is simulated for educational purposes.*
