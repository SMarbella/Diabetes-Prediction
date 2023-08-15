# Diabetes Data Mining Prediction - Frequency of Type 2 Diabetes Among Women of Pima Indigenous Heritage Living Near Phoenix, Arizona
Final Project for INFO 523: Data Mining and Discovery

Video: https://youtu.be/HklvHK4OKtk

## Dataset Information
**Title:** Pima Indians Diabetes Database

**Date of Study:** 1989 Nov 8

**Author:** Vincent Sigillito (vgs@aplcen.apl.jhu.edu), Larrie Hutton, and Richard S. Johannes

**Affiliation:** Research Center, RMI Group Leader Applied Physics Laboratory The Johns Hopkins University Johns Hopkins Road Laurel, MD 20707 (301) 953-6231 © Date received: 9 May 1990

**Original owners:** National Institute of Diabetes and Digestive and Kidney Diseases

**Relevant Information:** Several constraints were placed on the selection of these instances from a larger database. In particular, all patients here are females at least 21 years old of Pima Indian heritage.

**Source:** https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2245621/

**PDF:** https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2245621/pdf/procascamc00017-0301.pdf

## Table Columns
This diabetes dataframe comes from Datahub.io. It appears in many research papers regarding the frequency of type 2 diabetes among indigenous Native American people. The columns included in the table are:

Pregnancies - Number of pregnancies.

GlucoseLevel - Plasma glucose concentration from a 2-hour oral glucose tolerance test.

BloodPressure - Diastolic blood pressure measurement (mm Hg) taken at the time of the study.

SkinThickness - Triceps skin fold thickness (mm).

Insulin - 2-hour serum insulin (mu U/ml).

BMI - Body Mass Index at the time of the study (weight in kg/(height in m)^2).

DiabetesPedigreeFunction - A measure of genetic influence that provides data on diabetes mellitus history in relatives and the genetic relationship of those relatives to the patient.

Age - The woman's age in years at the time of the study.

Outcome - Tested either positive or negative for diabetes.

## Retrieved table from
- https://datahub.io/machine-learning/diabetes
- https://www.kaggle.com/datasets/akshaydattatraykhare/diabetes-dataset

## Other sources that used this dataset
1. https://diabetesjournals.org/diabetes/article/70/8/1603/137883/Pima-Indian-Contributions-to-Our-Understanding-of?searchresult=1
2. https://www.cdc.gov/diabetes/data/statistics-report/diagnosed-undiagnosed-diabetes.html
3. https://diabetesjournals.org/diabetes/article/69/Supplement_1/532-P/58032/532-P-The-Longitudinal-Determinants-of-Diabetic?searchresult=1
4. https://diabetesjournals.org/diabetes/article/64/12/3993/34762/Dissecting-the-Etiology-of-Type-2-Diabetes-in-the?searchresult=1

Many more that cited them: https://diabetesjournals.org/diabetes/search-results?page=1&q=pima&fl_SiteID=1000001

