# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm 
## 5a
### step1.
import the required numpy and scipy
### step2.
define the matrix A using np.array
### step3.
find the matrix P,L,U using lu(A)
### step4.
print L and U

## 5b
### step1. import the required numpy and scipy
### step2. define the matrix A and B using np.array
### step3. find the LU factorization of A using lu_solve()
### step4. solve the system using lu_solve()
### step5. print the solution matrix x

## Program:
(i) To find the L and U matrix
```
/*
'''Program to find L and U matrix using LU decomposition.

Developed by: T A Keerthana

RegisterNumber: 26009041
'''
import os

os.environ["OPENBLAS_NUM_THREADS"]="1"

import numpy as np

from scipy.linalg import lu

A=np.array(eval(input()))

P,L,U=lu(A)

print(L)

print(U) 
*/
```
(ii) To find the LU Decomposition of a matrix
```
/*
'''Program to solve a matrix using LU decomposition.

Developed by:T A Keerthana
 
RegisterNumber: 26009041
'''

# To print X matrix (solution to the equations)

import os

os.environ["OPENBLAS_NUM_THREADS"]="1"

import numpy as np

from scipy.linalg import lu_factor,lu_solve

a=np.array(eval(input()))

b=np.array(eval(input()))

l,p=lu_factor(a)

x=lu_solve((l,p),b)

print(x)
*/
```

## Output:
<img width="942" height="497" alt="image" src="https://github.com/user-attachments/assets/96e096e8-6fdc-4648-88ce-4919bf83c2c6" />
<img width="1222" height="473" alt="image" src="https://github.com/user-attachments/assets/6ea5c948-f728-4d33-9de7-2febfcbfe652" />



![lu decomposition]()


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

