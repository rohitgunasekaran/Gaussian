# Gaussian Elimination

## AIM:
To write a program to find the solution of a matrix using Gaussian Elimination.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Import numpy as np and get the values
2. Using for loop execute the program
3. Print the values
4. End the values

## Program:
```
/*
Program to find the solution of a matrix using Gaussian Elimination.
Developed by: rohit g 
RegisterNumber:212222240083
import numpy as np
n=int(input())
arr=np.zeros((n,n+1))
res=np.zeros(n)
for i in range(n):
    for j in range(n+1):
        arr[i][j]=int(input())
for i in range(n):
    for j in range(i+1,n):
        ratio=arr[j][i]/arr[i][i]
        for k in range(n+1):
            arr[j][k]=arr[j][k]-ratio*arr[i][k]
res[n-1]=arr[n-1][n]/arr[n-1][n-1]
for i in range(n-2,-1,-1):
    res[i]=arr[i][n]
    for j in range(i+1,n):
        res[i]=res[i]-arr[i][j]*res[j]
        res[i]=res[i]/arr[i][i]
for i in range(n):
    print("X%d = %0.2f" %(i,res[i]),end=" ")
*/
```

## Output:
![gaussian elimination]()

![image](https://github.com/rohitgunasekaran/Gaussian/assets/119404546/d05f2723-536a-47ee-980d-1c2e17bce9c5)

## Result:
Thus the program to find the solution of a matrix using Gaussian Elimination is written and verified using python programming.

