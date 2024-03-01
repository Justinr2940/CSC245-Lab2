​​1. Write a Pandas program to create and display a one-dimensional array-like object containing an array of data using Pandas module.


2. Write a Pandas program to convert a Panda module Series to Python list and it's type.


3. Write a Pandas program to add, subtract, multiple and divide two Pandas Series.
Sample Series: [2, 4, 6, 8, 10], [1, 3, 5, 7, 9]


4. Write a Pandas program to compare the elements of the two Pandas Series.
Sample Series: [2, 4, 6, 8, 10], [1, 3, 5, 7, 10]


5. Write a Pandas program to convert a dictionary to a Pandas series. 

Sample Series: 

Original dictionary:

{'a': 100, 'b': 200, 'c': 300, 'd': 400, 'e': 800}



Converted series:

a    100

b    200

c    300

d    400

e    800

dtype: int64



6. Write a Pandas program to convert a NumPy array to a Pandas series. 

Sample Series: 

  NumPy array:

[10 20 30 40 50]

Converted Pandas series:

0    10

1    20

2    30

3    40

4    50

dtype: int64 




7. Write a Pandas program to change the data type of given a column or a Series. 

Sample Series: 

    Original Data Series:

0       100

1       200

2    python

3    300.12

4       400

dtype: object

Change the said data type to numeric:

0    100.00

1    200.00

2       NaN

3    300.12

4    400.00

dtype: float64




8. Write a Pandas program to convert the first column of a DataFrame as a Series. 

Original DataFrame

   col1  col2  col3

0     1     4     7

1     2     5     5

2     3     6     8

3     4     9    12

4     7     5     1

5    11     0    11



1st column as a Series:

0     1

1     2

2     3

3     4

4     7

5    11

Name: col1, dtype: int64

<class 'pandas.core.series.Series'>




9. Write a Pandas program to convert a given Series to an array. 

Sample Output: 

Original Data Series:

0       100

1       200

2    python

3    300.12

4       400

dtype: object

Series to an array

['100' '200' 'python' '300.12' '400']

<class 'numpy.ndarray'>





1.Write a Pandas program to create a dataframe from a dictionary and display it.
Sample data: {'X':[78,85,96,80,86], 'Y':[84,94,89,83,86],'Z':[86,97,96,72,83]}

Expected Output:

    X   Y   Z                                                         

0  78  84  86                                                        

1  85  94  97                                                         

2  96  89  96                                                      

3  80  83  72                                                         

4  86  86  83 




2. Write a Pandas program to create and display a DataFrame from a specified dictionary data which has the index labels.
Sample Python dictionary data and list labels:
exam_data = {'name': ['Anastasia', 'Dima', 'Katherine', 'James', 'Emily', 'Michael', 'Matthew', 'Laura', 'Kevin', 'Jonas'],
'score': [12.5, 9, 16.5, np.nan, 9, 20, 14.5, np.nan, 8, 19],
'attempts': [1, 3, 2, 3, 2, 3, 1, 1, 2, 1],
'qualify': ['yes', 'no', 'yes', 'no', 'no', 'yes', 'yes', 'no', 'no', 'yes']}
labels = ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j']

Expected Output:

   attempts       name qualify  score                              

a         1  Anastasia     yes   12.5                                 

b         3       Dima      no    9.0                                 

....                              

i         2      Kevin      no    8.0                                

j         1      Jonas     yes   19.0




3. Write a Pandas program to display a summary of the basic information about a specified DataFrame and its data.
Sample Python dictionary data and list labels:
exam_data = {'name': ['Anastasia', 'Dima', 'Katherine', 'James', 'Emily', 'Michael', 'Matthew', 'Laura', 'Kevin', 'Jonas'],
'score': [12.5, 9, 16.5, np.nan, 9, 20, 14.5, np.nan, 8, 19],
'attempts': [1, 3, 2, 3, 2, 3, 1, 1, 2, 1],
'qualify': ['yes', 'no', 'yes', 'no', 'no', 'yes', 'yes', 'no', 'no', 'yes']}
labels = ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j']

Expected Output:

  Summary of the basic information about this DataFrame and its data:

<class 'pandas.core.frame.DataFrame'>

Index: 10 entries, a to j

Data columns (total 4 columns):

....

dtypes: float64(1), int64(1), object(2)

memory usage: 400.0+ bytes

None 



4. Write a Pandas program to get the first 3 rows of a given DataFrame.
Sample Python dictionary data and list labels:
exam_data = {'name': ['Anastasia', 'Dima', 'Katherine', 'James', 'Emily', 'Michael', 'Matthew', 'Laura', 'Kevin', 'Jonas'],
'score': [12.5, 9, 16.5, np.nan, 9, 20, 14.5, np.nan, 8, 19],
'attempts': [1, 3, 2, 3, 2, 3, 1, 1, 2, 1],
'qualify': ['yes', 'no', 'yes', 'no', 'no', 'yes', 'yes', 'no', 'no', 'yes']}
labels = ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j']

Expected Output:

First three rows of the data frame:                                   

   attempts       name qualify  score                              

a         1  Anastasia     yes   12.5                                 

