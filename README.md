
# Employee Attrition Prediction & Explainable HR Analytics
# Employee Attrition Prediction & Explainable HR Analytics

## Overview
An end-to-end Machine Learning project that predicts employee attrition and identifies the key factors influencing employee turnover. The project includes data exploration, preprocessing, handling class imbalance, model training, evaluation, and explainability.

## Objectives
- Analyze employee data through Exploratory Data Analysis (EDA).
- Clean and preprocess employee data.
- Handle class imbalance using SMOTE.
- Train and compare multiple Machine Learning models.
- Evaluate models using classification metrics.
- Interpret model predictions using SHAP (if implemented in the project).

## Dataset
- **Dataset:** IBM HR Employee Attrition Dataset
- **Records:** 1,470 employees
- **Original Features:** 35
- **Target Variable:** `Attrition`

## Technologies Used
- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- Scikit-learn
- XGBoost
- Imbalanced-learn (SMOTE)
- Joblib
- SHAP (if implemented)

## Project Workflow
1. Exploratory Data Analysis
2. Data Cleaning and Preprocessing
3. Feature Transformation and Scaling
4. Handling Class Imbalance using SMOTE
5. Model Training and Comparison
6. Hyperparameter Tuning
7. Model Evaluation
8. Model Interpretation using SHAP (if implemented)

## Machine Learning Models
- Logistic Regression
- Decision Tree
- Random Forest
- Random Forest with SMOTE
- XGBoost
- Hyperparameter-tuned XGBoost using RandomizedSearchCV

## Model Performance

Update this table using the **latest results from your final training notebook**.

| Model | Accuracy | F1-score | ROC-AUC |
|---|---:|---:|---:|
| Logistic Regression | 86.05% | 0.438 | 0.808 |
| Random Forest + SMOTE | 84.35% | 0.361 | 0.799 |
| Tuned XGBoost | 87.07% | 0.457 | 0.808 |

*Note: These are previously recorded results. Replace them if your latest training run produces different metrics.*

## Explainable AI
SHAP (SHapley Additive exPlanations) can be used to understand how individual features influence model predictions and identify important factors associated with employee attrition.

Keep this section only if SHAP analysis is actually present in the notebooks.

## Project Structure

```text
Employee-Attrition-Prediction/
│
├── datasets/
│   ├── HR-Employee-Attrition.csv
│   └── processed/
│       ├── X_train_scaled.pkl
│       ├── X_test_scaled.pkl
│       ├── y_train.pkl
│       └── y_test.pkl
│
├── images/
│
├── models/
│   ├── scaler.pkl
│   ├── preprocessor.pkl
│   └── final_xgboost.pkl
│
├── notebooks/
│   ├── 01_EDA.ipynb
│   ├── 02_Data_Preprocessing.ipynb
│   └── 03_Model_Training.ipynb
│
├── README.md
├── requirements.txt
└── .gitignore
```

## Installation and Usage

### 1. Clone the repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

### 2. Navigate to the project directory

```bash
cd Employee-Attrition-Prediction
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the notebooks

Open the notebooks using Google Colab or Jupyter Notebook and execute them in the following order:

1. `01_EDA.ipynb`
2. `02_Data_Preprocessing.ipynb`
3. `03_Model_Training.ipynb`

Make sure the dataset and required files are available at the paths expected by the notebooks.

## Author

**Prabhat Kumar**  
B.Tech Computer Science and Engineering  
NIT Kurukshetra
