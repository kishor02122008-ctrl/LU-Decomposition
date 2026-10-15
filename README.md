# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Import the required libraries: numpy and lu from scipy.linalg
2. Define the square matrix A using np.array().
3.  Use lu(A) to decompose A into the permutation matrix P, the lower triangular matrix L and the upper triangular matrix U, so that A = P·L·U.
4.  Print the matrices L and U (and P if needed)

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: kishor M
RegisterNumber: 26018383
*/
```
import os

os.environ["OPENBLAS_NUM_THREADS"]="1"

import numpy as np

from scipy.linalg import lu

A=np.array(eval(input()))

P,L,U=lu(A)

print(L)

print(U)

(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: kishor M
RegisterNumber: 26018383
*/
```
import os

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

## Output:<img width="1280" height="845" alt="{4294808C-9384-495A-8E49-EF85D546E94D}" src="https://github.com/user-attachments/assets/ce661bb6-ecfa-4c58-aef6-2569f275cc92" /><img width="917" height="724" alt="{8A29C083-223F-4B68-8B9E-D015E1694A14}" src="https://github.com/user-attachments/assets/844cd301-9bcb-4cfe-83fa-88e7fb8f4004" />


![lu decomposition]()


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