b         3       Dima      no    9.0                                 

c         2  Katherine     yes   16.5




5. Write a Pandas program to select the 'name' and 'score' columns from the following DataFrame.
Sample Python dictionary data and list labels:
exam_data = {'name': ['Anastasia', 'Dima', 'Katherine', 'James', 'Emily', 'Michael', 'Matthew', 'Laura', 'Kevin', 'Jonas'],
'score': [12.5, 9, 16.5, np.nan, 9, 20, 14.5, np.nan, 8, 19],
'attempts': [1, 3, 2, 3, 2, 3, 1, 1, 2, 1],
'qualify': ['yes', 'no', 'yes', 'no', 'no', 'yes', 'yes', 'no', 'no', 'yes']}
labels = ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j']

Expected Output:

Select specific columns:                                               

        name  score                                                  

a  Anastasia   12.5                                                   

b       Dima    9.0                                                

c  Katherine   16.5                                                    

...                                                  

h      Laura    NaN                                                   

i      Kevin    8.0                                                  

j      Jonas   19.0




6. Write a Pandas program to select the specified columns and rows from a given data frame.
Sample Python dictionary data and list labels:
Select 'name' and 'score' columns in rows 1, 3, 5, 6 from the following data frame.
exam_data = {'name': ['Anastasia', 'Dima', 'Katherine', 'James', 'Emily', 'Michael', 'Matthew', 'Laura', 'Kevin', 'Jonas'],
'score': [12.5, 9, 16.5, np.nan, 9, 20, 14.5, np.nan, 8, 19],
'attempts': [1, 3, 2, 3, 2, 3, 1, 1, 2, 1],
'qualify': ['yes', 'no', 'yes', 'no', 'no', 'yes', 'yes', 'no', 'no', 'yes']}
labels = ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j']

Expected Output:

Select specific columns and rows:

   score qualify

b    9.0      no

d    NaN      no

f   20.0     yes

g   14.5     yes




7. Write a Pandas program to select the rows where the number of attempts in the examination is greater than 2.
Sample Python dictionary data and list labels:
exam_data = {'name': ['Anastasia', 'Dima', 'Katherine', 'James', 'Emily', 'Michael', 'Matthew', 'Laura', 'Kevin', 'Jonas'],
'score': [12.5, 9, 16.5, np.nan, 9, 20, 14.5, np.nan, 8, 19],
'attempts': [1, 3, 2, 3, 2, 3, 1, 1, 2, 1],
'qualify': ['yes', 'no', 'yes', 'no', 'no', 'yes', 'yes', 'no', 'no', 'yes']}
labels = ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j']

Expected Output:

Number of attempts in the examination is greater than 2:

      name  score  attempts qualify

b     Dima    9.0         3      no

d    James    NaN         3      no

f  Michael   20.0         3     yes



8. Write a Pandas program to count the number of rows and columns of a DataFrame.
Sample Python dictionary data and list labels:
exam_data = {'name': ['Anastasia', 'Dima', 'Katherine', 'James', 'Emily', 'Michael', 'Matthew', 'Laura', 'Kevin', 'Jonas'],
'score': [12.5, 9, 16.5, np.nan, 9, 20, 14.5, np.nan, 8, 19],
'attempts': [1, 3, 2, 3, 2, 3, 1, 1, 2, 1],
'qualify': ['yes', 'no', 'yes', 'no', 'no', 'yes', 'yes', 'no', 'no', 'yes']}
labels = ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j']

Expected Output:

Number of Rows: 10                                                    

Number of Columns: 4



9. Write a Pandas program to select the rows where the score is missing, i.e. is NaN.
Sample Python dictionary data and list labels:
exam_data = {'name': ['Anastasia', 'Dima', 'Katherine', 'James', 'Emily', 'Michael', 'Matthew', 'Laura', 'Kevin', 'Jonas'],
'score': [12.5, 9, 16.5, np.nan, 9, 20, 14.5, np.nan, 8, 19],
'attempts': [1, 3, 2, 3, 2, 3, 1, 1, 2, 1],
'qualify': ['yes', 'no', 'yes', 'no', 'no', 'yes', 'yes', 'no', 'no', 'yes']}
labels = ['a', 'b', 'c', 'd', 'e', 'f', 'g', labels = ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j']

Expected Output:

Rows where score is missing:

   attempts   name qualify  score

d         3  James      no    NaN

h         1  Laura      no    NaN




10. Write a Pandas program to select the rows the score is between 15 and 20 (inclusive).
Sample Python dictionary data and list labels:
exam_data = {'name': ['Anastasia', 'Dima', 'Katherine', 'James', 'Emily', 'Michael', 'Matthew', 'Laura', 'Kevin', 'Jonas'],
'score': [12.5, 9, 16.5, np.nan, 9, 20, 14.5, np.nan, 8, 19],
'attempts': [1, 3, 2, 3, 2, 3, 1, 1, 2, 1],
'qualify': ['yes', 'no', 'yes', 'no', 'no', 'yes', 'yes', 'no', 'no', 'yes']}
labels = ['a', 'b', 'c', 'd', 'e', 'f', 'g', labels = ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j']

