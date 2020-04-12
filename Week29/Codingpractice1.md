Write a Python program that asks the user for his first name and last name and a number (1, 100]. The output is a text file with as email addresses for the user:

```.py
firstname = input()
lastname = input()
number = int(input())

for i in range(1,number+1):
    print('{}.{}{}@uwcisak.jp'.format(firstname,lastname,i))
```
