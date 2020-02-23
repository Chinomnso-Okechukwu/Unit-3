### Even indices
This program, given a list of numbers, find and print all the list elements with an even index number(i.e. A[0], A[2], A[4], ...).
```.py
a = input().split() #puts inputs into list of strings
for i in range(0, len(a), 2): #gets even numbers
    print(a[i])
```

### Even elements
Given a list of numbers, find and print all elements that are an even number. In this case use a for-loop that iterates over the list, and not over its indices! 
That is, don't use range()
```.py
a = [int(i) for i in input().split()]
for i in a:
    if i % 2 == 0:
        print(i)
```

### Greater than previous
Given a list of numbers, find and print all the elements that are greater than the previous element.
```.py
a = input().split()
for i in range(1, len(a)):
    if int(a[i - 1]) < int(a[i]):
        print(a[i])
```

### Neighbors of the same sign
Given a list of numbers, find and print the first adjacent elements which have the same sign. If there is no such pair, leave the output blank.
```.py
a = [int(i) for i in input().split()]
for i in range(1, len(a)):
    if a[i-1] * a[i] > 0:
        print(a[i-1], a[i])
        break
```

### Greater than neighbours
Given a list of numbers, determine and print the quantity of elements that are greater than both of their neighbors.
The first and the last items of the list shouldn't be considered because they don't have two neighbors.
```.py
a = [int(i) for i in input().split()]
count = 0
for i in range(1, len(a)-1):
    if a[i] > a[i-1] and a[i] > a[i+1]:
        count += 1
print(count)
```
      
