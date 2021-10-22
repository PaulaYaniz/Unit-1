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
Examples

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
