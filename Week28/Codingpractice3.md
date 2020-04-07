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
