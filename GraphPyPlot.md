### Program to print 100 random numbers and their average
```.py
 import random
 sum = 0
 for n in range(1, 1001):
    a = random.randrange(2, 101, 1)
    print(a)
    sum += a
 ave = sum / 1000
 print('Sum is equal to ' + str(sum))
 print('Average is equal to ' + str(ave))
```

### Program to graph the function 14sin(0.5x)
```.py
import math
import matplotlib.pyplot
x = [i for i in range(-10, 10)
y = [14*math.sin(0.5*x) for i in x]

pyplot.plot(x, y)
pyplot.xlabel("x")
pyplot.ylabel("$y = 14*math.sin(0.5*x)$")
pyplot.show()
```
### Program to print any other mathematical function with a different method
The function is y= cos(0.5x) and z=cos(0.5x)
```.py
step = 0.01
x = []
for points in range(2000):
    x.append(-10+step*(points))
y = [math.sin(0.5*i) for i in x]
z = [math.cos(0.5*i) for i in x]

pyplot.plot(y,z)
pyplot.xlabel("$y = math.sin(0.5*i)$"]
pyplot.ylabel("$z = math.cos(0.5*i)$"]
pyplot.show()
```
