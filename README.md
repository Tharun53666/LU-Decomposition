# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
### Step 1:  
Import required libraries `numpy` and `scipy.linalg`.  

### Step 2:  
Input the matrix/matrices using `eval(input())`.  

### Step 3:  
Perform LU decomposition using `lu()` or solve equations using `lu_factor()` and `lu_solve()`.  

### Step 4:  
Print the results `L` and `U` matrices or solution `X` matrix.  

## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: THARRUN D
RegisterNumber: 212224240170
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
Developed by: THARRUN D
RegisterNumber: 212224240170
'''

# To print X matrix (solution to the equations)

import numpy as np
from scipy.linalg import lu_factor, lu_solve


A = np.array(eval(input()))
b = np.array(eval(input()))


lu, piv = lu_factor(A)


x = lu_solve((lu, piv), b)


print(x)
  
```

## Output:
(i) To find the L and U matrix
![Screenshot 2025-05-16 223845](https://github.com/user-attachments/assets/8ded717a-1d69-4c29-a8b7-d31de6a7ad43)


(ii) To find the LU Decomposition of a matrix
![Screenshot 2025-05-16 223859](https://github.com/user-attachments/assets/9290149c-41d1-4a78-9e63-93319714226f)




## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

