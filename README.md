# Project-Diabetes-Prediction

# About Dataset

This dataset is originally from the National Institute of Diabetes and Digestive and Kidney Diseases. The objective of the dataset is to diagnostically predict whether or not a patient has diabetes, based on certain diagnostic measurements included in the dataset. Several constraints were placed on the selection of these instances from a larger database. In particular, all patients here are females at least 21 years old of Pima Indian heritage.

Link: https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database


## Features

### Pregnencies:

Pregnancy history of the patient.


### Glucose: 

#### Fasting blood glucose levels in adults: 

Normal Range: Typically, a fasting blood glucose level between 70 mg/dL (3.9 mmol/L) and 100 mg/dL (5.6 mmol/L) is considered normal.

Prediabetes Range: Fasting blood glucose levels between 100 mg/dL (5.6 mmol/L) and 125 mg/dL (6.9 mmol/L) may indicate prediabetes.

Diabetes Range: A fasting blood glucose level of 126 mg/dL (7 mmol/L) or higher on two separate occasions is often used as a diagnostic threshold for diabetes.

#### Postprandial Blood Sugar (PPBS) values:

Normal Range: Typically, a PPBS value below 140 mg/dL (7.8 mmol/L) is considered normal for most individuals. This measurement is often taken 2 hours after a meal.

Prediabetes Range: PPBS values between 140 mg/dL (7.8 mmol/L) and 199 mg/dL (11.0 mmol/L) may indicate prediabetes.

Diabetes Range: A PPBS value of 200 mg/dL (11.1 mmol/L) or higher on two separate occasions is often used as a diagnostic threshold for diabetes.


### Blood Pressure:

The acceptable range of blood pressure values can vary depending on factors such as age, sex, and individual health conditions. Blood pressure is typically measured using two values: systolic pressure (the higher number) and diastolic pressure (the lower number), both measured in millimeters of mercury (mm Hg). Here are general guidelines for blood pressure values:

Normal Blood Pressure: A normal blood pressure reading is usually defined as systolic pressure below 120 mm Hg and diastolic pressure below 80 mm Hg, often written as "120/80 mm Hg."

Elevated Blood Pressure: Elevated blood pressure, sometimes referred to as prehypertension, falls in the range of systolic pressure between 120 and 129 mm Hg and diastolic pressure below 80 mm Hg.

Hypertension Stage 1: Stage 1 hypertension is diagnosed when systolic pressure ranges from 130 to 139 mm Hg or diastolic pressure ranges from 80 to 89 mm Hg.

Hypertension Stage 2: Stage 2 hypertension is diagnosed when systolic pressure is 140 mm Hg or higher, or diastolic pressure is 90 mm Hg or higher.

#### Note: In this dataset only the diastolic pressure(Lower number) is given.


### Skin Thickness:

For adult males and females, the normal range for triceps skinfold thickness can be approximately 10 to 25 millimeters (mm) or more, depending on age and gender. 


### Insulin: 

Fasting insulin levels typically fall within the range of approximately 5 to 15 μU/ml for many individuals.


### Body Mass Index (weight in kg/(height in m)^2):

#### Lower Risk BMI Category:

BMI between 18.5 and 24.9 kg/m^2
This category is associated with a lower risk of weight-related health conditions and is often considered a "healthy" or "good" BMI range for many individuals.

#### Higher Risk BMI Category:

BMI of 25.0 kg/m^2 or higher
This category includes individuals who are classified as overweight or obese and may be at a higher risk for weight-related health issues.


### Diabetes Pedigree Function:

The "Diabetes Pedigree Function" in the dataset likely quantifies the genetic predisposition to diabetes based on family history.


### Age:

Age of the individual

The dataset can also be found within this repository folder Project-01 Full.

Data Preprocessing is done based on the presence of 0 values of some features.

Exploratory Data Analysis (EDA) EDA has been performed to understand the distribution of all the input features.

Model Building Logistic Regression for binary classification, KNN, Random Forest are used and to build the final implementable machine learning model Random Forest model with certain hyper parameter tuning is used. The model is having train and test accuracy of 82% and 76% repectively.

Model Evaluation Model's performance has been evaluated using Clawssification Report, Confusion Matrix, Accuracy score and Cross Validation tests for both test and train datasets.

Usage The model can be trained as shown in the .ipynb file and relevant input variables can be given to predict the output by using the following example code: 
prediction = rfc.predict(scaler.transform([[5,155,89,32,0,40.5,0.589,51]]))
if prediction == [1]:
    print('The patient is Diabetic')
else:
    print('The patient is not diabetic')


### Outcome:
The person is "diabetic"
