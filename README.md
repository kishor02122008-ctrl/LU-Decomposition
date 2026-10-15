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

## Algorithm
1. Import the required libraries (numpy and the lu function from scipy.linalg)
2. Receive the input matrix A and convert it into a NumPy array
3. Apply the lu(A) function to compute the permutation and triangular matrices (P, L, and U)
4. Print the resulting Lower (L) and Upper (U) matrices

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: kishor M
RegisterNumber: 26018383
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
Developed by: kishor M
RegisterNumber: 26018383
*/
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

## Output:<img width="1280" height="845" alt="{4294808C-9384-495A-8E49-EF85D546E94D}" src="https://github.com/user-attachments/assets/ce661bb6-ecfa-4c58-aef6-2569f275cc92" />

## Output:<img width="917" height="724" alt="Screenshot 2026-10-15 102319" src="https://github.com/user-attachments/assets/384f2f57-ffd4-4a67-bc83-0f580571072e" />



![lu decomposition]()


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

