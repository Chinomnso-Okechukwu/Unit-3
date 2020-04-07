This class has two methods: 

getString: to get a string from console input
printString: to print the string in upper case.


```.py
class Words:
    def __init__(self):
        self.firststring = " "

    def getString(self):
        self.firststring = input()

    def printString(self):
        print(self.firststring.upper())

firststring = Words()

firststring.getString()
firststring.printString()
```
