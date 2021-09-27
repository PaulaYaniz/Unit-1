## Ask the user for  2 numbers, A and B, Output TRUE if one of them is 10 or if their sum is 10.

Examples
Makes10(9, 10) → TRUE
Makes10(9, 9) → FALSE
Makes10(1, 9) → TRUE

```
A = int(input())
B = int(input())

if A or B or A+B == 10:
    print("True")
else: 
    print("False")
```
