# Lesson 4: For loop with range

## Series - 1
Given two integers A and B (A ≤ B). Print all numbers from A to B inclusively.
```
a = int(input())
b = int(input())

for i in range(a, b+1):
    print(i)
```

## Series - 2
Given two integers A and B. Print all numbers from A to B inclusively, in ascending order, if A < B, or in descending order, if A ≥ B.
```
a = int(input())
b = int(input())

if a<=b:
    for i in range(a, b+1):
        print(i)
else:
    for i in range(a, b-1, -1):
        print(i)
```

## Sum of ten numbers
10 numbers are given in the input. Read them and print their sum. Use as few variables as you can.
```
x = 0

for i in range (0,10):
    y = int(input())
    x += y
print(x)
```

## Sum of N numbers
N numbers are given in the input. Read them and print their sum.
The first line of input contains the integer N, which is the number of integers to follow. Each of the next N lines contains one integer. Print the sum of these N integers.
```
x = 0
N = int(input())

for i in range(N):
    x += int(input())
print(x)
```

## Sum of cubes
For the given integer N calculate the following sum:
1^3+2^3+…+N^3
```
N = int(input())
sum = 0

for i in range (1, N+1):
    sum += i**3
    
print(sum)
```

## Factorial
In mathematics, the factorial of an integer n, denoted by n! is the following product:
n!=1×2×…×n
For the given integer n calculate the value n!. Don't use math module in this exercise.
```
n = int(input())
factorial = 1

for i in range (1, n+1):
    factorial *= i
print(factorial)
```

## The number of zeros
Given N numbers: the first number in the input is N, after that N integers are given. Count the number of zeros among the given integers and print it.
You need to count the number of numbers that are equal to zero, not the number of zero digits.
```
count = 0

for i in range(int(input())):
    if int(input()) == 0:
        count += 1 
print(count)
```

## Adding factorials
Given an integer n, print the sum 1!+2!+3!+...+n!.
This problem has a solution with only one loop, so try to discover it. And don't use the math library :)
```
n = int(input())
factorial = 1
total = 0

for i in range (1, n+1):
    factorial *= i
    total += factorial
print(total)
```

## Ladder
For given integer n ≤ 9 print a ladder of n steps. The k-th step consists of the integers from 1 to k without spaces between them.
To do that, you can use the sep and end arguments for the function print().
```
n = int(input())

for i in range(1, n+1):
    for x in range(1, i+1):
        print(x, sep='', end='')
    print()
```

## Lost card
There was a set of cards with numbers from 1 to N. One of the card is now lost. Determine the number on that lost card given the numbers for the remaining cards.
Given a number N, followed by N − 1 integers - representing the numbers on the remaining cards (distinct integers in the range from 1 to N). Find and print the number on the lost card.
```
N = int(input())

result = 0
for i in range(1, N+1):
    result += i

nums = 0
for i in range(1, N):
    num = int(input())
    nums += num

print(result-nums)
```
