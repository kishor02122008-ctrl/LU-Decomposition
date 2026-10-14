# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Import the required libraries: numpy and lu from scipy.linalg.
2.Define the square matrix A using np.array(). 
3. Use lu(A) to decompose A into the permutation matrix P, the lower triangular matrix L and the upper triangular matrix U, so that A = P·L·U.
4. Print the matrices L and U (and P if needed).

## Program:

(i) To find the L and U matrix
```
import os

os.environ["OPENBLAS_NUM_THREADS"]="1"

import numpy as np

from scipy.linalg import lu

A=np.array(eval(input()))

P,L,U=lu(A)

print(L)

print(U)

/*
Program to find the L and U matrix.
Developed by: kishor M
RegisterNumber: 26018383
*/
```
(ii) To find the LU Decomposition of a matrix
```
import os

os.environ["OPENBLAS_NUM_THREADS"]="1"

# To print X matrix (solution to the equations)

import numpy as np

from scipy.linalg import lu_factor,lu_solve

a=np.array(eval(input()))

b=np.array(eval(input()))

l,p=lu_factor(a)

x=lu_solve((l,p),b)

print(x)

/*
Program to find the LU Decomposition of a matrix.
Developed by: kishor M
RegisterNumber: 26018383
*/
```



## Output:<img width="1208" height="830" alt="{42EFF620-C93A-4A08-9837-E69F33282668}" src="https://github.com/user-attachments/assets/d5beb0ac-5115-417c-b793-960cfce732f5" /> <img width="917" height="673" alt="{F9763853-1E6A-4233-88B1-C5DBE3783374}" src="https://github.com/user-attachments/assets/3daf9366-1d3b-468b-94cb-91dd960874ed" />


![lu decomposition]()


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