# Charts Generated For This Project
## Frequency of Being Diagnosed with Diabetes Based on Age
Plot 1 measures the frequency of type 2 diabetes in women of Pima indigenous heritage living near Phoenix, Arizona as they age. Older women are more likely to be tested positive for type 2 diabetes than younger women.
![Image](https://github.com/SMarbella/Diabetes-Prediction/blob/main/data/Chart%20-%20Frequency%20of%20Diabetes%20by%20Age.png)

## Frequency of Diabetes Between Age and Number of Pregnancies
Plot 2 measures the frequency of type 2 diabetes in women of Pima indigenous heritage living near Phoenix, Arizona as they age or have more children. Very few women have 5 or more children because nowadays, families do not produce that many children. Women get pregnant at a younger age because these years are their productive years. Most young women, whether they are pregnant or not, are less likely to become diabetic. As the woman ages, her chance of becoming diabetic increases. Women can become diabetic regardless of the number of pregnancies.

![Image](https://github.com/SMarbella/Diabetes-Prediction/blob/main/data/Chart%20-%20Diabetes%20by%20Age%20%26%20Pregnancy.png)

## Frequency of Diabetes Between Age and Blood Pressure Level
Plot 3 measures the frequency of type 2 diabetes between age and blood pressure. Younger women under 30 years old usually test negative for type 2 diabetes. Their diastolic blood pressure is within the normal limit of 60 to 80 mm Hg. Around 35 years old to 60 years old, the chances of becoming diabetic and hypertensive increases.
![Image](https://github.com/SMarbella/Diabetes-Prediction/blob/main/data/Chart%20-%20Diabetes%20Status%20by%20Age%20%26%20BP.png)

## Frequency of Diabetes Between BMI and Glucose Level
Plot 4 measures the frequency of type 2 diabetes between glucose level and BMI. As women's BMI reaches 25 and up (Obesity), their glucose level increases. The higher the BMI above the normal range (18.5–24.99), the higher the chance the woman becomes diabetic. According to American Diabetes Association (https://diabetes.org/diabetes/a1c/diagnosis), the normal glucose level in an oral glucose tolerance test is less than 140 mg/dL. Prediabetes is 140 to 199 mg/dL. Diabetes is 200 mg/dL or higher. At about 130 mg/dL glucose level and higher, majority of women are already at a high risk of becoming diabetic.
![Image](https://github.com/SMarbella/Diabetes-Prediction/blob/main/data/Chart%20-%20Diabetes%20by%20BMI%20%26%20Glucose%20Level.png)

## Frequency of Diabetes in Different Tricep Skin Fold Thickness and BMI
Plot 5 measures the frequency of type 2 diabetes between skin thickness and BMI. As a woman's BMI increases and her triceps skin fold thickness increases, the likelihood of becoming diabetic is prominent. Women with BMI 25 and higher and have thicker triceps skin folds (mm) are at a higher risk of getting type 2 diabetes.
![Image](https://github.com/SMarbella/Diabetes-Prediction/blob/main/data/Chart%20-%20Diabetes%20by%20BMI%20%26%20Skin%20Thickness.png)

## Frequency of Diabetes in Family History
Plot 6 measures the frequency of type 2 diabetes in the diabetes pedigree function. The diabetes pedigree function is a function that measures the likelihood of type 2 diabetes based on family history. A higher value in the diabetes pedigree function indicates that the woman is at risk of developing type 2 diabetes. Women can still become diabetic even when their diabetes pedigree is lower than 0.5. However, there are more women who tested negative for diabetes with a diabetes pedigree of 0.5 and lower.
![Image](https://github.com/SMarbella/Diabetes-Prediction/blob/main/data/Chart%20-%20Diabetes%20Status%20by%20Family%20History.png)

## Association Rules For Diabetes Frequency
The Association Rules from the apriori library compare the risk of type 2 diabetes occurring under different body conditions, such as number of Pregnancies, Blood Glucose Level, Blood Pressure, Skin Thickness, Insulin level, BMI, and Age.
![Image](https://github.com/SMarbella/Diabetes-Prediction/blob/main/data/Apriori%20Diabetes%20Association%20Rules.png)

The arulesViz library visualizes the rules. The x axis represents the support while the y axis represents the confidence or lift. Support indicates how frequently a set of items appear in the data. It is the number of transactions that contains this set. Confidence or lift indicates how often the support rule is true. Lift is a measure of association using both support and confidence. The lift value of an association rule includes the list of rules whose confidence is above the threshold.

![Image](https://github.com/SMarbella/Diabetes-Prediction/blob/main/data/Apriori%20-%20Visualized%20Association%20Rules%20Diabetes%20in%20Pima%20Indigenous%20Women.png)

The previously created Association Rules can be sorted and filtered to find the best rules. A high filter, such as lift > 2.9, picks out the best rules. The best rules have a very high confidence (precision) and low support (recall) value because they show that the data is very precise. In this data, values with a lift > 2.9 show that certain table columns have a strong association with positive type 2 diabetes diagnosis.

![Image](https://github.com/SMarbella/Diabetes-Prediction/blob/main/data/Apriori%20-%20Best%20Association%20Rules%20Diabetes%20in%20Pima%20Indigenous%20Women.png)
