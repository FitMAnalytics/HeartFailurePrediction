# Heart Failure Prediction using Machine Learning

This project aims to predict heart failure outcomes using ensemble learning techniques, including Decision Tree, Random Forest, and XGBoost. The goal is to predict whether a patient will experience heart failure based on various medical features.

## Table of Contents
1. [Overview](#overview)
2. [Data](#data)
3. [Modeling](#modeling)
   - [Decision Tree](#decision-tree)
   - [Random Forest](#random-forest)
   - [XGBoost](#xgboost)
4. [Evaluation](#evaluation)
5. [Installation](#installation)
6. [License](#license)

## Overview
The project is based on the **Heart Failure Prediction** dataset from [Kaggle](https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction). The dataset contains various features related to heart failure and aims to predict the likelihood of heart failure in patients.

Machine learning models used:
- **Decision Tree**: A simple and interpretable classification model based on decision-making rules.
- **Random Forest**: An ensemble model that aggregates multiple decision trees to improve accuracy and reduce overfitting.
- **XGBoost**: A powerful gradient boosting algorithm known for its speed and performance in structured/tabular data.

## Data
The dataset used for this project contains the following features:
- `age`: Age of the patient
- `anaemia`: Whether the patient has anaemia (1 = yes, 0 = no)
- `creatinine_phosphokinase`: Level of the enzyme creatinine phosphokinase in the blood
- `diabetes`: Whether the patient has diabetes (1 = yes, 0 = no)
- `ejection_fraction`: Percentage of blood pumped by the heart with each beat
- `high_blood_pressure`: Whether the patient has high blood pressure (1 = yes, 0 = no)
- `platelets`: Platelet count in the blood
- `serum_creatinine`: Serum creatinine level in the blood
- `serum_sodium`: Serum sodium level in the blood
- `sex`: Gender of the patient (1 = male, 0 = female)
- `smoking`: Whether the patient is a smoker (1 = yes, 0 = no)
- `time`: Duration of follow-up (in days)
- `DEATH_EVENT`: Target variable indicating whether the patient died (1 = death, 0 = survival)

## Modeling
### Decision Tree
A Decision Tree classifier was then trained to predict heart failure outcomes. The model was implemented using the `DecisionTreeClassifier` from the `sklearn.tree` library, and hyperparameters were tuned (using the grid search method) to improve accuracy.

### Random Forest
We used the Bayesian Search to tune the hyperparameters of the Random Forest classifier. The Random Forest classifier was implemented using the `RandomForestClassifier` from the `sklearn.ensemble` library.

### XGBoost
XGBoost, a gradient boosting algorithm, was used for classification. The `XGBClassifier` from the `xgboost` library was employed, and the model was optimized through hyperparameter tuning to achieve the best performance.

## Evaluation
Each model was evaluated using classification metrics such as:
- **Accuracy**
- **Precision**
- **Recall**
- **F1-Score**
- **ROC-AUC Score**

The models were compared, and the best-performing model was selected for heart failure prediction.

## Installation
1. Clone this repository:
    ```bash
    git clone https://github.com/FitMAnalytics/HeartFailurePrediction.git  
    ```
2. Run the Jupyter Notebook to see the results:
    ```bash
    jupyter notebook heart_failure_prediction.ipynb
    ```

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

