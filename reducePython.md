### Reduce function in Python
```.py
reduce(f, data):
  Step 1: val1 = f(a1,a2)
  Step 2: val2 = f(val1, a3)
  Step 3: val3 = f(val2, a4)
  .
  .
  .
  Step n-1: val(n-1) = f(valn-2, an)
  return val(n-1)
  
print ("The sum of the list elements is : ",end="") 
print (functools.reduce(lambda a1,f : a1+a2,f)) 
  ```
  
  To use the reduced function, we need to import it from functools.
