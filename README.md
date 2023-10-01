# pesu_io



print("Hello world")
     
Hello world

n=int(input("enter a number:"))
if n%2==0 :
  print("is even number")
else:
  print("is odd")
     
enter a number:6
is even number

text= input("enter the string ")
vowels= ['a', 'e','i', 'o', 'u']
for i in text:
  if i in vowels:
    print(i)
     
enter the string sameer
a
e
e

l=[1,1,3,4,4,4,6,7,8,8,8]
d={}
for i in l:
  if i in d:
    d[i]+=1
  else:
    d[i]=1
print(d)
     
{1: 2, 3: 1, 4: 3, 6: 1, 7: 1, 8: 3}

str="betty bought butter but the butter was bitter so betty bought better butter to make the bitter butter better"
list=str.split(" ")
myset=set(list)
#print(myset)
d={}

for i in list:
  if i in d:
    d[i]+=1
  else:
    d[i]=1
print(d)
     
{'betty': 2, 'bought': 2, 'butter': 4, 'but': 1, 'the': 2, 'was': 1, 'bitter': 2, 'so': 1, 'better': 2, 'to': 1, 'make': 1}

n_1=input("Enter the first name ")
a_1=int(input("Enter the age"))
n_2=input(("Enter the second name"))
a_2=int(input("Enter the age"))
print(a_1+a_2)

     
Enter the first name sameer 
Enter the age19
Enter the second namehota
Enter the age19
38

a=int(input("Enter the first number"))
b=int(input("Enter the second number"))
c=int(input("Enter the third"))
mean=(a+b+c)/3
print(mean)
     
Enter the first number3
Enter the second number7
Enter the third8
6.0

l=int(input("Enter the length: "))
b=int(input("Enter the breadth: "))
h=int(input("Enter the height: "))
volume=(l*b*h)
print(volume)
     
Enter the length: 3
Enter the breadth: 5
Enter the height: 6
90

num=int(input("Enter the number : "))

if num < 0:
   print("Enter a positive number")
else:
   sum = 0

   while(num > 0):
       sum += num
       num -= 1
   print("The sum is", sum)


     
Enter the number : 17
The sum is 153

