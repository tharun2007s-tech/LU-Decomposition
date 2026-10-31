# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm

Step 1:
Import the NumPy and SciPy libraries.

Step 2:
Get the coefficient matrix (A) and constant matrix (b) as input.

Step 3: 
Use lu() to obtain the L and U matrices and lu_factor() and lu_solve() to solve the system of equations.

Step 4: 
Print the L, U and solution (X) matrices.

## Program:
(i) To find the L and U matrix
```python
'''Program to find L and U matrix using LU decomposition.
Developed by: Tharun S
RegisterNumber: 212225240174
'''
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```python
'''Program to solve a matrix using LU decomposition.
Developed by: Tharun S
RegisterNumber: 212225240174
'''

# To print X matrix (solution to the equations)
import os
os.environ["OPENBLAS_NUM_THREADS"]="1" 
import numpy as np
from scipy.linalg import lu_factor,lu_solve 
A=np.array(eval(input()))
b=np.array(eval(input())) 
lu,piv=lu_factor(A)
X=lu_solve((lu,piv),b)
print(X)
```

## Output:

<img width="1175" height="719" alt="image" src="https://github.com/user-attachments/assets/4725ba4d-fc02-41d7-b83f-5cd8f38bc14a" />
<img width="1178" height="389" alt="image" src="https://github.com/user-attachments/assets/9f728a4c-4027-43a0-bdfe-dbb0a70823dc" />


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

