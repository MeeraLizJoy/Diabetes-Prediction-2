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

Before/After SMOTE	Model Name	   True Negative	False Positive	False Negative	True Positive	Accuracy Score	F1 Score

0	Before	         LR	            16936	         141	         639	         1111	         0.958570	      0.740173

1	Before	         KNN	         17077	         0	            1750	         0	            0.907048	      0.000000

2	Before	         SVM	         17008	         69	            729	         1021	         0.957614	      0.719014

3	Before	         Naive Bayes	   15865	         1212	         601	         1149	         0.903702	      0.558988

4	Before	         DecisionTree	17077	         0	            1750	         0	            0.907048     	0.000000

5	Before	         RandomForest	17013	         64	            543	         1207	         0.967759	      0.799073

6	After	            LR	            15108	         2023	         258	         1438	         0.878844	      0.557689

7	After	            KNN	         15298	         1833	         347	         1349	         0.884209	      0.553096

8	After	            SVM	         14909	         2222	         125	         1571	         0.875339	      0.572418

9	After	            Naive Bayes	   15223	         1908	         327	         1369	         0.881288	      0.550573

10	After	            DecisionTree	16525	         606	         430	         1266	         0.944973	      0.709641

11	After	            RandomForest	16999	         132	         488	         1208	         0.967069	      0.795784
