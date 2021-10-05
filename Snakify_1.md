# Lesson 1: Input, print and numbers

## Sum of three numbers
Write a program that takes three numbers and prints their sum. Every number is given on a separate line.
```
a = int(input())
b = int(input())
c = int(input())

print(a + b + c)
```

## Hi John
Write a program that greets the person by printing the word "Hi" and the name of the person. See the examples below.
```
name = input()

print("Hi " + name)
```

## Square
Write a program that takes a number and print its square.
```
a = int(input())

print(a*a)
```

## Area of right-angled triangle
Write a program that reads the length of the base and the height of a right-angled triangle and prints the area. Every number is given on a separate line.
```
b = int(input())
h = int(input())

print(b*h/2)
```

## Hello, Harry!
Write a program that greets the user by printing the word "Hello", a comma, the name of the user and an exclamation mark after it. See the examples below.
```
name = input()

print('Hello,', name+'!')
```

## Apple sharing
N students take K apples and distribute them among each other evenly. The remaining (the undivisible) part remains in the basket. How many apples will each single student get? How many apples will remain in the basket?
The program reads the numbers N and K. It should print the two answers for the questions above.
```
n = int(input())
k = int(input())

print(k // n)
print(k % n)
```

## Previous and next
Write a program that reads an integer number and prints its previous and next numbers. See the examples below for the exact format your answers should take. There shouldn't be a space before the period.
Remember that you can convert the numbers to strings using the function str.
```
a = int(input())
n = str(a+1)
p = str(a-1)

print("The next number for the number", a, "is", n + ".")
print("The previous number for the number", a, "is", p + ".")
```

## Two timestamps
A timestamp is three numbers: a number of hours, minutes and seconds. Given two timestamps, calculate how many seconds is between them. The moment of the first timestamp occurred before the moment of the second timestamp.
```
h1 = int(input())
m1 = int(input())
s1 = int(input())

h2 = int(input())
m2 = int(input())
s2 = int(input())

t1 = h1 * 3600 + m1 * 60 + s1
t2 = h2 * 3600 + m2 * 60 + s2

print(t2 - t1)
```

## School desks
A school decided to replace the desks in three classrooms. Each desk sits two students. Given the number of students in each class, print the smallest possible number of desks that can be purchased.
The program should read three integers: the number of students in each of the three classes, a, b and c respectively.
In the first test there are three groups. The first group has 20 students and thus needs 10 desks. The second group has 21 students, so they can get by with no fewer than 11 desks. 11 desks is also enough for the third group of 22 students. So we need 32 desks in total.

```
c1 = int(input())
c2 = int(input())
c3 = int(input())

print(c1//2 + c2//2 + c3//2 + c1%2 + c2%2 + c3%2)
```

