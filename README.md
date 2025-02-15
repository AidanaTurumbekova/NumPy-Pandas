#1 A Pandas Series object can be created from the Lists, Tuples, Dictionaries, NumPy Arrays and etc. data types.

import pandas as pd
import numpy as np

#2
s = pd.Series(np.arange(1, 13), index = ["January", "February", "March", "April", "May", "June", "July", "August", "September", "October", "November", "December"])
print(s)
