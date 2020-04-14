Using the data from the WHO about the covid virus, and the price of  gold for the month of March, create a scatter plot for the number of cases versus the price of gold. Then find the way to calculate the correlation coefficient with Python for this data. Explain the result.

```.py
import matplotlib.pyplot as pplot
import csv

from scipy.stats import spearmanr

with open('data.csv', 'r') as dt:
    data = []
    values = csv.reader(dt, delimiter=',')
    for row in values:
        data.append(row)

x = [int(d) for d in data[1]]
y = [int(d) for d in data[0]]

corr, _ = spearmanr(x, y)
print(corr,_)

pplot.plot(x, y,"-ro")
pplot.xlabel('Price of gold')
pplot.ylabel('Number of cases')
pplot.show()
```
My output values were -0.36470160676823155 & 0.04367384558365209

The first value is the correlation coefficient and another is the p-value.
The correlation coefficient is a negative value showing that there is no particular relation between two set of values.
