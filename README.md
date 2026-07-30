# Exno:1
Data Cleaning Process

# AIM
To read the given data and perform data cleaning and save the cleaned data to a file.

# Explanation
Data cleaning is the process of preparing data for analysis by removing or modifying data that is incorrect ,incompleted , irrelevant , duplicated or improperly formatted. Data cleaning is not simply about erasing data ,but rather finding a way to maximize datasets accuracy without necessarily deleting the information.

# Algorithm
STEP 1: Read the given Data

STEP 2: Get the information about the data

STEP 3: Remove the null values from the data

STEP 4: Save the Clean data to the file

STEP 5: Remove outliers using IQR

STEP 6: Use zscore of to remove outliers

# Coding and Output
1. import pandas as pd
df=pd.read_csv("SAMPLEIDS.csv")
print(df)
print(df.shape
<img width="792" height="492" alt="image" src="https://github.com/user-attachments/assets/98558d98-ed86-4985-a169-325b43d4b828" />
<img width="315" height="515" alt="image" src="https://github.com/user-attachments/assets/0acb96d3-b1fa-4d40-ac50-ab6dd28fd821" />

2. df.head(7)
<img width="1003" height="337" alt="image" src="https://github.com/user-attachments/assets/1a87f6ad-bce2-4d39-a364-f6e5aa8e6d0e" />

3. df.tail()
<img width="1005" height="252" alt="image" src="https://github.com/user-attachments/assets/184a734a-a2c3-4251-b257-be9ea1c3254e" />

4. df.info()
<img width="438" height="425" alt="image" src="https://github.com/user-attachments/assets/89d308a4-f22b-4333-908a-bc8b5b30eb58" />
5. df.describe()
<img width="947" height="363" alt="image" src="https://github.com/user-attachments/assets/0fb47938-f0da-493b-8a60-9bbcefd50349" />

6. df.isnull().sum()
<img width="221" height="561" alt="image" src="https://github.com/user-attachments/assets/66d07f65-8e7d-40bf-bf6c-f89faa77937b" />

7. df.isnull().any()
<img width="233" height="577" alt="image" src="https://github.com/user-attachments/assets/65c3a381-5a45-49d1-8b65-873ff311ab36" />

8. df.dropna()
<img width="1018" height="570" alt="image" src="https://github.com/user-attachments/assets/83874295-7cd3-4887-94d2-8f121e8d37ab" />

9. df.fillna(7)
<img width="818" height="658" alt="image" src="https://github.com/user-attachments/assets/b1314b82-1aa5-434c-a902-6793f5c2d48f" />

10. df.fillna(method='ffill')
<img width="817" height="698" alt="image" src="https://github.com/user-attachments/assets/acfae78b-8c03-4988-b2f7-6a15547d30c6" />

11. df.fillna({'GENDER':'MALE','NAME':'AADHI'})
<img width="852" height="685" alt="image" src="https://github.com/user-attachments/assets/f79f916f-ab49-479b-adc0-3f62e597751b" />


# Result
 Thus,the the given data is cleaned and saved successfully. 
