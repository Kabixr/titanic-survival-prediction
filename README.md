Titanic Survival Prediction (Machine Learning)

This repository contains a complete machine learning pipeline for the Kaggle Titanic Survival Prediction Challenge.  
The goal is to predict whether a passenger survived based on their demographic and travel information.

## 📁 Project Structure
titanic-survival-prediction/
│
├── train.csv # Kaggle training dataset
├── test.csv # Kaggle test dataset
├── gender_submission.csv # Baseline sample submission
├── titanic_survival_prediction.ipynb # Full Colab notebook
├── submission.csv # Model output for Kaggle submission
└── README.md # Project documentation


## 🧠 Model Overview
The notebook performs:

### 1. Data Cleaning  
- Missing value imputation  
- Handling categorical values  
- Scaling numeric features  

### 2. Feature Engineering  
- Extract `Title` from Name  
- Compute `FamilySize`, `IsAlone`  
- Detect `CabinKnown`  
- Encode categorical features using OneHot  

### 3. Model Training  
Model used: **RandomForestClassifier**

Includes:
- Train/validation split  
- 5-fold cross-validation  
- ROC-AUC analysis  
- Feature importance ranking  

### 4. Final Submission  
Generates a `submission.csv` file ready for Kaggle.

## 🚀 How to Run
Install libraries:
```bash
pip install pandas numpy scikit-learn matplotlib


Open the notebook:

titanic_survival_prediction.ipynb


Run all cells.
A submission.csv will be created in the working directory.

📊 Results

Typical metrics:

Accuracy: ~0.80

ROC AUC: ~0.82

CV Accuracy: ~0.78–0.82 range

🏁 Author

Kabir Puri
