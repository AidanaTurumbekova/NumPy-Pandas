#1 A Pandas Series object can be created from the Lists, Tuples, Dictionaries, NumPy Arrays and etc. data types.
import pandas as pd
import numpy as np

#2
s = pd.Series(np.arange(1, 13), index = ["January", "February", "March", "April", "May", "June", "July", "August", "September", "October", "November", "December"])
print(s)

#3
students_number = {"MatMIE" : 40, "MatDAIS" : 36, "COMIE" : 45, "COMCE" : 45}
print(pd.Series(students_number))
