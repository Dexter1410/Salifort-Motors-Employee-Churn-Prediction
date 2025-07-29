# **Salifort Motors Employee Churn Prediction and Employee Retention Strategies**
---

## 🔍 Problem Statement

**Business Question:**  
> What factors are most likely to cause an employee to leave Salifort Motors?

The project was commissioned to analyze historical employee data to build a predictive model that classifies employees as likely to stay or leave, based on a variety of factors including performance, workload, salary, tenure, and more.

---

## 🧾 Dataset Overview

- **File**: [`HR_capstone_dataset.csv`](./HR_capstone_dataset.csv)
- **Target Variable**: `left` (binary: 1 if the employee left the company, 0 otherwise)
- **Key Features**:
  - `last_evaluation`
  - `number_project`
  - `tenure`
  - `overworked` (e.g., avg monthly hours)
  - `salary` level (`low`, `medium`, `high`)
  - `work_accident`
  - `promotion_last_5years`
  - and other HR attributes

---

## 🧪 Methodology (see [`Salifort-Project-Notebook.ipynb`](./Salifort-Project-Notebook.ipynb))

### 1. **Exploratory Data Analysis (EDA)**
- Univariate and bivariate analysis
- Distribution plots for numeric features
- Countplots for categorical variables
- Correlation heatmaps

### 2. **Data Preprocessing**
- Label encoding for categorical variables
- Handling of imbalanced data
- Feature transformation and scaling

### 3. **Modeling Techniques**
Models were trained to predict the binary target `left`:

- **Logistic Regression** (baseline model)
- **Decision Tree Classifier**
- **Random Forest Classifier** (two variations with different hyperparameters)

### 4. **Model Evaluation**
- Accuracy, Precision, Recall, and F1-score
- Confusion Matrix
- Feature Importance (especially for tree-based models)

---

## ✅ Key Insights

(From [`Salifort-Employee-Retention-Executive-Summary.pdf`](./Salifort-Employee-Retention-Executive-Summary.pdf))

- **Top Predictive Features**:
  - `last_evaluation`
  - `number_project`
  - `tenure`
  - `overworked`
  - `salary_low`
  - `work_accident`

- **Best Model**: Random Forest (outperformed other classifiers)

- **Recommendations for HR**:
  - Cap the number of simultaneous projects.
  - Reward or promote long-tenured employees (especially 4+ years).
  - Address overworking concerns and clarify overtime policies.
  - Use proportionate evaluation methods tied to hours worked.

---

## 📌 Milestones (as per [`Project Proposal`](./Salifort-Employee-Retention-Project-Proposal.pdf))

| Stage     | Task                                                   |
|-----------|--------------------------------------------------------|
| 🟩 Plan    | Understand business problem and define goals          |
| 🟨 Analyze | Perform EDA, prepare data, select model               |
| 🟧 Construct | Train and evaluate models                           |
| 🟥 Execute | Share results and provide HR recommendations          |

---

## 📎 Future Enhancements

- Add employee satisfaction survey data for deeper insights.
- Deploy model via Streamlit or Flask for HR team usage.
- Use SHAP or LIME for model explainability.
- Automate retraining with updated data every quarter.

---

## 👨‍💻 Author

**Shubham Thakur**  
MBA - Business Analytics | Ex-Drone Engineer | Data & Strategy Enthusiast  
📫 [LinkedIn](#) | [GitHub](#) | [Email](#)

---

## 📚 References

- Project Proposal: [`Salifort-Employee-Retention-Project-Proposal.pdf`](./Project-Proposal/Salifort-Employee-Retention-Project-Proposal.pdf)  
- Executive Summary: [`Salifort-Employee-Retention-Executive-Summary.pdf`](./Executive-Summary/Salifort-Employee-Retention-Executive-Summary.pdf)
- Dataset: [`HR_capstone_dataset.csv`](./Raw-Dataset/HR_capstone_dataset.csv)  
- Notebook: [`Salifort-Project-Notebook.ipynb`](./Salifort-Project-Notebook.ipynb)
- Random Forest Models: ['hr_rf1.pickle and hr_rf2.pickle'](./models)

---

> *This project was completed as part of a capstone requirement and serves as a demonstration of practical business analytics using Python.*


