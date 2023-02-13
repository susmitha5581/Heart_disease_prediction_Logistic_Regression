
# **Heart Disease Prediction**
![Heart disease](https://github.com/susmithareddy-1996/Heart_disease_prediction/blob/main/images/Heart%20disease.jpg)

"Heart disease is broad term used for diseases and conditions affecting the heart and circulatory system. They are also referred as cardiovascular diseases. It is a major cause of disability all around the world. Since heart is amongst the most vital organs of the body, its diseases affect other organs and part of the body as well. There are several different types and forms of heart diseases. The most common ones cause narrowing or blockage of the coronary arteries, malfunctioning in the valves of the heart, enlargement in the size of heart and several others leading to  **heart failure and heart attack."**

## **Problem**

World Health Organization has estimated 12 million deaths occur worldwide, every year due to Heart diseases. Half the deaths in the United States and other developed countries are due to cardio vascular diseases. The early prognosis of cardiovascular diseases can aid in making decisions on lifestyle changes in high risk patients and in turn reduce the complications. This research intends to pinpoint the most relevant/risk factors of heart disease as well as predict the overall risk using logistic regression.

## **Solution**

The classification goal is to predict whether the patient has 10-year risk of future coronary heart disease (CHD).

I have implemented Logistic Regression Model to predict Coronary Heart Disease.

# **Data information**

Data set: [Heart disease prediction.csv](https://github.com/susmitha5581/Heart_disease_prediction_Logistic_Regression/blob/main/Heart%20disease%20prediction.csv)

## **Overview**
![overview](https://github.com/susmithareddy-1996/Heart_disease_prediction/blob/main/images/overview.png)

## **Contents**
Basic Data Analysis

Analyzing Features using Visualizations 

Cleaning the dataset 

Standardization 

Normalization  

Feature selection 

Applying models 

Conclusion 

Will you develop CHD?

## **Basic data Analysis**

Before anything is done to the data, we must take a look at the features and values included. 

Here are what all the features are described as: 

male: 0 = Female; 1 = Male 

age: Age at exam time.

education: 1 = Some High School; 2 = High School or GED; 3 = Some College or Vocational School; 4 = college 

currentSmoker: 0 = nonsmoker; 1 = smoker 

cigsPerDay: number of cigarettes smoked per day (estimated average) 

BPMeds: 0 = Not on Blood Pressure medications; 1 = Is on Blood Pressure medications 

prevalentStroke 

prevalentHyp 

diabetes: 0 = No; 1 = Yes 

totChol: mg/dL 

sysBP: mmHg 

diaBP: mmHg 

BMI: Body Mass Index calculated as: Weight (kg) / Height(meter-squared) 

heartRate: Beats/Min (Ventricular) 

glucose: mg/dL 

TenYearCHD: If the patient has had congestive heart failure in the last ten years. This will be what my models will be predicting. 

## **Analysing Features using Visualization**
![variables](https://github.com/susmitha5581/Heart_disease_prediction_Logistic_Regression/blob/main/images/variables.png)

## **Correlation Matrix**
![correlations](https://github.com/susmitha5581/Heart_disease_prediction_Logistic_Regression/blob/main/images/correlations.png)

## **Data Cleaning**

We have to find a way to effectively remove or replace the null values so that models can be applied.
The education column could be very subjective, has many null values and has no correlation to the other feature, so I'm going to drop it.

Here I want to change the column name Males as gender

And here Gender as 0 = Female; 1 = Male

## **Standardization**

Standardization is an important technique that is mostly performed as a pre-processing step before many Machine Learning models, to standardize the range of features of input data set.

## **Normalization**

Normalization is a data preparation technique that is frequently used in machine learning. The process of transforming the columns in a dataset to the same scale is referred to as normalization. Every dataset does not need to be normalized for machine learning.

![Normalization](https://github.com/susmitha5581/Heart_disease_prediction_Logistic_Regression/blob/main/images/Normalization.png)

Without a thorough analysis of this data, models will be more likely to predict that a patient does not have heart disease. The unbalance will be resolved by splitting training and testing data and then balancing the training data. To ensure that the training data is balanced, I will undersample to balance the training data.

When you get to the model training section, you may notice that I don't use these normalized values for training. I tried using the normalized values and the 4 types of accuracies were almost around the same percentages, which is good, however all the accuracies were between 50%~70%. So, I decided to not use the normalized data.

## **Feature selection**

![Feature Selection](https://github.com/susmitha5581/Heart_disease_prediction_Logistic_Regression/blob/main/images/Feature%20Selection.png)

## **Models Used**

**Linear regression** : Logistic Regression Machine Learning is basically a classification algorithm that comes under the Supervised category (a type of machine learning in which machines are trained using "labelled" data, and on the basis of that trained data, the output is predicted) of Machine Learning algorithms. This simply means it fetches its roots in the field of Statistics.

**Random forest** : Random forest is a commonly-used machine learning algorithm trademarked by Leo Breiman and Adele Cutler, which combines the output of multiple decision trees to reach a single result. Its ease of use and flexibility have fueled its adoption, as it handles both classification and regression problems.

**KNN** : It is one of the simplest algorithms in Machine Learning. This algorithm is a supervised algorithm. The main function of this algorithm is to identify new items or cases by checking older items or cases in data set. Mainly it checks whether the new case has some similarity with older cases which is available in data set, or not. This algorithm can be used in both regression and classification techniques of Machine Learning. But it is mainly used in classification cases. This algorithm is a non parametric algorithm because it does not build any assumptions by underlying data. We know for every model there is training stage where the model learns about the method of prediction but for KNN algorithm the training phase is quite different. In training phase it only takes the data set and when new cases arrive then it stores them by checking older data set. This algorithm is called as lazy learner algorithm because it does not learn fast from training data set. It only does action when there are new cases. For this reason it is named so.

## **Conclusion**


![conclusion](https://github.com/susmitha5581/Heart_disease_prediction_Logistic_Regression/blob/main/images/Feature%20Selection.png)


In logistic regression, we get a little higher when comparing three models

