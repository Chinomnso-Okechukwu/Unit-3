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
### Program to graph another mathematical function with a different method
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
### Program to graph another function with a different method.
```.py
min_x = -10                                 
max_x = 500                                 
step = 0.01                                 
num_points = int((max_x - min_x)/step)      
                                            
x_axis = list()                             
for p in range(num_points):                 
    x_axis.append(min_x + step*p)           
print(x_axis)                               
                                            
# y = sin(0.5x)                             
y = [math.sin(0.5*n) for n in x_axis]       
y = list()                                  
w = list()                                  
am = list()                                 
for n in x_axis:                            
    y.append(math.sin(0.5*n))               
    w.append(0.1*math.sin(0.05*n))          
    am.append(y[-1] + w[-1])                
                                            
pyplot.plot(x_axis, am)                     
pyplot.xlabel("x_axis")                     
pyplot.ylabel("am")                         
pyplot.show() 
```
