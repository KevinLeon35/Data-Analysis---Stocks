#import all modules

import pandas as pd
import datetime as dt
from pandas_datareader import data
from matplotlib import pyplot as plt
import numpy as np
import seaborn as sns
%matplotlib inline

#use matplotlib to show a line chart to present the high and low price of the IBM stock


plt.figure(figsize = (15,10))  #create a new figure
plt.plot(stocks["High"]["IBM"], color = "Green", label = "High")  # plot the line of IBM stock high price, x axis is date
plt.plot(stocks["Low"]["IBM"], color = "Red", label = "Low", linestyle = "--") # plot the line of IBM stock low price.
plt.xlabel("Date")
plt.ylabel("Dollars")
plt.title("high and low price of IBM stocks")
plt.legend(loc = 6) #location of the legend
plt.savefig("IBM stock high and low prices - October.jpg") #This line chart jpg has been uploaded to the repository.

#use a pie chart to compare the high of each stocks on 2020-10-01

plt.figure(figsize = (15,10))  #create a new figure
plt.pie(stocks.loc["2020-10-01", "High"], labels = ["IBM", "ORCL", "MSFT"], autopct='%0.1f%%')
plt.savefig("IBM stock high Pie chart.jpg")  ##This pie chart jpg file has been uploaded to the repository.


plt.hist(stocks["High"]["ORCL"], bins = 20)
