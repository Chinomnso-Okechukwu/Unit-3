## String Practice
```.py
from functools import reduce

file = open("text.txt", "r")

extract = file.read()

print(extract)

words = extract.split()
print("number of words is {}".format(len(words)))


keywords = ['house', 'worker', 'master', 'hard', 'responsible', 'skillful']
for key in keywords:
    print("Checking word "+key+" in the text: found?")
    print(key in words)

lengthOfText = len(extract)
# using C thinking
num_letters = 0
for symbol in extract:
    if symbol.isalpha():
        num_letters += 1

print(f'There are {num_letters} out of {lengthOfText} total characters')

print(extract.lower())

long_words = '#'.join(list(filter(lambda a: len(a)>5, words)))
print(long_words)

for word in words:
    if len(word) > 5:
        print('#' + word)

totalSum = 0
for l in extract:
    totalSum += ord(l)
print(totalSum)

totalSum = reduce(lambda a,b : a+b, [ord(e) for e in extract])
print(totalSum)
```
     
