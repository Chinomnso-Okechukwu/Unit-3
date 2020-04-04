### With a given integral number n, write a program to generate a dictionary that contains (i, i*i) such that i is an integral number between 1 and n (both included). The program should print the dictionary.

```.py
a = int(input())
dict = {i:i*i for i in range(1, a+1)}
print(dict)
```
