# 118BFinal-Project

Implementation and Evaluation of several machine learning models to predict housing prices as part of the UC San Diego class COGS118B Intro to Machine Learning

## Goal of the project
Prediction task is to determine whether a person makes over 50K a year. 

## The data

According to information from the [UCI ML repository](https://archive.ics.uci.edu/ml/datasets/adult), the data was extracted by Barry Becker from the 1994 Census database. 

The following attributes are part of the dataset: 

* target variable: yearly income (>50K, <=50K)

We used the following predictor variables: 
* age: continuous
* workclass: Private, Self-emp-not-inc, Self-emp-inc, Federal-gov, Local-gov, State-gov, Without-pay, Never-worked
* education: Bachelors, Some-college, 11th, HS-grad, Prof-school, Assoc-acdm, Assoc-voc, 9th, 7th-8th, 12th, Masters, 1st-4th, 10th, Doctorate, 5th-6th, Preschool
* education-num: continuous
* marital-status: Married-civ-spouse, Divorced, Never-married, Separated, Widowed, Married-spouse-absent, Married-AF-spouse
* occupation: Tech-support, Craft-repair, Other-service, Sales, Exec-managerial, Prof-specialty, Handlers-cleaners, Machine-op-inspct, Adm-clerical, Farming-fishing, Transport-moving, Priv-house-serv, Protective-serv, Armed-Forces
* relationship: Wife, Own-child, Husband, Not-in-family, Other-relative, Unmarried
* race: White, Asian-Pac-Islander, Amer-Indian-Eskimo, Other, Black
* sex: Female, Male
* capital-gain: continuous
* capital-loss: continuous
* hours-per-week: continuous
Further, we only included datapoints from the US to avoid class imbalance. 

Source: https://archive.ics.uci.edu/ml/datasets/adult


## Method


