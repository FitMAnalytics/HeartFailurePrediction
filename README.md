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
- `Age`: age of the patient [years]
- `Sex`: sex of the patient [M: Male, F: Female]
- `ChestPainType`: chest pain type [TA: Typical Angina, ATA: Atypical Angina, NAP: Non-Anginal Pain, ASY: Asymptomatic]
- `RestingBP`: resting blood pressure [mm Hg]
- `Cholesterol`: serum cholesterol [mm/dl]
- `FastingBS`: fasting blood sugar [1: if FastingBS > 120 mg/dl, 0: otherwise]
- `RestingECG`: resting electrocardiogram results [Normal: Normal, ST: having ST-T wave abnormality (T wave inversions and/or ST elevation or depression of > 0.05 mV), LVH: showing probable or definite left ventricular hypertrophy by Estes' criteria]
- `MaxHR`: maximum heart rate achieved [Numeric value between 60 and 202]
- `ExerciseAngina`: exercise-induced angina [Y: Yes, N: No]
- `Oldpeak`: oldpeak = ST [Numeric value measured in depression]
- `ST_Slope`: the slope of the peak exercise ST segment [Up: upsloping, Flat: flat, Down: downsloping]
- `HeartDisease`: output class [1: heart disease, 0: Normal]

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

