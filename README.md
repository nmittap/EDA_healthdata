# EDA_healthdata

Aim of the project:
To conduct exploratory data analysis using python to derive insights on drivers of cost of care .

Dataset:
Consists of financial data, clinical data, demographics in csv files of patients hospitalised for a certain condition.
Merged all the files into a single file based on common columns - "patient_id" and "date of admission".
Initial dataset after merging consisted of 13600 rowns and 32 columns.

Data Pre-processing/Data cleaning:
Dataset consisted on missing values in certain columns. Dropped all the rows with missing values.
Certain columns in the dataset required replacing values. For example, gender column consisted of 4 values - "male", "female", "f" and "m". Replaced "f" and "m" values with "female" and "male" respectively.
The next step was to remove duplicate values which were a result of merging.
Calculated columns like age, age group, total amount, bmi and year were added that were necessary for data analysis
The final dataset after all the data cleaning and pre processing steps consisted of 2608 ows and 38 columns.

Exploratory Data analysis:
I conducted univariate, bivariate and multivariate data analysis to get an overall understanding of the variables, relationship between the variables and to that of the target variable(in our case is "total amount") and to finally draw insights about drivers of cost of care.

Univariate data analysis:The objective of univariate analysis is to derive the data, define and summarize it, and analyze the pattern present in it. In a dataset, it explores each variable separately. Univariate analysis can be conducted on both categorical and numerical variables.

Bivariate data analysis: Analysis conducted using two variables denotes bivariate analysis.It helps in understanding the relation between two variavles in a dataset.

Multivariate data analysis:Multivariate analysis is required when more than two variables have to be analyzed simultaneously. It is used to study more complex sets of data and shows relations between multiple variables in a dataset.

In this project I used correlation analysis as a part of multivariate analysis to derive insights on relation between clinical data variables(independent variables) and total amount(dependent variable).
Correlation analysis deals with relationships among variables. The correlation coefficient is a measure of linear association between two variables. Values of the correlation coefficient are always between -1 and +1. A correlation coefficient of +1 indicates that two variables are perfectly related in a positive linear sense, a correlation coefficient of -1 indicates that two variables are perfectly related in a negative linear sense, and a correlation coefficient of 0 indicates that there is no linear relationship between the two variables.Correlation analysis cannot establish cause-and-effect relationships between dependent and independent variables. It can indicate only how or to what extent variables are associated with each other. The correlation coefficient measures only the degree of linear association between two variables. Any conclusions about a cause-and-effect relationship must be based on the judgment of the analyst.

Results/Insights on cost drivers:
Following insights have been drawn from the analysis:
Demographic data: The dataset consisted of patients between the age groups 30-40 years and most of the patient population belonged to chinese race and singaporean resident status. There was equal distribution of male and female patient population in the dataset.
The highest total amount was contributed by 
