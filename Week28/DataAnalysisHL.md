This program gets the inputs(total number of corona cases in the world, number of days and total number of cases in Nigeria) from a .csv file and plots the graph of total world cases by number of days and total Nigeria cases by number of days.

```.py
import matplotlib.pyplot as pyplot
import csv

with open('covid.csv') as cd:
    data = []
    cases = csv.reader(cd, delimiter=",")
    for row in cases:
        data.append(row)
    print(data)

#number of days
x1 = data[1]
y1 = data[2]
pyplot.plot(x1, y1)
x2 = data[1]
y2 = data[2]
pyplot.plot(x2, y2)
pyplot.xlabel("number of days")
pyplot.ylabel("number of cases")
pyplot.show()
```


```.py
282, 314, 581, 846, 1320, 2014, 2798, 4593, 6065, 7818, 9826, 11953, 14557, 17391, 20630, 24544, 28276, 31481, 34886, 37558, 40554, 43103, 45171, 46997, 49053, 50580, 51857, 71429, 73332, 75204, 75748, 76769, 77794, 78811, 79331, 80239, 81109, 82294, 83652, 85403, 87137, 88948, 90869, 93090, 95324, 98192, 101927, 105592, 109577, 113702, 118319, 125260, 132758, 142534, 153517, 167506, 179112
1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31, 32, 33, 34, 35, 36, 37, 38, 39, 40, 41, 42, 43, 44, 45, 46, 47, 48, 49, 50, 51, 52, 53, 54, 55, 56, 57
0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2,
```
This is the .csv file that shows the:

number of world cases of covid-19 in row 1.

number of days in row 2.

number of cases in Nigeria in row 3.


