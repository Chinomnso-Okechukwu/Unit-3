### This Python program calculates a dog's age in dog's years.
Note: For the first two years, a dog year is equal to 10.5 human years. After that, each dog year equals 4 human years.

```.py
a = int(input())

if a <= 2:
    age = a * 10.5
elif a > 2:
    age = 2 * 10.5 + (a-2) * 4
print(age)
```
