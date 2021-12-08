# EDA_healthdata

Aim of the project:
To conduct exploratory data analysis using python to derive insights on drivers of cost of care .

Dataset:
Consists of financial data, clinical data, demographic data of patients hospitalised for a certain condition in different csv files.
Merged all the files into a single file(merge.csv) based on common columns - "patient_id" and "date of admission".
Initial dataset after merging consisted of 13600 rowns and 32 columns.

Data Pre-processing/Data cleaning:
Dataset consisted on missing values in certain columns. Dropped all the rows with missing values.
Certain columns in the dataset required replacing values. For example, gender column consisted of 4 values - "male", "female", "f" and "m". Replaced "f" and "m" values with "female" and "male" respectively.
The next step was to remove duplicate values which resulted from merging.
Calculated columns like age, age group, total amount, bmi and year were added that were necessary for data analysis.
The final dataset after all the data cleaning and pre processing steps consisted of 2608 rows and 38 columns.

Exploratory Data analysis:
I conducted univariate, bivariate and multivariate data analysis to get an overall understanding of the variables, relationship between the variables and to that of the target variable(in our case is "total amount") and to finally draw insights about drivers of cost of care.

Univariate data analysis:The objective of univariate analysis is to derive the data, define and summarize it, and analyze the pattern present in it. In a dataset, it explores each variable separately. Univariate analysis can be conducted on both categorical and numerical variables.

Bivariate data analysis: Analysis conducted using two variables denotes bivariate analysis.It helps in understanding the relation between two variavles in a dataset. in our case, I conducted this analysis for variables like age, gender, race etc vs total amount to understand the relation between them.

Multivariate data analysis:Multivariate analysis is required when more than two variables have to be analyzed simultaneously. It is used to study more complex sets of data and shows relations between multiple variables in a dataset.

In this project I used correlation analysis as a part of multivariate analysis to derive insights on relation between numeric variables(independent variables) and total amount(dependent variable).

Correlation analysis deals with relationships among variables. The correlation coefficient is a measure of linear association between two variables. Values of the correlation coefficient are always between -1 and +1. A correlation coefficient of +1 indicates that two variables are perfectly related in a positive linear sense, a correlation coefficient of -1 indicates that two variables are perfectly related in a negative linear sense, and a correlation coefficient of 0 indicates that there is no linear relationship between the two variables.Correlation analysis cannot establish cause-and-effect relationships between dependent and independent variables. It can indicate only how or to what extent variables are associated with each other. The correlation coefficient measures only the degree of linear association between two variables.

Results/Insights on cost drivers:
Following insights have been drawn from the analysis:
Demographic data: From univariate analysis it is evdient that the dataset consisted of most of the patients between age groups 30-40 years and most of the patient population belonged to chinese race and singaporean resident status. There was equal distribution of male and female patient population in the dataset.
Bivariate analysis shows that the patients with Malaysian race, foreigners(resident status), and age group of 80-90 (with more males than females in that age group) contirubute to the highest total amount. In the overall dataset, males and females equally contribute to the total amount.
From multivariate analysis conducted to see the relation between numeric variables and total sum,symptom 5,age,medical history 1, symptom 3, medical history 6 and symptom 4 are identified as the top contributors driving the cost of care.
