#import all modules

import pandas as pd
import datetime as dt
from pandas_datareader import data
from matplotlib import pyplot as plt
import numpy as np
import seaborn as sns
%matplotlib inline


#get the stocks info from the yahoo website, and store them as a dataframe

stocks = data.DataReader(name = ["IBM", "ORCL", "MSFT"], data_source = "yahoo", start = "2020-10-01", end = "2020-10-20")
dates = pd.date_range(start = "2020-10-01", end = "2020-10-20", freq = "B")


stocks.head()  #show the top 5 lines of the stocks dataframe

stocks.describe()   #show the numeric details of the stocks dataframe

stocks.describe().to_csv("stocks description.csv") #output the above description info to a csv file, this description file has been uploaded to the repository.

stocks.info()  #present the info of each column in the dataframe

stocks.loc["2020-10-05": "2020-10-10", "High"]  #show the high column value of rows from 2020-10-05 to 2020-10-10

stocks.iloc[2:7, 6:9] #the same output as above, but using index locations instead of index names

np.mean(stocks["High"]["IBM"]) #get the mean of all IBM high
np.max(stocks["High"]["IBM"]) #get the max of all IBM high
np.min(stocks["High"]["IBM"]) #get the min of all IBM high
np.std(stocks["High"]["IBM"]) #get the std of all IBM high
np.sum(stocks["High"]["IBM"]) #get the sum of all IBM high
np.percentile(stocks["High"]["IBM"], 25)
np.percentile(stocks["High"]["IBM"], 75)
