# Prediction-of-Cirrhosis-Outcomes-with-XGB
Predicting the multi-class outcomes of cirrhosis patients using an XGB classifier

![image](https://github.com/user-attachments/assets/0f525470-ef9b-4a20-b10e-a716ae6fe90e)

---

### Objective
This project was completed as part of Kaggle's Playground Series competitions (Season 3, Episode 26). The main goal of this project is to use a multi-class approach to predict the outcomes of patients with cirrhosis. Broadly speaking, cirrhosis is a condition in which the liver is severely scarred due to excessive liver injury. This permanent scarring can ultimately lead to liver failure and thus can be fatal. For this project, the cirrhosis will lead to three possible outcomes: 1) The patient was alive, 2) The patient was alive due to a liver transplant, 3) The patient was deceased. This project leverages an XGB Classifier model to solve this multi-class classification task. The dataset used in this project was provided by Kaggle (under the CC BY 4.0 license) and was synthetically generated from an actual Cirrhosis Patient Survival Prediction dataset. 

---

### Methods
Libraries Used
- numpy
- pandas
- matplotlib
- seaborn
- sklearn (train_test_split, LabelEncoder, Kmeans, TimeSeriesSplit, log_loss, KFold)
- xgboost
- optuna

Data Preprocessing
- Converting object-type predictors to numerical w/ LabelEncoder()

Exploratory Data Analysis (EDA)
- Viewing summary statistics of the train and test datasets
- Histograms visualizing the distributions of predictor variables
- Bar charts showing the counts of each target variable class
- Heatmap (correlation matrix) showing potential correlations amongst features

Building the Model
- XGB classifier
- 80% train, 20% test
- Leveraging optuna to run trials to determine optimal parameters (eval metric: 'mlogloss'

---

### General Results
The final model yielded a log loss of ~0.427.
