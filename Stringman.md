## String Practice
Read and use the following extract from the book “The Pragmatic Programmer: From Journeyman to Master by Andrew Hunt, David Thomas” as your text under analysis.

“What Makes a Pragmatic Programmer? Each developer is unique, with individual strengths and weaknesses, preferences and dislikes. Over time, each will craft his or her own personal environment. That environment will reflect the programmer's individuality just as forcefully as his or her hobbies, clothing, or haircut. However, if you're a Pragmatic Programmer, you'll share many of the following characteristics: Early adopter/fast adapter. You have an instinct for technologies and techniques, and you love trying things out. When given something new, you can grasp it quickly and integrate it with the rest of your knowledge. Your confidence is born of experience. Inquisitive. You tend to ask questions. That's neat—how did you do that? Did you have problems with that library? What's this BeOS I've heard about? How are symbolic links implemented? You are a pack rat for little facts, each of which may affect some decision years from now. Critical thinker. You rarely take things as given without first getting the facts. When colleagues say "because that's the way it's done," or a vendor promises the solution to all your problems, you smell a challenge. Realistic. You try to understand the underlying nature of each problem you face. This realism gives you a good feel for how difficult things are, and how long things will take. Understanding for yourself that a process should be difficult or will take a while to complete gives you the stamina to keep at it. Jack of all trades. You try hard to be familiar with a broad range of technologies and environments, and you work to keep abreast of new developments.“

① Create a program in Python that counts the number of words in the text.

② Create a small program program that check if any of the following words are in the text.
house
worker
master
hard
responsible
skillful

③ Use a f string to show a message indicating the number of letters out of the total number of characters. Ex: “in this text there are 10 letters out of a total of 100 characters.”

④ Make the text all lowercase.

⑤ Use the join method to print all the words in the text longer than 5 characters with a # appended at the beginning. Ex. #makes

⑥ Calculate the total addition of all the numeric codes for the letters in the text.

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
     
