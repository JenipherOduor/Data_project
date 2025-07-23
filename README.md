# H1N1 FLU VACCINE INTAKE PREDICTION USING MACHINE LEARNING

## PROJECT OVERVIEW
The goal of this project is to predict whether individuals got the H1N1 flu vaccine during the 2009 outbreak. The data was collected through a phone survey and included information on respondent’s demographics, social and economic background, health behaviours and opinion on the flu and vaccination. 

## ABOUT THE DATA
**Files Used**
  - `training_set_features.csv`: Demographic, health, and opinion data.
  - `training_set_labels.csv`: Target labels (H1N1 and seasonal flu vaccine).

- **Target Variable**: `h1n1_vaccine`
  - `1`: Received the vaccine
  - `0`: Did not receive the vaccine

  The dataset has 36 features and each row represents an individual respondent

  ## TOOLS AND LIBRARIES
  - Python
  - Pandas, NumPy
  - Scikit-learn
  - Matplotlib

  ## ## Methodology

### Data Preprocessing
- Handled missing values using median (numerical) and "Missing" placeholder (categorical).
- Split dataset using `train_test_split` with stratification.

### Baseline Model: Logistic Regression
- Accuracy: 0.837  
- Recall (vaccinated): 0.441  
- ROC-AUC: 0.829

### 🔹 Tuned Logistic Regression
- Tuned `C` and `penalty` using `GridSearchCV`
- Recall (vaccinated): ** 0.72**
- ROC-AUC: **0.829**

### 🔹 Decision Tree (for comparison)
- Recall (vaccinated): 0.451  
- ROC-AUC: 0.640

## FINDING
- The tuned logistic regression model significantly improved recall while maintaining good precision.
- Logistic regression outperformed decision trees on most performance metrics.

  

