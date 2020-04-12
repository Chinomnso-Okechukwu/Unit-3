This Python program generates random passwords of length 20. The user provides how many passwords should be generated

```.py
import random
import string
number = 3

def randomString(stringLength):
    characters = string.ascii_letters + string.digits
    return ''.join(random.choice(characters) for i in range(stringLength))

for i in range(1, number+1):
    print('Password {}: {}'.format(i, randomString(stringLength=20)))
    
```
