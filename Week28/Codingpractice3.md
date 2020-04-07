This program accepts a comma separated sequence of words as input and prints the words in a comma-separated sequence after sorting them alphabetically.


```.py
from string import ascii_lowercase
word = input().split(",")
text = []

for a in ascii_lowercase:
    for i in range(len(word)):
        if word[i][0] != a:
            continue
        else:
            text.append(word[i])
            
print(','.join(text))
```
