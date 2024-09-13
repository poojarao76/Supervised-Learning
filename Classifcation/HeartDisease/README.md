 # HEART DISEASE PREDICTION USING LOGISTIC REGRESSION

### Introduction

World Health Organization has estimated 12 million deaths occur worldwide, every year due to Heart diseases. Half the deaths in the United States and other developed countries are due to cardiovascular diseases. The early prognosis of cardiovascular diseases can aid in making decisions on lifestyle changes in high-risk patients and turn, reduce the complications. This research intends to pinpoint the most relevant/risk factors of heart disease and predict the overall risk using logistic regression.


## Dataset

The project uses the Framingham Heart Study dataset, which is publicly available on Kaggle. The dataset consists of demographic, behavioral, and medical history information of patients and is used to predict the 10-year risk of coronary heart disease.

Dataset link: https://www.kaggle.com/datasets/aasheesh200/framingham-heart-study-dataset

**Dataset Attributes:**

Each attribute is a potential risk factor. There are both **demographic, behavioural and medical risk factors**.


1. **Demographic:** 

**sex:** male or female;(Nominal)

**age:** age of the patient;(Continuous - Although the recorded ages have been truncated to whole numbers, the concept of age is continuous)
Behavioural

**currentSmoker:** whether or not the patient is a current smoker (Nominal)

**cigsPerDay:** the number of cigarettes that the person smoked on average in one day.(can be considered continuous as one can have any number of cigarretts, even half a cigarette.)

2. **Medical( history):**

**BPMeds:** whether or not the patient was on blood pressure medication (Nominal)

**prevalentStroke:** whether or not the patient had previously had a stroke (Nominal)

**prevalentHyp:** whether or not the patient was hypertensive (Nominal)

**diabetes:** whether or not the patient had diabetes (Nominal)

3. **Medical(current):**

**totChol:** total cholesterol level (Continuous)

**sysBP:** systolic blood pressure (Continuous)

**diaBP:** diastolic blood pressure (Continuous)

**BMI:** Body Mass Index (Continuous)

**heartRate:** heart rate (Continuous - In medical research, variables such as heart rate though in fact discrete, yet are considered continuous because of the large number of possible values.)

**glucose:** glucose level (Continuous)

**Predict variable (desired target):**

**TenYearCHD:** 10 year risk of coronary heart disease CHD (binary: “1”, means “Yes”, “0” means “No”)


## Prerequisites

This project uses the Framingham Heart Study dataset. The dataset is downloaded from Kaggle using the 'opendatasets' library and loaded into a Pandas DataFrame for analysis.

Before running the code, make sure you have the following Python packages installed:

* pandas
* numpy
* matplotlib
* seaborn
* opendatasets

You can install these packages using "pip".

### Usage

1. **Download the Dataset:**
   
The dataset is automatically downloaded from Kaggle using the opendatasets library. Please make sure you have an active internet connection.


2. **Load the Dataset:**
   
The dataset is loaded into a Pandas DataFrame from the CSV file.


3. **Model Training:**

The project uses logistic regression to predict the 10-year risk of CHD. The dataset is split into training and test sets, and the logistic regression model is trained on the training set.


4. **Model Evaluation:**

Model performance is evaluated using accuracy, ROC curves, and the AUC score.


## Key Steps


1. **Data Preprocessing:** 

Missing values are handled and categorical variables are converted into numeric format using one-hot encoding.

2. **Logistic Regression:** 

A logistic regression model is trained to predict the TenYearCHD.

3. **Evaluation:** 

The model's performance is evaluated using accuracy, confusion matrix, ROC curve, and AUC score.


## Results

* **Accuracy:** The model achieves an accuracy of 85% in predicting heart disease risk.

* **ROC Curve:** The ROC curve shows the trade-off between sensitivity and specificity.

* **AUC:** The AUC score of the model is 0.67, indicating a reasonable ability to distinguish between patients with and without heart disease risk.


## Conclusion

The logistic regression model successfully predicts the 10-year risk of coronary heart disease with decent accuracy. The AUC score of 0.67 indicates room for improvement, potentially by using a more comprehensive dataset or more complex models.
