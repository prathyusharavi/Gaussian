# Gaussian Elimination

## AIM:
To write a program to find the solution of a matrix using Gaussian Elimination.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. start the program
2. develop the code in gusaasian elimination method
3. to find the solution of given use the following method.
4. end the program 

## Program:
```
/*
Program to find the solution of a matrix using Gaussian Elimination.
Developed by: YENUGANTI PRATHYUSHA
RegisterNumber: 23009045
import numpy as np
import sys
n=int(input())
a=np.zeros((n,n+1))
X=np.zeros(n)
for i in range(n):
    for j in range(n+1):
        a[i][j]=float(input())
for i in range(n):
    for j in range(i+1,n):
        ratio=a[j][i]/a[i][i]
        for k in range(n+1):
            a[j][k]=a[j][k]-ratio*a[i][k]
X[n-1]=a[n-1][n]/a[n-1][n-1]
for i in range(n-2,-1,-1):
    X[i]=a[i][n]
    for j in range(i+1,n):
        X[i]=X[i]-a[i][j]*X[j]
    X[i]=X[i]/a[i][i]
for i in range(n):
    print('X%d = %.2f'%(i,X[i]),end=' ')
*/
```

## Output
![image](https://github.com/prathyusharavi/Gaussian/assets/147474424/3dc7b290-89bc-4e2c-a1fc-4880ff757b05)
![image](https://github.com/prathyusharavi/Gaussian/assets/147474424/55a08e8a-fa20-46f7-b378-3bf08a6b4e01)






## Result:
Thus the program to find the solution of a matrix using Gaussian Elimination is written and verified using python programming.

