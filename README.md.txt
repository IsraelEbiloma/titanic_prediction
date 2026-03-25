 Titanic Survival Prediction 🚢

📌 Project Overview
This project aims to predict which passengers survived the Titanic disaster using machine learning techniques.  
The dataset is sourced from the Kaggle Titanic competition.


🎯 Objectives
- Perform data cleaning and preprocessing
- Explore survival patterns through visualization
- Build predictive models
- Improve performance using feature engineering


📂 Dataset
Data Dictionary
Variable	Definition	Key
- survival	Survival	0 = No, 1 = Yes
- pclass	Ticket class	1 = 1st, 2 = 2nd, 3 = 3rd
- sex	Sex	
- Age	Age in years	
- sibsp	# of siblings / spouses aboard the Titanic	
- parch	# of parents / children aboard the Titanic	
- ticket	Ticket number	
- fare	Passenger fare	
- cabin	Cabin number	
- embarked	Port of Embarkation	C = Cherbourg, Q = Queenstown, S = Southampton

Variable Notes
pclass: A proxy for socio-economic status (SES)
1st = Upper
2nd = Middle
3rd = Lower

age: Age is fractional if less than 1. If the age is estimated, is it in the form of xx.5

sibsp: The dataset defines family relations in this way...
Sibling = brother, sister, stepbrother, stepsister
Spouse = husband, wife (mistresses and fiancés were ignored)

parch: The dataset defines family relations in this way...
Parent = mother, father
Child = daughter, son, stepdaughter, stepson
Some children travelled only with a nanny, therefore parch=0 for them.

Source: Kaggle Titanic Competition

🔍 Exploratory Data Analysis (EDA)
Key insights from the data:
- Female passengers had significantly higher survival rates than males
- First-class passengers were more likely to survive
- Passengers traveling alone had lower survival rates


🛠️ Data Preprocessing
- Missing values handled:
  - Age → filled with median
  - Embarked → filled with mode
- Irrelevant columns removed:
  - Ticket, Cabin
- Categorical variables encoded:
  - Sex mapped to numerical values
  - One-hot encoding applied to Embarked and Title

⚙️ Feature Engineering
New features were created to improve model performance:
- Title- extracted from passenger names
- FamilySize- = SibSp + Parch + 1
- IsAlone- (whether a passenger traveled alone)
- FarePerPerson = Fare / FamilySize

🤖 Model Building
Two models were explored:
- Logistic Regression (baseline)
- Random Forest (final model)

Final Model: Random Forest Classifier

Parameters:
- n_estimators = 300
- max_depth = 8
- min_samples_split = 4
- min_samples_leaf = 2



📊 Model Evaluation
- Validation Accuracy: ~0.84
- Cross-validation Score: ~0.825

🏆 Kaggle Submission
- Final Kaggle Score: 0.77990
- Submission file generated using the trained Random Forest model

📁 Project Structure