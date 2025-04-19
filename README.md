# Alzheimer’s Disease Prediction using Machine Learning

**Team Video presentation link** : https://youtu.be/w3NqzkMJKy0

## Overview  
This project aims to develop a machine learning-based early warning system for predicting Alzheimer’s Disease (AD) onset using clinical, lifestyle, and cognitive data. Early detection is key to slowing disease progression and enabling timely medical interventions.

##  Dataset  
- **Source**: Kaggle  
- **Size**: 2,149 records with 35 features  
- **Target**: `Diagnosis` (0 = No Alzheimer’s, 1 = Alzheimer’s)

### Key Features:
- **Demographics**: Age, Gender, Education  
- **Lifestyle**: Diet, Physical Activity, Sleep, Smoking, Alcohol  
- **Medical History**: Cardiovascular Disease, Diabetes, Depression  
- **Cognitive Assessments**: MMSE, Functional Assessment, Memory Complaints  
- **Symptoms**: Confusion, Disorientation, Personality Changes  

##  Methodology  
### 1. Data Preprocessing  
- Handled missing values (mean/mode imputation)  
- Removed duplicates  
- Label encoding of categorical variables  

### 2. Feature Engineering  
- Applied **StandardScaler** for normalization  
- Used **Recursive Feature Elimination (RFE)** with Random Forest to select top 10 features  

### 3. Class Balancing  
- Original dataset was imbalanced  
- Applied **SMOTE** to generate synthetic samples for the minority class (Alzheimer’s)  

### 4. Model Training  
- Split data: 70% train / 30% test (with stratification)  
- Models used: Logistic Regression, SVM, Random Forest  
- Evaluation metrics: Accuracy, Precision, Recall, F1-score  

### 5. Hyperparameter Tuning  
- Performed **GridSearchCV** on Random Forest  
- Improved performance from 90.5% to 91% accuracy  

##  Results  
- **Final Model**: Random Forest  
- **Accuracy**: 91%  
- **Precision (AD class)**: 0.94  
- **Recall (AD class)**: 0.86  
- **F1-score**: 0.90  
- Model demonstrated reliable, confident predictions in synthetic test cases  

##  Future Work  
- Integrate MRI/genetic data  
- Apply deep learning models (CNNs, LSTM)  
- Develop a web-based CDSS  
- Use NLP for analyzing clinical notes  
- Model interpretability with SHAP/LIME  
- Real-world validation  

##  References  
- Alzheimer’s Disease Facts and Figures, 2024  
- The Lancet Commission Report on Dementia, 2020  
- NIA-AA Research Framework  

