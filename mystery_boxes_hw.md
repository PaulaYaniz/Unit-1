# Mystery boxes

## Exercise 1: mystery_box1 and mystery_box2
mystery_box1: If it is True all input reversed in lowecase. "Hello" and "True" into "olleh"

mystery_box1: If it is False all input reversed. "Hello" and "False" into "olleH"

mystery_box2: john.doe@gmail.com into "John Doe" and "gmail.com"
````
def mystery_box1(a, b):
  reverse = a[::-1]
  if b == "True":
    print(reverse.lower())
  else:
    print(reverse)

def mystery_box2(email):
  x = email.split("@")
  username = x[0]
  domain = x[1]
  x = username.split(".")
  name = x[0].capitalize()
  surname = x[1].capitalize()
  print(name, surname)
  print(domain)

print("mystery_box1:")
a = input()
b = input()
mystery_box1(a, b)

print("mystery_box2:")
email = input()
mystery_box2(email)
````

## Exercise 2: mystery_box3
Least Common Multiple of three integers.

8, 6, 2 to 24 ---- 18, 4, 7 to 252
````
import math

def mystery_box3(a, b, c):
  lcm = a*b//math.gcd(a, b)
  lcm = lcm*c//math.gcd(lcm, c)
  return lcm

a = int(input())
b = int(input())
c = int(input())

print(mystery_box3(a, b, c))
````

## Exercise 3: mystery_box4
[5, 6, 3, 8, 1, 7, 9] to 4.4 [5, 6, 3, 8, 1, 7]
````
def mystery_box4(x):
  m = max(x)
  s = sum(x)
  x.remove(m)
  print(round((s/m +0.1), 1))
  print(x)

mystery_box4([5, 6, 3, 8, 1, 7, 9])
````
