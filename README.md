# Heart Disease Classifier: Project Overview
* Created a heart disease classifier (Accuracy ~90              %)
* Engineered features by creating indicator features.
* Tuned and optimized hyper-parameters of Ridge Logistic Regression, Support Vector Machine, Random Forest and AdaBoost. 

## Code and Resources Used
**Python Version:** 3.8.2

**Packages:** pandas, numpy, sklearn, matplotlib, seaborn, pickle

## Exploratory Data Analysis
I looked at the distributions the features and the summary statistics. Below are a few of the visualizations I used.

!["Distribution of Age with Respect to Heart Disease](https://github.com/vatdaell/Heart-Disease-Analysis/blob/master/readme_images/age_dist.png "Distribution of Age with Respect to Heart Disease")

![Thal vs Age with respect to heart disease](https://github.com/vatdaell/Heart-Disease-Analysis/blob/master/readme_images/agevsthal.png "Thal vs Age with respect to heart disease")

![Confusion matrix](https://github.com/vatdaell/Heart-Disease-Analysis/blob/master/readme_images/confusion%20matrix.png "Thal vs Age with respect to heart disease")


## Model 
I created a train-test split of the data where the test was 20%. 

I used accuracy to measure the effectiveness of the model while making sure the true negative remained low.

I used 4 different models:

**L2-Penalty Logistic Regression:** - Used as a Baseline

**Support Vector Machine** - To combat potential overfitting of logistic regression

**Random Forest** - Ensemble method to combat overfitting and because there are lots of sparse categorical features 

**AdaBoost** - Boosting Random Forests usually perform better than standard Random Forests

## Model Performance

The AdaBoosted Random Forest with Logistic Regression estimators performed the best.

**L2-Penalty Logistic Regression:** - Accuracy: 92%        

**Support Vector Machine** - Accuracy: 90%

**Random Forest** - Accuracy: 90%

**AdaBoost** - Accuracy: 94%