# Autisme Classifier Using Random Forest

## Files
## Files
- autism_screening.csv: Dataset used to train and evaluate the model.
- main.ipynb: Jupyter notebook that implements a Random Forest Classifier for autism screening.

## Dataset
- ** Source: ["autism_screening.csv"] (https://www.kaggle.com/competitions/autism-prediction/data)
- ** Features:
  - A1-A10 scores --> Each item is an answer to the "Autism Spectrum Quotient (AQ) 10 item screening tool [Source: https://embrace-autism.com/aq-10/#test]". However, this tool traditionally gives four response options (Definitely Agree, Slightly Agree, Slightly Disagree, Definitely Disagree). These have been translated to binary values (0 and 1) in the following manner:
    - A1: 1 if Definitely/Slightly Agree, 0 otherwise 
    - A2: 1 if Definitely/Slightly Agree, 0 otherwise 
    - A3: 1 if Definitely/Slightly Disagree, 0 otherwise 
    - A4: 1 if Definitely/Slightly Disagree, 0 otherwise 
    - A5: 1 if Definitely/Slightly Disagree, 0 otherwise 
    - A6: 1 if Definitely/Slightly Disagree, 0 otherwise 
    - A7: 1 if Definitely/Slightly Disagree, 0 otherwise 
    - A8: 1 if Definitely/Slightly Disagree, 0 otherwise 
    - A9: 1 if Definitely/Slightly Agree, 0 otherwise 
    - A10: 1 if Definitely/Slightly Agree, 0 otherwise
  - age, gender, ethnicity, jundice, austim, contry_of_res, used_app_before, result, age_desc, relation
  - Target Variable: Class/ASD (yes or no)

## Objective
Train and evaluate a machine learning model to classify whether a person has austisme syndrome disorder (ASD) based on a standardized questionnaire. 

## Methods
- Preprocessing:
   - Converted categorical values to numerical values
   - Dropped irrelevant or noisy features
- Model:
  - Implemented arandom forest algorithm the RandomForestClassifier algorithm from scikit-learn
  - Split the dataset into 80% training and 20% testing using train_test_split
  - Tuned the "max_depth" and "n_estimators" for performance

## Results
- Accuracy: Model produced result with an accuracy of 0.9574468085106383


