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
### Program to print any other mathematical function
