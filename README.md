# 118BFinal-Project

Implementation and Evaluation of several machine learning models to predict housing prices as part of the UC San Diego class COGS118B Intro to Machine Learning

 <img src="https://github.com/janinaschuhmacher/UCSD_COGS118B_final_ML_project/blob/master/test_accuracies.png" alt="Test accuracies for each classifier per feature
                                                                                                                      and overall"  width="800" height="800">


## Summary

In this project, we compared the performance of different classifiers in a binary classification task. The goal was to predict if a person makes more or less than 50 k per year, given a set of categorical and continuous attributes. The algorithms which we used were support vector machines with linear kernel (SVM) and multilayer perceptrons with different activation functions. As can be seen in the figure above, testing accuracy was around 0.86 for all classifiers except for SVM with automated correction for class imbalance which had significantly lower testing accuracy. Training and testing accuracies were similar for all classifiers, indicating good generalization from training to test data. The biggest challenge consisted in the imbalance in the data set, resulting in relatively poor recall rates and, consequently, low F1 scores. Using sklearn’s automated
correction for class imbalance improved recall but at the cost of lowering precision.

## The data

For our project, we use the [“Census Income Data Set”](https://archive.ics.uci.edu/ml/datasets/Census+Income).

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

Further information about the data set and relevant publication can be found on the UCI Machine Learning Repository website (https://archive.ics.uci.edu/ml/datasets/Census+Income).





