# Diabetes-Prediction-2
____

# About the Dataset
The Diabetes prediction dataset is a collection of medical and demographic data from patients, along with their diabetes status (positive or negative). The data includes features such as age, gender, body mass index (BMI), hypertension, heart disease, smoking history, HbA1c level, and blood glucose level. This dataset can be used to build machine learning models to predict diabetes in patients based on their medical history and demographic information. This can be useful for healthcare professionals in identifying patients who may be at risk of developing diabetes and in developing personalized treatment plans. Additionally, the dataset can be used by researchers to explore the relationships between various medical and demographic factors and the likelihood of developing diabetes.

____
# Attributes
1. age
2. gender
3. body mass index (BMI)
4. hypertension, heart disease
5. smoking history
6. HbA1c level
7. blood glucose level

____
# Data Transformation
1. All the categorical values converted to numerical/ ordinal values
2. All ages in decimal were removed and age converted from float to integer data type
3. The SMOT technique was applied to balance the highly imbalanced dataset

____

# Data Visualization
1. The box plot for diabetes VS blood_glucose level
   
   Observation:-

                 a. The Box Plot for diabetes VS blood_glucose level appears to be similar for all genders except for the 'other' gender category.
   
                 b. This might be due to the small sample size of the 'other' gender category having only 18 samples amoung the total 96146 samples.
   
                 c. Thus this could give us a potential bias when model training and prediction.

2. The box plot for Diabetes VS age

   Observation:-

                 a. The plots indicates that there is a higher chance of suffering from Diabetes with increasing age.
   
                 b. Females (0) have a little higher probability of gettind diabetes and hypertension with age than Males (1)

3. The box plot for Hypertension VS age

   Observation:-

                 a. The plots indicates that there is a higher chance of suffering from Hypertension with increasing age.
   
                 b. Females (0) have a little higher probability of gettind diabetes and hypertension with age than Males (1)

4. The line plot for HbA1c level VS blood glucose level

   Observation:-

                 a. The HbA1c level and blood glucose level between males and females have a similar pattern, but it is very different for the 'other' gender category.
   
                 b. This might be due to the small sample size of the 'other' gender category having only 18 samples amoung the total 96146 samples.
   
                 c. Thus this could give us a potential bias when model training and prediction.

5. The Line plot for blood_glucose_level VS BMI

   Observation:-

                 a. The Line plot for blood_glucose_level VS BMI shows similar pattern for both males and females, but the pattern is highly different fot the 'other' gender category.
   
                 b. This might be due to the small sample size of the 'other' gender category having only 18 samples amoung the total 96146 samples.
   
                 c. Thus this could give us a potential bias when model training and prediction.

____
# Model Accuracy before and after SMOTE
