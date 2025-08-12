# Ex.No: 01A PLOT A TIME SERIES DATA
###  Date: 

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
import numpy as np # linear algebra
import pandas as pd # data processing, CSV file I/O (e.g. pd.read_csv)
import seaborn as sns
import matplotlib.pyplot as plt
import warnings
warnings.filterwarnings('ignore')

df = pd.read_csv("/kaggle/input/delhi-air-quality-dataset/final_dataset.csv")
df.head()
plt.figure(figsize=(14, 6))
for col in ['PM2.5', 'PM10', 'NO2', 'SO2', 'CO', 'Ozone']:
    plt.plot(df['Date'], df[col], label=col, alpha=0.7)

plt.title('Daily Trend of Pollutants in Delhi')
plt.xlabel('Date')
plt.ylabel('Pollutant Levels')
plt.legend()
plt.tight_layout()
plt.show()

```
# OUTPUT:


<img width="1417" height="612" alt="Screenshot 2025-08-12 140908" src="https://github.com/user-attachments/assets/7aa162cc-bdcb-464d-8eca-ced4a38cf3dc" />




# RESULT:
Thus we have created the python code for plotting the time series of given data.