a=int(input("Enter the first number: "))
b=int(input("Enter the second number:"))
if(a
Enter the first number: 6
Enter the second number:3
HCF is : 3

def fact(n):
    return 1 if (n==1 or n==0) else n * fact(n - 1);

num = 5
print("Factorial of",num,"is",)
fact(num)
     
Factorial of 5 is
120

l= [10,20,30,10,40,20,40,50,60,30]

dupe = []
org = set()

for i in l:
    if i in org:
        dupe.append(i)
    else:
        org.add(i)


print("Duplicate are:", dupe)
     
Duplicate are: [10, 20, 40, 30]

n=int(input("Enter the number of rows:"))
for i in range(1,n+1):
  print(i*"*")
     
Enter the number of rows:5
*
**
***
****
*****

import pandas as pd


     


     

df=pd.read_csv("pesu io.csv")
df.head()
     
Period	Revenue	Sales_quantity	Average_cost	The_average_annual_payroll_of_the_region
0	01.01.2015	16010072.12	12729.0	1257.763541	30024676.0
1	01.02.2015	15807587.45	11636.0	1358.507000	30024676.0
2	01.03.2015	22047146.02	15922.0	1384.697024	30024676.0
3	01.04.2015	18814583.29	15227.0	1235.606705	30024676.0
4	01.05.2015	14021479.61	8620.0	1626.621765	30024676.0
df. describe This command shows the first 5 rows of the dataset. The number of rows can be change by specifying the number in().


df.shape
     
(96, 5)
df. describe This command shows number of dimensions and size in each dimension ie the number of columns and number of rows.


df.count
     
<bound method DataFrame.count of         Period      Revenue  Sales_quantity  Average_cost  \
0   01.01.2015  16010072.12         12729.0   1257.763541   
1   01.02.2015  15807587.45         11636.0   1358.507000   
2   01.03.2015  22047146.02         15922.0   1384.697024   
3   01.04.2015  18814583.29         15227.0   1235.606705   
4   01.05.2015  14021479.61          8620.0   1626.621765   
..         ...          ...             ...           ...   
91  01.08.2022          NaN             NaN           NaN   
92  01.09.2022          NaN             NaN           NaN   
93  01.10.2022          NaN             NaN           NaN   
94  01.11.2022          NaN             NaN           NaN   
95  01.12.2022          NaN             NaN           NaN   

    The_average_annual_payroll_of_the_region  
0                                 30024676.0  
1                                 30024676.0  
2                                 30024676.0  
3                                 30024676.0  
4                                 30024676.0  
..                                       ...  
91                                       NaN  
92                                       NaN  
93                                       NaN  
94                                       NaN  
95                                       NaN  

[96 rows x 5 columns]>
df. describe This command shows the number of rows and columns.


df.columns
     
Index(['Period', 'Revenue', 'Sales_quantity', 'Average_cost',
       'The_average_annual_payroll_of_the_region'],
      dtype='object')
df. describe This command shows the names of all the columns in the dataset.


import pandas as pd
df=pd.read_csv("pesu io.csv")
len(df)
     
96
df.describe the command shows the number of columns.


df.info()
     
<class 'pandas.core.frame.DataFrame'>
RangeIndex: 96 entries, 0 to 95
Data columns (total 5 columns):
 #   Column                                    Non-Null Count  Dtype  
---  ------                                    --------------  -----  
 0   Period                                    96 non-null     object 
 1   Revenue                                   64 non-null     float64
 2   Sales_quantity                            64 non-null     float64
 3   Average_cost                              64 non-null     float64
 4   The_average_annual_payroll_of_the_region  64 non-null     float64
dtypes: float64(4), object(1)
memory usage: 3.9+ KB
df. describe This ccommand shows the overview of the dataset.



df.tail()
     
Period	Revenue	Sales_quantity	Average_cost	The_average_annual_payroll_of_the_region
91	01.08.2022	NaN	NaN	NaN	NaN
92	01.09.2022	NaN	NaN	NaN	NaN
93	01.10.2022	NaN	NaN	NaN	NaN
94	01.11.2022	NaN	NaN	NaN	NaN
95	01.12.2022	NaN	NaN	NaN	NaN
df. describe This command shows the last 'n' rows of the dataset.


df.size

     
480
df. describe This command shows the number of elements in the dataset


df.ndim

     
2
d. describe This command shows the dimensions of the dataset.


df.describe()
     
Revenue	Sales_quantity	Average_cost	The_average_annual_payroll_of_the_region
count	6.400000e+01	64.000000	64.000000	6.400000e+01
mean	3.236045e+07	19197.375000	1695.061159	2.869083e+07
std	1.164150e+07	6591.287257	296.844793	1.057191e+06
min	1.402148e+07	8314.000000	1110.576805	2.740647e+07
25%	2.242655e+07	15065.500000	1499.142841	2.782857e+07
50%	3.209088e+07	18368.000000	1654.399797	2.819785e+07
75%	3.992999e+07	22856.250000	1916.401095	2.987852e+07
max	5.875647e+07	38069.000000	2559.328184	3.002468e+07
Values




Distributions




2-d distributions

df. describe This command shows data like mean,percentile,standard deviation of the dataset.


df.sample()
     
Period	Revenue	Sales_quantity	Average_cost	The_average_annual_payroll_of_the_region
91	01.08.2022	NaN	NaN	NaN	NaN
df .describe This command shows a random row and column in the dataset.


df.isnull().sum()
     
Period                                       0
Revenue                                     32
Sales_quantity                              32
Average_cost                                32
The_average_annual_payroll_of_the_region    32
dtype: int64
df. desribe This commans shows the missing value in each column.


df.nunique()
     
Period                                      96
Revenue                                     64
Sales_quantity                              64
Average_cost                                64
The_average_annual_payroll_of_the_region     6
dtype: int64
df. describe This command shows number of unique entires in a row and coloumn.


df.memory_usage()
     
Index                                       128
Period                                      768
Revenue                                     768
Sales_quantity                              768
Average_cost                                768
The_average_annual_payroll_of_the_region    768
dtype: int64
df. describe This command shows the amount of memory used by each column in bytes.


df.dropna()
     
Period	Revenue	Sales_quantity	Average_cost	The_average_annual_payroll_of_the_region
0	01.01.2015	16010072.12	12729.0	1257.763541	30024676.0
1	01.02.2015	15807587.45	11636.0	1358.507000	30024676.0
2	01.03.2015	22047146.02	15922.0	1384.697024	30024676.0
3	01.04.2015	18814583.29	15227.0	1235.606705	30024676.0
4	01.05.2015	14021479.61	8620.0	1626.621765	30024676.0
...	...	...	...	...	...
59	01.12.2019	58756473.66	38069.0	1543.420464	29878525.0
60	01.01.2020	56288300.87	27184.0	2070.640850	29044998.0
61	01.02.2020	40225243.26	23509.0	1711.057181	29044998.0
62	01.03.2020	50022165.23	32569.0	1535.882748	29044998.0
63	01.04.2020	52320692.94	26615.0	1965.834790	29044998.0
64 rows × 5 columns

df. describe This command removes the row or coloumn that has missing values in it.


df.dtypes
     
Period                                       object
Revenue                                     float64
Sales_quantity                              float64
Average_cost                                float64
The_average_annual_payroll_of_the_region    float64
dtype: object
df. describe This command shows the datatype of each coloumn.


import pandas as pd
import matplotlib.pyplot as plt

data = pd.read_csv("pesu io.csv")

data['Period'] = pd.to_datetime(data['Period'], format='%d.%m.%Y')

data.fillna(0, inplace=True)

plt.figure(figsize=(12, 6))
plt.plot(data['Period'], data['Revenue'], label='Revenue', color='dodgerblue')


plt.plot(data['Period'], data['The_average_annual_payroll_of_the_region'], label='Annual Payroll', color='darkorange')

plt.xlabel('Year-Month')
plt.ylabel('Values')
plt.title('Monthly Data from 2015 to 2020')
plt.xticks(rotation=45)
plt.legend()
plt.grid(True)

plt.tight_layout()
plt.show()

     

df. describe This code shows the visual representation of the dataframe in different years.


import pandas as pd
import matplotlib.pyplot as plt

data = pd.read_csv("pesu io.csv")

data['Period'] = pd.to_datetime(data['Period'], format='%d.%m.%Y')

data.fillna(0, inplace=True)

plt.figure(figsize=(12, 6))
plt.plot(data['Period'], data['Sales_quantity'], label='Sales Quantity', color='limegreen')

plt.xlabel('Year-Month')
plt.ylabel('Values')
plt.title('Monthly Data from 2015 to 2020')
plt.xticks(rotation=45)
plt.legend()
plt.grid(True)

plt.tight_layout()
plt.show()

     


import pandas as pd
import matplotlib.pyplot as plt

data = pd.read_csv("pesu io.csv")

data['Period'] = pd.to_datetime(data['Period'], format='%d.%m.%Y')

data.fillna(0, inplace=True)

plt.figure(figsize=(12, 6))
plt.plot(data['Period'], data['Average_cost'], label='Average Cost', color='gold')

plt.xlabel('Year-Month')
plt.ylabel('Values')
plt.title('Monthly Data from 2015 to 2020')
plt.xticks(rotation=45)
plt.legend()
plt.grid(True)

plt.tight_layout()
plt.show()

     

df. describe This program plots average_cost year wise.
