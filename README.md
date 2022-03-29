# Ex-01_DS_Data_Cleansing


## AIM
To read the given data and perform data cleaning and save the cleaned data to a file. 

# Explanation
Data cleaning is the process of preparing data for analysis by removing or modifying data that is incorrect ,incompleted , irrelevant , duplicated or improperly formatted. 
Data cleaning is not simply about erasing data ,but rather finding a way to maximize datasets accuracy without necessarily deleting the information. 

# ALGORITHM
### STEP 1
Read the given Data
### STEP 2
Get the information about the data
### STEP 3
Remove the null values from the data
### STEP 4
Save the Clean data to the file


# CODE
```
import pandas as pd
df=pd.read_csv("Data_set.csv")
df.head(10)
df.tail()
df.info()
df.isnull().sum()
df['show_name']=df['show_name'].fillna(df['show_name'].mode()[0])
df.head()
df['rating']=df['rating'].fillna(df['rating'].mean())
df.info()
```

# OUPUT
output1:
![image](https://user-images.githubusercontent.com/94165326/159853794-8f288f57-3104-48ec-ab06-1fced896aad5.png)
output2:
![image](https://user-images.githubusercontent.com/94165326/159853924-c2d9cbe5-ce45-4569-b13a-535d2a1b1628.png)
output3:
![image](https://user-images.githubusercontent.com/94165326/159854023-6f0f6288-d62e-4568-841a-e4c45ca7e386.png)

