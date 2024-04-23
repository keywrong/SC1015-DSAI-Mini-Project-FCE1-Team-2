# Diabetes Classifier using Machine Learning and Optimisation Techniques

## About
This is the Mini-Project done for SC1015 Introduction to Data Science and Artificial Intelligence. In this project, we aim to identify individuals with high risk of diabetes who are undiagnosed, using Data Science and Machine Learning algorithms. 

The dataset we chose is taken from 2021 Behavioural Risk Factor Surveillance System Survey Data and Documentation conducted by US Centers for Disease Control and Prevention (CDC).

The documents and source codes are presented in the following order:
1. [Data Preparation & Cleaning]
2. [Exploratory Data Analysis and Visualisation]
3. [Model 1. Decision Tree]
4. [Model 2. Random Forest]
5. [Model 3. Logistic Regression]

## Contributors
### Team:
Practical Motivation & Problem Formulation
### Choo Yun Chuan, Dylan:
Decision Tree with Optimisation
### Lee Yun Jia:
Data Cleaning, Exploratory Data Analysis & Analytic Visualisation
### Kieron Yew Qi Rong:
Random Forest with Optimisation & Logistic Regression with Optimisaion

## Problem Definition
Diabetes has emerged as a significant health concern in Singapore. Despite being non-fatal in the short term, the increasing prevalence of diabetes (8.8% in 2017 to 9.5% in 2020) poses a huge long-term risk of getting serious comorbidities like Obesity and Heart Disease. Statistics reveal a concerning rise in diabetes, with projections suggesting a surge to 1 million affected individuals by 2050. Additionally, it's noteworthy that more than 400,000 Singaporeans currently grapple with diabetes.

This leads to our problem statement: 
<b>What are the variables correlated with diabetes and how can we identify undiagnosed individuals suffering from diabetes?</b>
- How can we identify undiagnosed individuals suffering from diabetes?
- Which models are most suitable for machine learning?

## Data Cleaning and Preparation
<p>Data cleaning and preparation are crucial steps in the data analysis process. These steps involve transforming raw data into a format that is suitable for analysis, and ensuring that the data is accurate, complete, and consistent. </p>

Key steps involved in our data cleaning and preparation process include:
1. Extract columns that are relevant to our problem, i.e. diabetes analysis
2. Tackling missing values
3. Simplify variable values to suit ML algorithms
4. Making column names more readable 
5. Creating a 50-50 balanced dataset
6. Export cleaned dataset to csv

## Exploratory Data Analysis and Visualisation
After data cleaning, Exploratory Data Analysis (EDA) and Visualisation are conducted to better understand the variables and obtain initial data-driven insights on their relationships with diabetes.

Key steps involved in our EDA and Visualisation include:
1. Uni-variate analysis and visualisation for both numeric and categorical variable
2. Bi-variate analysis and visualisation to identify promising predictor numeric variables via boxplots
3. Bi-variate analysis and visualisation to identify promising predictor categorical variables via catplots

## Machine Learning Models
The models were chosen by considering the large data set and the high number of categorical variables. The following models were used:

### 1. Decision Tree
- Constructing a model of decisions and their possible consequences
- Optimising depth level using AUC value of ROC Curve

### 2. Random Forest
- Using multiple decision trees to diversify train data set 
- Optimising depth level using AUC value of ROC Curve

### 3. Logistic Regression
- Predicting output of a categorical variable based on multiple independent variables
- Optimisation through hyperparameters
- Identifying best hyperparameters through GridSearch

## Conclusion
- Affirm: Smoking is significantly correlated to having diabetes although there has not been any conclusive research about whether it is a main cause or not.
- Debunk: There is no significant difference in the average intake of fruits and vegetables for people with and without diabetes.
- Discover: There is a consistent pattern between the income level of people with and without diabetes, where people in lower income brackets have a surprisingly HIGHER rate of diabetes.
- Observe: Most important variables for prediction are High Blood Pressure and General Health.

## References
https://www.moh.gov.sg/news-highlights/details/result-from-government%27s-five-year-war-against-diabetes-effort
https://www.channelnewsasia.com/singapore/war-against-diabetes-singapore-doctors-seeing-rise-young-patients-below-40-lifestyle-habits-stress-early-screening-treatment-3921976#:~:text=HABITS%2C%20EARLY%20SCREENING-,More%20than%20400%2C000%20people%20in%20Singapore%20live%20with%20diabetes%2C%20with,to%20control%20blood%20sugar%20levels.
https://www.diabetes.org.sg/about-diabetes/the-singapore-demographics-of-diabetes/

### Data Source
https://www.cdc.gov/brfss/annual_data/annual_2021.html

### Machine Learning
https://scikit-learn.org/stable/modules/tree.html
https://developers.google.com/machine-learning/crash-course/classification/roc-and-auc
https://www.section.io/engineering-education/introduction-to-random-forest-in-machine-learning/#:~:text=What%20is%20a%20random%20forest,consists%20of%20many%20decision%20trees
https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegressionCV.html
https://www.kaggle.com/code/funxexcel/p2-logistic-regression-hyperparameter-tuning/notebook
