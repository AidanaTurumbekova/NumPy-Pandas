#1 A Pandas Series object can be created from the Lists, Tuples, Dictionaries, NumPy Arrays and etc. data types.
import pandas as pd
import numpy as np

#2
s = pd.Series(np.arange(1, 13), index = ["January", "February", "March", "April", "May", "June", "July", "August", "September", "October", "November", "December"])
print(s)

#3
students_number = {"MatMIE" : 40, "MatDAIS" : 36, "COMIE" : 45, "COMCE" : 45}
print(pd.Series(students_number))

exam_data = {'name':["Anastasia", "Dima", "Katherine", "James", "Emily", "Michael", "Matthew", "Laura", "Kevin", "Jonas"], 'score': [12.5, 9, 16.5, np.nan, 9, 20, 14.5, np.nan, 8, 19],
'attempts': [1, 3, 2, 3, 2, 3, 1, 1, 2, 1],
'qualify': ['yes', 'no', 'yes', 'no', 'no', 'yes', 'yes', 'no', 'no', 'yes']} 

exam = pd.DataFrame(exam_data)
exam.index = ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j']
print(exam)

