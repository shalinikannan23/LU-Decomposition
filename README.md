# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1.  Generate a matrix A = LU such that L is the lower triangular matrix with principal diagonal elements being equal to 1 and U is the upper triangular matrix.
2.  Now, we can write AX = B as:LUX = B
3.  Let us assume UX = Y
4.  From equations (1) and (2), we have:LY = B
5.  Substituting Y in equation (2), we get UX = Y. 
## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: shalini.k
RegisterNumber: 212222240095
'''
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by:shalini.k 
RegisterNumber: 212222240095
'''
# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=eval(input())
B=eval(input())
lu,piv=lu_factor(A)
C=lu_solve((lu,piv),B)
print(C)
```

## Output:

![Screenshot (143)](https://github.com/shalinikannan23/LU-Decomposition/assets/118656529/ab2539fb-0b54-4226-b843-46b7aaa4f1eb)
![Screenshot (144)](https://github.com/shalinikannan23/LU-Decomposition/assets/118656529/f340fc09-a622-47ec-b06c-182279205241)
## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

