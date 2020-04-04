### This Python program accepts a string and calculates the number of digits and letters. 
```.py
a = input()
length = len(a)
digit = 0
letters = 0

for i in range(len(a)):
    if a[i].isalpha():
            letters += 1
    elif a[i].isnumeric():
            digit += 1
print('Letters {}'.format(letters))
print('Digits {}'.format(digit))
```
