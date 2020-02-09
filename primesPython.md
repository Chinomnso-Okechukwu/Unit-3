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
d represents various divisors that would be used to test the numbers.

n represents the numbers that are being tested for prime properties or not. 

The for loop iterates the values of d for a number n. The % represents the modulo operator. A result of modulo 0 indicates that d is a factor of n. So, for each value of d within the range (2, n-1), n is being divided.

This program doesn't just print out all the prime numbers but it should do so at the shortest time possible. 
```.py 
t0 = time.time()
for n in range(1, 100000):
  is_prime_v(n)
t1 = time.time()
print("Time required: ", t1-t0)
```
This code above calculates the amount of time required to print the prime results of 100000 numbers. 
In the video above, the time taken to execute the code is too long. Hence, we have to look for ways to reduce this time.

When expressing a number as the product of various two positive factors in the way such that the first factor is always increasing and the second one is always increasing, the midpoint is the expression of the multiplication of the square root of that number. The factorizations after that point are just a repetition of the factorizations before it in a reversed order. Therefore, it is more concise if we only test for divisors from 2 till the square root of n.

When dealing with square roots, we have to import the square root function (sqrt(n)) from the math module.
```.py
max_divisor = math.floor(math.sqrt(n))
for d in range(2, 1 + max_divisor):
```
math.floor rounds down the square root of the number to the nearest integer.

max_divisor is the rounded down value of the square root of n plus 1.

Now, the code only iterates values of d till the max divisor. 

This brings about a lower time execution. But is this actually the lowest possible execution time? 
We are checking for all values of n within a range but from our basic knowledge of math, we know that it is not possible for an even number to be prime as it can be divided by the number two. The only even number that is prime is two itself. Then I guess there is no point of checking prime for even numbers. 

```.py 
def is_prime_v(n):
  if n == 2 :
    return True
  if n > 2 and n % 2 == 0:
    return False

max_divisor = math.floor(sqrt(n))
for d in range(3, 1 + max_divisor, 2):
  if n % d == 0:
    return False
return True
```
Now, it only interates over odd numbers. The two at the end of the for loop indicates the step. Since we want to check all odd numbers in a given range, we need to add two to go to the next even number. 

This action has led to an even faster result than the second one.
  


