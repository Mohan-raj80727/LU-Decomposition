# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. 
2. 
3. 
4. 

## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: Mohanraj.s
RegisterNumber: 212224100036
'''
import numpy as np
from scipy.linalg import lu

A = np.array(eval(input()))
P, L, U = lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by: Mohanraj.s
RegisterNumber: 212224100036
'''
import numpy as np
from scipy.linalg import lu_factor, lu_solve

A = np.array(eval(input()))
b = np.array(eval(input()))
lu, piv = lu_factor(A)
X = lu_solve((lu, piv), b)
print(X)

```

## Output:
# L and U matrix:

![image](https://github.com/user-attachments/assets/5f8a40be-acfb-405e-bd34-0087a5c7134e)

# LU Decomposition of a matrix:

![image](https://github.com/user-attachments/assets/fd1266c9-9231-43dc-8dc4-c23ce1543748)


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

