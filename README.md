# Ex.No: 01A PLOT A TIME SERIES DATA
###  Date: 12/08/2025

# AIM:
To Develop a python program to Plot a time series data (population/ market price of a commodity
/temperature.
# ALGORITHM:
1. Import the required packages like pandas and matplot
2. Read the dataset using the pandas
3. Calculate the mean for the respective column.
4. Plot the data according to need and can be altered monthly, or yearly.
5. Display the graph.
# PROGRAM:
```

import numpy as np 
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

df=pd.read_csv('/content/BMW_Car_Sales_Classification.csv')
df

df.info()

df.isnull().sum()

df.dtypes

target = 'Year'

sns.set(style="whitegrid")
plt.rcParams["figure.figsize"] = (10, 6)

plt.figure()
sns.countplot(x=target, data=df, palette='pastel')
plt.title('Target Class Distribution')
plt.xlabel(target)
plt.ylabel('Count')
plt.show()


```
# OUTPUT:
<img width="1398" height="516" alt="Screenshot 2025-08-12 134933" src="https://github.com/user-attachments/assets/a58d301e-5065-4258-ae90-a68ba85f66f2" />
<img width="537" height="406" alt="Screenshot 2025-08-12 134948" src="https://github.com/user-attachments/assets/dab24ebf-6f99-48c3-aaff-3611e146ba01" />

<img width="338" height="534" alt="Screenshot 2025-08-12 134958" src="https://github.com/user-attachments/assets/3aa4a850-8273-4257-bb13-b1dd7d12325d" />
<img width="1184" height="665" alt="Screenshot 2025-08-12 135043" src="https://github.com/user-attachments/assets/72b049d8-a006-4ac3-ad02-b7b3a0962a0d" />







# RESULT:
Thus we have created the python code for plotting the time series of given data.
