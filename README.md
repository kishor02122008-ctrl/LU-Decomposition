# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Import the required libraries: numpy and lu from scipy.linalg.
2. Define the square matrix A using np.array()
3. Use lu(A) to decompose A into the permutation matrix P, the lower triangular matrix L and the upper triangular matrix U, so that A = P·L·U.  
4. Print the matrices L and U (and P if needed).


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

os.environ["OPENBLAS_NUM_THREADS"]="1"

# To print X matrix (solution to the equations)

import numpy as np

from scipy.linalg import lu_factor,lu_solve

a=np.array(eval(input()))

b=np.array(eval(input()))

l,p=lu_factor(a)

x=lu_solve((l,p),b)

print(x)



## Output:<img width="1257" height="813" alt="{B1864E7B-BCC8-4B74-9A9A-DDB006DE3A85}" src="https://github.com/user-attachments/assets/0844ab9c-a085-41f0-a395-d2867cb67656" /><img width="884" height="706" alt="{7CE3D485-9984-46DC-8A6F-BACED230B8F2}" src="https://github.com/user-attachments/assets/5e980bbc-4f46-45b2-b963-427903679319" />


![lu decomposition]()


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

