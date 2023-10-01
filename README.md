EDA-exploratory data analysis

mae-mean absolute error-diff netween actual and predicted value .

mape:mean absolute percentage error-% of diff between actual and predicted value

mape = 0:overfitting(fitting very tightly in the date set)

underfittng













SGQ( Scenario,Gap,Quest)

scenario-stake holders roles and resoposnsibilty ,excpectation

gap- the space between the current scenario and the future

future-some % increase or decrease ,action ,outcome



holt winter model-predit next quarter

i)seasonality ,stationality - every model will have this .

ii)unique indetifiers.





i)problem statement,sgp,representation

ii)EDA

iii) MODEL,LSTM(stock market analysis to capture the final details)

iv) presentation : Tech , Non-tech







pandas functions for eda

first import pandas as pd , then df=read_csv("file_name")

i) df.head():returns the first 5 rows of data frame .To change value insert number in ().

ii) df.tail(); returns last n rows of the data frame.

iii)df.info():Quick overview of the dataset

iv)df.shape: Number of dimesnions and size in each dimension.

v)df.size:number of elements in the object.

vi) df.ndim: Returns dimesnions of the dataset.

vii)df.describe(): Statical calculations like mean ,percentile,sd etc.

viii)df.sample():Random row or column is generated.

ix)df.isnul().sum(): Returns the missing value in each column

x)df.nunique():Counts number of unique entries in any row or column.

xi)df.index: This function searches for a given element from the start of the list and returns the lowest index where the element appears.

xii)df.columns: Return the column labels of the dataframe.

xiii)df.memory_usage( ): Returns how much memory each column uses in bytes.

xiv)df.dropna( ): This function is used to remove a row or a column from a dataframe that has a NaN or missing values in it.

xv)df.nlargest( ): Returns the first n rows ordered by columns in descending order.

xvi)df.isna( ): This function returns a dataframe filled with boolean values with true indicating missing values.

xvii)value_counts( ): This function is used to get a Series containing counts of unique values.

ix)df.corr( ): This function is used to find the pairwise correlation of all columns in the dataframe.

xx)df.dtypes: This function shows the data type of each column.



hypothetical testing - consists of 2 ( null hypothesis H0 and alt hypothesis H1) 

z testing - for more than 30 values  

t testing - for less than 30 values

khi ^2 - for qualitative dataset

anova - analysis of variance 

	

seasonality: preditcatble data

stationality: cannot be predicted,p<0.05(after running adf test)

adf test,kpss test

Why two diff tests?

 



data prepossesing - length columns name unique values

descriptive anaylisis - null values , outliers,box plots, inference,
