# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Define the package as scipy.linalg import lu.
2. Get input from user and print L and U matrix by 'print' .
3. Define a package as "from scipy.linalg import lu_factor, lu_solve" and create the variable as 'X' include the package in that variable.
4. Print the variable 'X'

## Program:
(i) To find the L and U matrix
```
Program to find L and U matrix using LU decomposition.
Developed by:S.VENGADA KRISHNAN
RegisterNumber: 212223110061
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))#getting the matrix as array
P,L,U=lu(A)#it returns three values stored in three variables.P IS PERMUTATION MATRIX,DOES NOT WORK THE OTHER WAY AROUND 
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
Program to solve a matrix using LU decomposition.
Developed by:S.VENGADA KRISHNAN
RegisterNumber: 212223110061
# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu_factor,lu_solve
a=np.array(eval(input()))#given matrix lhs
b=np.array(eval(input()))#matrix rhs
lu,piv=lu_factor(a)#it returns lu value and pivot value
X=lu_solve((lu,piv),b)#we are passing these three values to solve the matrix
print(X)

```

## Output:
![maths exp5 q1](https://github.com/SVENGADAKRISHNAN/LU-Decomposition/assets/147473084/44cac6c7-5603-4674-bc10-cbd8b400e3cc)

![maths exp 5 q2](https://github.com/SVENGADAKRISHNAN/LU-Decomposition/assets/147473084/d30c8349-53b6-4ba0-8357-f5f40a5f497e)


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

