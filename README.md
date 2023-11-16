## Ex-03 UNIVARIATE ANALYSIS
## AIM
To read the given data and perform the univariate analysis with different types of plots.
## EXPLANATION
Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.
## ALGORITHM
Step1:Read the given data.

Step2:Get the information about the data.

Step3:Remove the null values from the data.

Step4:Mention the datatypes from the data.

Step5:Count the values from the data.
## PROGRAM:
```
Developed By : NAVEENAA V.R
Register Number : 212221220035
```
## superstore.csv
```
import pandas as pd
import numpy as np
import seaborn as sns
df=pd.read_csv('/content/SuperStore (1).csv')
print(df)
df.head()
df.info()
df.dtypes
df['Postal Code'].value_counts()
sns.boxplot(x='Postal Code', data=df)
sns.countplot(x='Postal Code',data=df)
sns.distplot(df["Postal Code"])
df.describe()
```
## employeesal.csv
```
import pandas as pd
df=pd.read_csv("/content/employeesal (1).csv")
df
df.info()
df.dtypes
df['Salary'].value_counts()
df.describe()
import seaborn as sns
sns.boxplot(x='Experience_Years',data=df)
sns.countplot(x="Experience_Years",data=df)
sns.distplot(df['Experience_Years'])
sns.histplot(x="Experience_Years",data=df)
df.skew()
sns.histplot(x='Salary',data=df)
sns.distplot(df['ID'])
df.kurtosis()
sns.boxplot(x='Salary',data=df)
sns.boxplot(x='Experience_Years',data=df)
```
## diabetes.csv
```
import pandas as pd
import numpy as np
import seaborn as sns
df = pd.read_csv("/diabetes.csv")
df
df.info()
df.isnull().sum()
df.dtypes
df.describe()
df['Glucose'].value_counts()
sns.boxplot(x="Glucose",data=df)
sns.countplot(x="Glucose",data=df)
sns.distplot(df['Glucose'])
sns.histplot(x="Glucose",data=df)
df.skew()
df.kurtosis()
```
## OUTPUT
![image](https://github.com/Naveenaa28/ODD2023-DataScience-Ex-03/assets/131433133/cb4e1d32-1f00-4683-8611-94ba498b353c)
![image](https://github.com/Naveenaa28/ODD2023-DataScience-Ex-03/assets/131433133/c971163f-eb7b-45e6-bcbc-c00042caa9fa)
![image](https://github.com/Naveenaa28/ODD2023-DataScience-Ex-03/assets/131433133/6984312a-1d90-43ae-b087-63eaeb4d6e62)
![image](https://github.com/Naveenaa28/ODD2023-DataScience-Ex-03/assets/131433133/cdd2dc67-5569-430f-8f27-d0d67da3453d)
![image](https://github.com/Naveenaa28/ODD2023-DataScience-Ex-03/assets/131433133/84e1f362-7aac-4cd1-bb1a-c234f14fcc2c)
![image](https://github.com/Naveenaa28/ODD2023-DataScience-Ex-03/assets/131433133/c1293b9f-893e-42a9-8c4a-73069fb9c6f3)
![image](https://github.com/Naveenaa28/ODD2023-DataScience-Ex-03/assets/131433133/777c9230-dbb0-4d3b-b78c-d6de243cfb39)
![image](https://github.com/Naveenaa28/ODD2023-DataScience-Ex-03/assets/131433133/0509d594-b4eb-49d1-8d7d-65ea4bd52ad6)
![image](https://github.com/Naveenaa28/ODD2023-DataScience-Ex-03/assets/131433133/063d7808-a498-423f-b3ef-6cd38ae7ab20)
![image](https://github.com/Naveenaa28/ODD2023-DataScience-Ex-03/assets/131433133/6418abc9-f024-4d10-869a-13c22cbbfe30)
![image](https://github.com/Naveenaa28/ODD2023-DataScience-Ex-03/assets/131433133/d764940c-5022-4f23-acbb-62cf10bf46a8)
![image](https://github.com/Naveenaa28/ODD2023-DataScience-Ex-03/assets/131433133/568b2033-950e-4089-8850-4b65b94271bd)
![image](https://github.com/Naveenaa28/ODD2023-DataScience-Ex-03/assets/131433133/f7815b43-e26d-4b1f-9b2a-e2cc7d0313e6)
![image](https://github.com/Naveenaa28/ODD2023-DataScience-Ex-03/assets/131433133/4ede76f5-b26f-4908-a6bd-145dfdcba10a)
![image](https://github.com/Naveenaa28/ODD2023-DataScience-Ex-03/assets/131433133/63fb6eea-37e4-46c4-9507-bbe47c19a737)
![image](https://github.com/Naveenaa28/ODD2023-DataScience-Ex-03/assets/131433133/c2743427-f9fa-4d57-a89a-040076b3917a)
![image](https://github.com/Naveenaa28/ODD2023-DataScience-Ex-03/assets/131433133/53ac4f35-1339-401a-b0ed-8294fa1a4a0c)
![image](https://github.com/Naveenaa28/ODD2023-DataScience-Ex-03/assets/131433133/0b44b90f-7076-47a0-bee0-c2e7c1aa4ef6)
![image](https://github.com/Naveenaa28/ODD2023-DataScience-Ex-03/assets/131433133/c3cde1b5-2c13-4e6f-9603-bcf39bcd9b69)
## RESULT
Hence the univariate analysis is verified.
