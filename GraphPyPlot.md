import random
sum = 0
for n in range(1, 1001):
    a = random.randrange(2, 101, 1)
    print(a)
    sum += a
ave = sum / 1000
print('Sum is equal to ' + str(sum))
print('Average is equal to ' + str(ave))
