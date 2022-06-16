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

## Model Evaluation

![cm](/images/confusion_mat.PNG)

The precision-recall curve confirms that achieving a recall of 50% comes in for free in terms that the precision starts decreasing only when the recall is above 50%. An efficient set point would be to chose a recall of around 80% and thus allowing the precision to drop to around 80%. However, optimizing the tradeoff between recall and precision requires profound business knowlede in terms of the costs of false-positive and false-negative predictions.  

