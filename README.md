# Loan-default-prediction-SBA

Data science project containing preprocessing and machine learning - predicting default in SBA loans.

# Requirements

The project was developed using python 3.6.9

### Packages

Following packages were used:

- Pandas 1.0.5
- Numpy 1.18.5
- Sklearn 0.22.2.post1
- Plotly 4.4.1
- Matplotlib 3.2.2
- Seaborn 0.10.1
- Scipy 1.4.1
- Xgboost 0.90
- Joblib 0.16.0


### Software

Project was created using Google Colaboratory and this is recommended environment for reviewing and executing the code. Google Colaboratory already have all required packages installed. Google Colab is accessible via google drive and there is no need to install any software. Otherwise you can use Jupyter Notebook. This option may require to adjust display options for plotly graphics and to install missing libraries with pip install command.

### Data

Dataset used in the project is bigger size than 25mb, therefore couldn't be attached to the repository files on github. Please download it directly from the kaggle:
https://www.kaggle.com/mirbektoktogaraev/should-this-loan-be-approved-or-denied

Please use download button, unzip file and upload SBAnational.csv to your Google Colaboratory notebook working files using 'Upload to session storage' button in 'Files' section.

### Code

Project code is avalaible in Loan_default_SBA.ipynb file. To execute code please add file to the google drive, open it in Google Colaboratory, upload dataset (please see above) and use 'Run all' option in 'Runtime' menu.

# Project description

The goal of the project was to create an effective model being able to predict if loan will be repaid by borrower or not, therefore if bank should grant a loan. Dataset used in the project contains real SBA data concerning borrower and loan itself, however it does not include financial information about the company applying for a loan.

The project consists of two parts: prepocessing including feature engineering, data cleaning, data exploring, data visualizations and machine learning including data preparation, models building, models validation and hyperparameters tuning, models evaluation, models dump.

# Summary

Best results from all of the models used in the project (logistic regression, decision tree, XGBoost, and K-nearest neighbors classifiers) was achieved by decision tree classifier with 75% value of the threshold. The f1 score and false negative rate metrics were used to evaluate the model as classification risk in project problem is not symmetrical, therefore accuracy metric is not sufficient for purpose of evaluation.

The best model obtained 93% in the f1 score metric. False negative rate for the model was about 11%.
