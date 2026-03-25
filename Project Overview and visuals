 
<img width="376" height="221" alt="image" src="https://github.com/user-attachments/assets/1debb2f8-db71-4a06-a300-56fecb3a92e7" />






# Titanic Survival Prediction 🚢

![Python](https://img.shields.io/badge/python-3.12-blue)
![License](https://img.shields.io/badge/license-MIT-green)

---

## 📌 Project Overview

This project aims to predict which passengers survived the Titanic disaster using machine learning techniques.  
The dataset is sourced from the [Kaggle Titanic Competition](https://www.kaggle.com/c/titanic).

---

## 🎯 Objectives

- Perform data cleaning and preprocessing  
- Explore survival patterns through visualization  
- Build predictive models  
- Improve performance using feature engineering  

---

## 📂 Dataset

### Data Dictionary

| Variable   | Definition                        | Key |
|------------|----------------------------------|-----|
| survival   | Survival                           | 0 = No, 1 = Yes |
| pclass     | Ticket class                       | 1 = 1st, 2 = 2nd, 3 = 3rd |
| sex        | Sex                                |     |
| age        | Age in years                       |     |
| sibsp      | # of siblings / spouses aboard     |     |
| parch      | # of parents / children aboard    |     |
| ticket     | Ticket number                      |     |
| fare       | Passenger fare                     |     |
| cabin      | Cabin number                       |     |
| embarked   | Port of Embarkation                | C = Cherbourg, Q = Queenstown, S = Southampton |

**Notes**:

- `pclass`: a proxy for socio-economic status (1st = Upper, 2nd = Middle, 3rd = Lower)  
- `age`: fractional if less than 1; estimated ages may be `xx.5`  
- `sibsp` & `parch`: define family relations aboard  

---

## 🔍 Exploratory Data Analysis (EDA)

Key insights:

- Female passengers had significantly higher survival rates than males  
- First-class passengers were more likely to survive  
- Passengers traveling alone had lower survival rates  

<img width="682" height="478" alt="image" src="https://github.com/user-attachments/assets/184c78f8-26dd-488f-8999-6e406e84ff79" />


---

## 🛠️ Data Preprocessing

- Handled missing values:
  - `Age` → filled with median  
  - `Embarked` → filled with mode  
- Removed irrelevant columns: `Ticket`, `Cabin`  
- Encoded categorical variables:
  - `Sex` → numeric mapping  
  - One-hot encoding for `Embarked` and `Title`  

---

## ⚙️ Feature Engineering

- `Title` → extracted from passenger names  
- `FamilySize` → `SibSp + Parch + 1`  
- `IsAlone` → 1 if passenger traveled alone, 0 otherwise  
- `FarePerPerson` → `Fare / FamilySize`  

---

## 🤖 Model Building

Two models were explored:

1. **Logistic Regression** – baseline model  
2. **Random Forest Classifier** – final model  

**Random Forest Parameters**:

- `n_estimators = 300`  
- `max_depth = 8`  
- `min_samples_split = 4`  
- `min_samples_leaf = 2`  

<img width="694" height="448" alt="image" src="https://github.com/user-attachments/assets/ed454820-69d8-4f0b-99be-7a0dcf774a99" />

---

## 📊 Model Evaluation

- **Validation Accuracy**: ~0.84  
- **Cross-validation Score**: ~0.825  

---

## 🏆 Kaggle Submission

- Final Kaggle Score: **0.77990**  
- Submission file generated using the trained Random Forest model  

---

