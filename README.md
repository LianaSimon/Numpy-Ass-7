# NUMPY

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






