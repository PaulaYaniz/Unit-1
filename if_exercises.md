# Solution to if exercises in Snakify

## 1. Minimum of two numbers
Given two integers, print the smaller value.


![Minimum of two numbers (1)](https://user-images.githubusercontent.com/89135778/132567629-ce18df6a-f453-4add-b74e-4a7915206912.png)



```.py
a = int(input())
b = int(input())

if a < b:
        print(a)    
else:
        print(b)    
```

## 2. Sign function
For the given integer X print 1 if it's positive, -1 if it's negative, or 0 if it's equal to zero.

```.py
x = int(input())

if x > 0:
    print(1)
elif x == 0:
    print(0)
else:
    print(-1)    
```

## 3. Minimum of three numbers
Given three integers, print the smallest value.

```.py
a = int(input())
b = int(input())
c = int(input())

if b > a < c:
    print(a)
elif a > b < c:
    print(b)
else:
    print(c)   
```

## 4. Equal numbers
Given three integers, determine how many of them are equal to each other. 
The program must print one of these numbers: 3 (if all are the same), 2 (if two of them are equal to each other and the third is different) or 0 (if all numbers are different).

```.py
a = int(input())
b = int(input())
c = int(input())

if a == b == c:
    print("3")
elif a == b or b == c or c == a:
    print("2")
else:
    print("0")
```

## 5. Rook move
Chess rook moves horizontally or vertically. Given two different cells of the chessboard, determine whether a rook can go from the first cell to the second in one move.
The program receives the input of four numbers from 1 to 8, each specifying the column and row number, first two - for the first cell, and then the last two - for the second cell. 
The program should output YES if a rook can go from the first cell to the second in one move, or NO otherwise.

```.py
c1 = int(input())
r1 = int(input())
c2 = int(input())
r2 = int(input())

if c1 == c2 or r1 == r2:
    print("YES")
else:
    print("NO")
```

## 6. Chess board - same color
Given two cells of a chessboard. If they are painted in one color, print the word YES, and if in a different color - NO.
The program receives the input of four numbers from 1 to 8, each specifying the column and row number, first two - for the first cell, and then the last two - for the second cell.

```.py

```

## 7. King move
Chess king moves horizontally, vertically or diagonally to any adjacent cell. Given two different cells of the chessboard, determine whether a king can go from the first cell to the second in one move.
The program receives the input of four numbers from 1 to 8, each specifying the column and row number, first two - for the first cell, and then the last two - for the second cell. 
The program should output YES if a king can go from the first cell to the second in one move, or NO otherwise.

```.py

```

## 8. Bishop moves
In chess, the bishop moves diagonally, any number of squares. Given two different squares of the chessboard, determine whether a bishop can go from the first to the second in one move.
The program receives as input four numbers from 1 to 8, specifying the column and row numbers of the starting square and the column and row numbers of the ending square. The program should output YES if a Bishop can go from the first square to the second in one move, or NO otherwise.

```.py

```

## 9. Queen move
Chess queen moves horizontally, vertically or diagonally to any number of cells. Given two different cells of the chessboard, determine whether a queen can go from the first cell to the second in one move.
The program receives the input of four numbers from 1 to 8, each specifying the column and row number, first two - for the first cell, and then the last two - for the second cell. 
The program should output YES if a queen can go from the first cell to the second in one move, or NO otherwise.

```.py

```

## 10. Knight move
Chess knight moves like the letter L. It can move two cells horizontally and one cell vertically, or two cells vertically and one cells horizontally. Given two different cells of the chessboard, determine whether a knight can go from the first cell to the second in one move.
The program receives the input of four numbers from 1 to 8, each specifying the column and row number, first two - for the first cell, and then the last two - for the second cell. 
The program should output YES if a knight can go from the first cell to the second in one move, or NO otherwise.

```.py

```

## 11. Chocolate bar
Chocolate bar has the form of a rectangle divided into n×m portions. Chocolate bar can be split into two rectangular parts by breaking it along a selected straight line on its pattern. Determine whether it is possible to split it so that one of the parts will have exactly k squares.
The program reads three integers: n, m, and k. It should print YES or NO.

```.py
n = int(input())
m = int(input())
k = int(input())

if m * n < k:
    print("NO")
else:
    if (k % m == 0) or (k % n == 0):
        print("YES")
    else:
        print("NO")
```

## 12. Leap year
Given the year number. You need to check if this year is a leap year. If it is, print LEAP, otherwise print COMMON.
The rules in Gregorian calendar are as follows:
- a year is a leap year if its number is exactly divisible by 4 and is not exactly divisible by 100
- a year is always a leap year if its number is exactly divisible by 400

```.py

```
