# Lesson 2: Integer and float numbers

## Last digit of integer
Given an integer number, print its last digit.
```
n = int(input())

print(n%10)
```

## Tens digit
Given an integer. Print its tens digit.
```
n = int(input())

print(n//10%10)
```

## Sum of digits
Given a three-digit number. Find the sum of its digits.
```
n = int(input())

n1 = n//100
n2 = n//10%10
n3 = n%10

print(n1+n2+n3)
```

## Fractional part
Given a positive real number, print its fractional part.
```
n = float(input())

print(n - int(n))
```

## First digit after decimal point
Given a positive real number, print its first digit to the right of the decimal point.
```
n = float(input())

print(n*10%10//1)
```

## Car route
A car can cover distance of N kilometers per day. How many days will it take to cover a route of length M kilometers? The program gets two numbers: N and M.
```
from math import ceil

n = int(input())
m = int(input())

print(ceil(m/n))
```

## Digital clock
Given the integer N - the number of minutes that is passed since midnight - how many hours and minutes are displayed on the 24h digital clock?
The program should print two numbers: the number of hours (between 0 and 23) and the number of minutes (between 0 and 59).
For example, if N = 150, then 150 minutes have passed since midnight - i.e. now is 2:30 am. So the program should print 2 30.
```
n = int(input())

h = int(n/60)
m = int(n%60)

print(h, m)
```

## Total cost
A cupcake costs A dollars and B cents. Determine, how many dollars and cents should one pay for N cupcakes. A program gets three numbers: A, B, N. It should print two numbers: total cost in dollars and cents.
```
a = int(input())
b = int(input())
n = int(input())

d = a*n
d2 = b*n // 100
c = (b*n) % 100

print(d+d2, c)
```

## Clock face - 1
H hours, M minutes and S seconds are passed since the midnight (0 ≤ H < 12, 0 ≤ M < 60, 0 ≤ S < 60). Determine the angle (in degrees) of the hour hand on the clock face right now.
```
h = int(input())
m = int(input())
s = int(input())

st = h*3600 + m*60 + s

a = (st*360) / (3600*12)
print(a)
```

## Clock face - 2
Hour hand turned by α degrees since the midnight. Determine the angle by which minute hand turned since the start of the current hour. Input and output in this problems are floating-point numbers.
```
a = float(input())

a = a%30

x = (a*360) / 30
print(x)
```
