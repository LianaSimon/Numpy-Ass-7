# NUMPY

## 📘 Introduction

This repository contains a set of beginner-friendly Python exercises using NumPy and Pandas, designed to build foundational data manipulation and analysis skills. Each exercise focuses on key concepts such as array creation, reshaping, slicing, Series and DataFrame operations, filtering, and file handling.

These programs are well-suited for anyone starting with data science, machine learning, or Python programming in general. The code is written to be simple, clear, and easy to follow within a Jupyter Notebook environment.



pip install numpy

import numpy as np

### Exercise 1: 

#### Create a numpy array containing the numbers from 1 to 10, and then reshape it to a 2x5 matrix.

#### PROGRAM 1

arr1=np.arange(1,11)

reshaped_arr=arr1.reshape(2,5)

print("2*5 matrix is ",reshaped_arr)


#### OUTPUT 1

![image](https://github.com/user-attachments/assets/dbf1f48d-7bfe-4cfe-95de-8e7e3c7efb8d)



### Exercise 2: 

#### Create a numpy array containing the numbers from 1 to 20, and then extract the elements between the 5th and 15th index.


#### PROGRAM 2

arr2=np.arange(1,21)

extracted=arr2[5:16]

print("The extracted array from 5th to 15th index are: ",extracted)


#### OUTPUT 2

![image](https://github.com/user-attachments/assets/1e2b3b7c-6134-4d66-99ec-ea77de1c639d)


### Exercise 3: 

#### Create a Pandas series with the following data: {'apples': 3, 'bananas': 2, 'oranges': 1}. Then, add a new item to the series with the key 'pears' and the value 4.

pip install pandas

import pandas as pd

#### PROGRAM 3

fruits=pd.Series({'apples':3,'bananas':2,'oranges':1})

fruits['pears']=4

print("The series of fruits with new item,'pears' added is:\n")

fruits

#### OUTPUT 3

![image](https://github.com/user-attachments/assets/69b0a13e-811f-4e67-ba06-931872d3116a)



### Exercise 4: 

#### Create a dataframe with the following columns: name, age, and gender. The dataframe should have 10 rows of data.


#### PROGRAM 4

data={

    'Name':['Alice','Susan','Leo','Jim','Henry','Rhea','Derick','Anna','Katerine','Jake'],
    
    'Age':[25,12,32,22,18,45,27,36,55,11],
    
    'Gender':['F','F','M','M','M','F','M','F','F','M']
    
}


df=pd.DataFrame(data)

print("DATA FRAME:\n\n",df)


#### OUTPUT 4

![image](https://github.com/user-attachments/assets/63897aa2-188e-4c33-860c-6e5062e922cb)


### Exercise 5: 

#### Add a new column to the data frame created in question 1, called occupation. The values for this column should be Programmer, Manager, and Analyst, corresponding to the rows in the dataframe.


#### PROGRAM 5

occupations=['Programmeer','Manager','Analyst']*3+['Programmer']

df['Occupations']=occupations

print("NEW DATA FRAME:\n",df)


#### OUTPUT 5

![image](https://github.com/user-attachments/assets/2f6f5a60-9c1d-416f-be2a-d32ac889ae1a)


### Exercise 6: 

#### Select the rows of the dataframe where the age is greater than or equal to 30.


#### PROGRAM 6

age_above30=df[df['Age']>=30]

print("The rows of the dataframe where the age is greater than or equal to 30 are:\n",age_above30)


#### OUTPUT 6

![image](https://github.com/user-attachments/assets/1f1a28c3-9147-4b47-a5d7-96faa351d5bc)



### Exercise 7: (Score : 2)

#### Convert this dataframe to a csv file and read that csv file, finally display the contents.

#### PROGRAM 7

##### #Save to CSV file

df.to_csv('people_data.csv',index=0)

##### #Read the CSV file

df_csv=pd.read_csv('people_data.csv')

print("Contents of CSV file: \n",df_csv)


#### OUTPUT 7

![image](https://github.com/user-attachments/assets/cf554050-b226-43f7-954a-86cc3ed3b907)




## ✅ Conclusion

These exercises provide a practical introduction to working with NumPy and Pandas—two of the most essential libraries for data analysis in Python. By completing them, users can gain hands-on experience in creating arrays, manipulating data, and working with real-world data structures like Series and DataFrames.

Feel free to fork this repository, explore further, and build on top of these examples as you continue your journey in data science!




