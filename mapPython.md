### Understanding the map function

The map function helps to reduce lines of code into just one single line.

The map function takes two arguments. The first argument is the function while the second one is the iterable object.
 
In order for the map function to work, first specify your data list then define the function to be applied to each data values. This is shown in the code snippet below.
```.py
import math
def area(r):
  """Area of a circle with radius 'r'."""
  return math.pi * (r**2)
radii = [2, 5, 7.1, 0.3, 10]
```

Under the bracket of the map function, first specify the data list, then the data list.
```.py
Data: 
Function:
map(f, data)
```
To print out the results in a list, we use the list function as shown below.
```.py
list(map(f, data))
```
