# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
### (1) To Find The L and u matrix
# step 1: Import NumPy and lu from scipy.linalg.
# step 2: Read matrix input from the user using input() and convert it into a NumPy array.
# step 3: Perform LU decomposition using lu() function and store the result in P, L, U.
# step 4: Print the lower triangular matrix L.
# step 5: Print the upper triangular matrix U.

### (2) To Find The L and u matrix
# step 1: Import NumPy and the functions lu_factor and lu_solve from scipy.linalg.
# step 2: Read matrix A (coefficient matrix) from the user and convert it into a NumPy array.
# step 3: Read matrix or vector B (right-hand side of the equation Ax = B) from the user and convert it into a NumPy array.
# step 4: Perform LU factorization of matrix A using lu_factor(A).This returns lu (combined LU decomposition) and piv (pivot indices).
# step 5: Solve the linear system using lu_solve((piv, lu), B) and store the result.
# step 6: Print the solution vector or matrix.

## Program:
(i) To find the L and U matrix
```python
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
```python
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

