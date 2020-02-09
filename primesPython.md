## The code prints out all the prime numbers within a given range at the shortest time possible.
A prime number is a number that is divisible by 1 and itself only.

The first step is to define the function for prime numbers.
```.py
def is_prime_v1(n):
if n == 1:
  return False # 1 is not prime
for d in range(2, n-1):
        if n % d == 0:
            return False
    return True
```
