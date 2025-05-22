# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm 
### (i) To Find the L and U Matrices

1. *Start*

2. *Import the necessary library*: numpy as np.

3. *Prompt the user to enter a square matrix A*.

4. *Convert the user input into a NumPy array*.

5. *Check if the matrix is invertible* by verifying that its determinant is not zero using np.linalg.det(A).

6. *If the matrix is invertible*, compute the inverse using np.linalg.inv(A) and store the result.

7. *Display the inverse matrix*.

8. *If the determinant is zero*, display a message stating that the matrix is not invertible.

9. *End the program*.

### (ii) To Find the LU Decomposition and Solve a System

1. *Start*

2. *Import the necessary library*: numpy as np.

3. *Prompt the user to enter a square matrix A.*

4. *Convert the input into a NumPy array.*

5. **Use np.linalg.det(A) to compute the determinant of the matrix A and store the result in det.**

6. **Display the value of the determinant det.**

7. *End the program.*


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

