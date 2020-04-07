```.py
class Words:
    def __init__(self):
        self.string1 = " "

    def getString(self):
        self.string1 = input()

    def printString(self):
        print(self.string1.upper())

string1 = Words()

string1.getString()
string1.printString()
```
