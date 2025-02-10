# DHL2-Task01-Employee-Attrition-Prediction

## Overview
This project aims to predict employee attrition using the IBM HR Analytics dataset. The goal is to build a classification model that can identify employees likely to leave the company and provide actionable insights for retention strategies. The model achieves an accuracy of **79%** using a Random Forest classifier.

## Dataset
The dataset used is the **IBM HR Analytics Employee Attrition & Performance** dataset, which contains 1,470 rows and 35 columns. Key features include:
- `Age`
- `MonthlyIncome`
- `JobSatisfaction`
- `WorkLifeBalance`
- `Attrition` (Target Variable)

Dataset Source: [Kaggle](https://www.kaggle.com/pavansubhasht/ibm-hr-analytics-attrition-dataset)

## Project Structure
employee-attrition-prediction/
├── data/
│ └── WA_Fn-UseC_-HR-Employee-Attrition.csv
├── notebooks/
│ └── Employee_Attrition_Prediction.ipynb
├── README.md
└── requirements.txt

## Key Steps
1. **Exploratory Data Analysis (EDA)**:
   - Analyzed key factors influencing attrition.
   - Visualized feature distributions and correlations.

2. **Data Preprocessing**:
   - Handled missing values.
   - Encoded categorical variables.
   - Scaled numerical features.

3. **Model Building**:
   - Trained a Random Forest classifier.
   - Achieved **79% accuracy** on the test set.

4. **Model Interpretation**:
   - Used SHAP (SHapley Additive exPlanations) to explain model predictions.
   - Identified top features influencing attrition.

5. **Actionable Insights**:
   - Provided recommendations to reduce employee attrition.

## Results
- **Accuracy**: 79%
- **Top Features Influencing Attrition**:
  1. `MonthlyIncome`
  2. `Age`
  3. `JobSatisfaction`
  4. `WorkLifeBalance`
  5. `YearsAtCompany`

## Usage
### Prerequisites
- Python 3.8+
- Required libraries: `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`, `shap`

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/employee-attrition-prediction.git
   cd employee-attrition-prediction
### 1. Install dependencies:

pip install -r requirements.txt

### 2. Run the Jupyter Notebook:

jupyter notebook notebooks/Employee_Attrition_Prediction.ipynb

### Steps to Reproduce
Load the dataset (**WA_Fn-UseC_-HR-Employee-Attrition.csv**).

1. Perform EDA to understand the data.
2. Preprocess the data (encoding, scaling).
3. Train the Random Forest model.
4. Evaluate the model using accuracy and SHAP values.

### **Generate actionable insights.**
### Actionable Insights
Based on the analysis, the following strategies are recommended to reduce employee attrition:
Improve Job Satisfaction: Regular feedback sessions and career development programs.
Enhance Work-Life Balance: Flexible work hours and remote work options.
Review Compensation: Ensure competitive salaries, especially for high-performing employees.
Focus on Long-Tenure Employees: Provide growth opportunities for employees with many years at the company.

---

### **How to Use This README**
1. Replace placeholders like `your-username`, `your-email@example.com`, and image paths with your actual details.
2. Add the dataset (`WA_Fn-UseC_-HR-Employee-Attrition.csv`) to the `data/` folder.
3. Save the Jupyter Notebook in the `notebooks/` folder.
4. Update the `requirements.txt` file with the necessary libraries.

### **Example `requirements.txt`**
```plaintext
pandas==1.5.3
numpy==1.23.5
scikit-learn==1.2.0
matplotlib==3.6.2
seaborn==0.12.1
shap==0.41.0
jupyter==1.0.0
