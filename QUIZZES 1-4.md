# QUIZ 001
## Given 2 numbers, A and B, Output TRUE if one of them is 20 or if their sum is 20.
Examples:

Makes20(9, 20) → TRUE

Makes20(9, 9) → FALSE

Makes20(11, 9) → TRUE

````
num1 = int(input())
num2 = int(input())

if (num1 + num2) == 20:
  print("TRUE")
elif num1 == 20 or num2 == 20:
  print("TRUE")
else:
  print("FALSE")
````

# QUIZ 002
## Given three integer values, A, B, and C, output the largest difference between any of the numbers.
Examples:

largestDistance(1, 2, 3) → 2

largestDistance(1, 3, 10) → 9

largestDistance(3, 2, 4) → 2
````
num1 = int(input())
num2 = int(input())
num3 = int(input())

dist1 = abs(num1 - num2)
dist2 = abs(num2 - num3)
dist3 = abs(num3 - num1)

m = max(dist1, dist2, dist3)
print(m)
````

# QUIZ 003
## Given an integer N, show 100 integers with the repeating pattern 0 to N-1, 0 to N-1,... 
Examples:

rangePatternN(3)   → 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2,.... (100 numbers)   → 4950

rangePatternN(5)  → 0, 1, 2, 3, 4, 0, 1, 2, 3, 4, 0, 1,.... (100 numbers)   → 4950
```
n = int(input())
a = 0

for i in range(0, 100):
  r = i % n
  print(r, end = ", ")
  a += i

print()
print(a)
```

# QUIZ 004
## Write a function that receives an integer N, and returns all its factors. 
Examples:

perfectN(6)   → [1, 2, 3]

perfectN(10)  → [1, 2, 5] 

```
def print_factors(x):
   for i in range(1, x):
       if x % i == 0:
           print(i)

num = int(input())

print_factors(num)
```
