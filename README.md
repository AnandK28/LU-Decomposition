# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
### Program (i): LU Decomposition
1.Import NumPy and lu from scipy.linalg.

2.Input square matrix A from the user.

3.Use lu(A) to compute permutation matrix P, lower matrix L, and upper matrix U.

4.Print matrix L.

5.Print matrix U.

### Program (ii): Solving Ax = b using LU Decomposition
1.Import NumPy and lu_factor, lu_solve from scipy.linalg.

2.Input square matrix A and vector b from the user.

3.Compute LU decomposition and pivot using lu_factor(A).

4.Solve the system using lu_solve((lu, piv), b).

5.Print the solution vector x.


## Program:
(i) To find the L and U matrix
``` python

Program to find the L and U matrix.
Developed by: ANAND K
RegisterNumber: 212224040022

import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
``` python

Program to find the LU Decomposition of a matrix.
Developed by: ANAND K
RegisterNumber: 212224040022

import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
b=np.array(eval(input()))
lu,piv=lu_factor(A)
X=lu_solve((lu, piv),b)
print(X)

```

## Output:
### 1:
![image](https://github.com/user-attachments/assets/7e2e9bca-d5fc-4187-89d6-202f561dc99d)
### 2:
![image](https://github.com/user-attachments/assets/2421a60a-2465-4e49-b8f5-9c4db928659e)



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

