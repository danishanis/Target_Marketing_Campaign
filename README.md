# Marketing Ad Campaign - Case Study
*Project to predict who is most likely to click on an Ad that generates revenue*

**Author: Danish Anis**

**Contact: danishanis10@hotmail.com**

## Business Objective

As a part of my job shadowing assignment, I was asked to present this case study for a bank's Analytics Team and assist in devising a target Ad campaign. The aim of this case study is to be able to predict how much profit a marketing team can make by accurately classifying which of their target customers are most likely to click on their ads.

Also pertinent to the study is to be able to comment on how a particular feature contributes to the end result and how can those results be optimized by adequate EDA, Feature Engineering & Model Optimization

## Background

Profit & Loss are to be determined based on who clicks on the Ad. We assume that we spend **$1000 per potential customer**. For each **customer that we target** with our ad campaign **and** that **clicks on the ad**, we get an **overall profit of $100**. However, if we target a **customer that ends up not clicking** on the ad, we incur a **net loss of $1050**. Therefore we can conclude that for each **customer that was not targeted** by the campaign **and** who **clicks on the ad**, we get an **overall profit of $1100**.

Unfortunately, we have no information about the advertized product; this information could have guided us through our understanding of the user behavior.

## Dataset Information

The dataset includes available features or labelled columns for analysis as follows:

**Daily Time Spent on Site** : in minutes

**Age** : Users' age in years

**Area Income** : In $

**Daily Internet Usage** : In Units

**Ad Topic Line** : Topics of respective Target Campaigns

**City**

**Male** : Binary column, 1 meaning 'Male' and '0' meaning Female

**Country**

**Timestamp** : Needs to be converted for analysis

**Clicked on Ad** : *Target Variable*. 0 meaning 'No', 1 meaning 'Yes'

## Technologies/Libraries Used

 - *Python 3*
 - *Jupyter*
 - *Pandas*
 - *Numpy*
 - *Datetime*
 - *Matplotlib*
 - *Scikit-Learn*
 - *Scipy*
 
## Feature Insights

Feature dependencies with respect to target variables have been visualized to understand behaviors. Following is a peak into the box plot & distribution plot analysis that reveal useful trends: 

![alt text](https://github.com/danishanis/Target_Marketing_Campaign/blob/master/Images/bplots.png)

![alt text](https://github.com/danishanis/Target_Marketing_Campaign/blob/master/Images/distplots.png)

## Model Results

Models trained & tested for classification were **Logistic Regression, Decision Tree Classifier** and **Random Forest Classifier**. The Logistic Regression model was tuned with L2 Regularization and achieved the best evaluation scores. Using metrics, the following summary was created in terms of **Profit from Correct Classifications** and **Losses incurred from misclassifications**, including the number of misclassifications that need to be reduced.

![alt text] (https://github.com/danishanis/Target_Marketing_Campaign/blob/master/Images/logreg.png)

The ROC metric for the model is as follows:

![alt text](https://github.com/danishanis/Target_Marketing_Campaign/blob/master/Images/roc.png)

## Miscellaneous

Feature importance was ranked using the Random Forest Classifier as per the following. Please refer to the Feature Engineering cell for clarification on updates features:

![alt text](https://github.com/danishanis/Target_Marketing_Campaign/blob/master/Images/featimp.png)
