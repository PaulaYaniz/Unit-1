# Lesson 5: Strings

## Slices
You are given a string.
In the first line, print the third character of this string.
In the second line, print the second to last character of this string.
In the third line, print the first five characters of this string.
In the fourth line, print all but the last two characters of this string.
In the fifth line, print all the characters of this string with even indices (remember indexing starts at 0, so the characters are displayed starting with the first).
In the sixth line, print all the characters of this string with odd indices (i.e. starting with the second character in the string).
In the seventh line, print all the characters of the string in reverse order.
In the eighth line, print every second character of the string in reverse order, starting from the last one.
In the ninth line, print the length of the given string.
```
S = input()

print(S[2])
print(S[1:])
print(S[:5])
print(S[:-2])
print(S[0::2])
print(S[1::2])
print(S[::-1])
print(S[::-2])
print(len(S))

# I think that the solution given by snakify is incorrect, there's an error on the second line. 
```

## The number of words
Given a string consisting of words separated by spaces. Determine how many words it has. To solve the problem, use the method count.
```
S = input()
N = S.count(' ') + 1

print(N)
```

## The two halves
Given a string. Cut it into two "equal" parts (If the length of the string is odd, place the center character in the first string, so that the first string contains one more characther than the second). Now print a new string on a single row with the first and second halfs interchanged (second half first and the first half second)
Don't use the statement if in this task.
```
from math import ceil

s = input()

n = s.count('') - 1

p = ceil(n / 2)

a = (s[p:])
b = (s[:p])

print(a+b)
```

## To swap the two words
Given a string consisting of exactly two words separated by a space. Print a new string with the first and second word positions swapped (the second word is printed first).
This task should not use loops and if.
```
s = input()

n = s.find(' ')

p = int(n)

a = (s[p::])

b = (s[:p])

print(a, b)
```

## The first and last occurrence
Given a string that may or may not contain a letter of interest. Print the index location of the first and last appearance of f. If the letter f occurs only once, then output its index. If the letter f does not occur, then do not print anything.
Don't use loops in this task.
```
s = input()
a = s.find('f')
b = s.rfind('f')

if a >= 0:
    print(a)
    if a != b:
        print(b)
```

## The second occurrence
Given a string that may or may not contain the letter of interest. Print the index location of the second occurrence of the letter f. If the string contains the letter f only once, then print -1, and if the string does not contain the letter f, then print -2.
```
s = input()
a = s.find('f')
b = s.find('f', a+1)

if a == -1:
    print(-2)
else:
    print(b)
```

## Remove the fragment
Given a string in which the letter h occurs at least twice. Remove from that string the first and the last occurrence of the letter h, as well as all the characters between them.
```
s = input()

a = s.find('h')
b = s.rfind('h') + 1

x = s[a:b]

print(s.replace(x,''))
```

## Reverse the fragment
Given a string in which the letter h occurs at least two times, reverse the sequence of characters enclosed between the first and last appearances.
```
s = input()

a = s.find('h')
b = s.rfind('h') + 1

w = s[a:b]
x = (w[::-1])

y = s[0:a]
z = s[b::]

print(y+x+z)
```

## Replace the substring
Given a string. Replace in this string all the numbers 1 by the word one.
```
s = input()

print(s.replace('1', 'one'))
```

## Delete a character
Given a string. Remove from this string all the characters @.
```
s = input()

print(s.replace('@', ''))
```

## Replace within the fragment
Given a string. Replace every occurrence of the letter h by the letter H, except for the first and the last ones.
```
s = input()
a = s.find('h') + 1
b = s.rfind('h')

s1 = s[0:a]
s2 = s[a:b].replace('h', 'H')
s3 = s[b::]

print(s1 + s2 + s3)
```

## Delete every third character
Given a string. Delete from it all the characters whose indices are divisible by 3.
```
s = input()

result = ''

for i in range(0, len(s)):
    a = s[i]
    if i%3 != 0:
        result += a

print(result)
```
