# Predicting Cardiovascular Disease using AWS Sagemaker

## Project Overview
The purpose of this project is to predict cardiovascular disease in aws using sagemaker studio. This feasibility study is structured in the following order:
- Exploratory data analysis
- Model development using sklearn´s open-source linear model
- Model development using Sagemaker´s build-in linear model
- Model Deployment
- Model Evaluation

## Running the JupyterNotebook
- create an IAM user with adequate permissions
- open the notebook in Sagemaker Studio
- select image "Data Science"
- select kernel: Python 3

## Exploratory Data Analysis
- see Jupyter Notebook

## Model Development
- see Jupyter Notebook

## Model Evaluation

![cm](figures/confusion_mat.png)

The confusion matrix shows the percentages of the true predicted labels (0: healthy; 1: cardiovascular disease) using the linear built-in model by Sagemaker. The model correctly classifies 75% of all healthy subjects as healthy while 25% of the heathy are being misclassified as being healthy. The model further classifies 69% of all unhealthy subjects as unhealthy while 31% of the healthy are being misclassified as being healthy. The overall accuracy score of the model is 72%. With a recall score of 69% and a precision score of 73%, the f1 score is 71%. The roc-auc score is 78%.  

![cm](figures/prec_recall.png)

Plotting recall vs precision shows that the precision smoothly decreases with increasing recall. For example, if the model is calibrated to detect 80% (recall) of all subjects with cardiovascular disease, then the precision is a little below 70% meaning the 70% of all predictions are correct.  

In conclusion, the mode is quite robust but however could probably be improved by applying also non-linear classifiers such as xgboost or neural networks.