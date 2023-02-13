
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






