# Norm of a matrix
## Aim
To write a program to find the 1-norm, 2-norm and infinity norm of the matrix and display the result in two decimal places.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
	1. Get the input matrix using np.array()   
    2. Find the 2-norm of the matrix using np.linalg.norm()
	3. Print the norm of the matrix in two decimal places.
## Program:
```Python
#Developed by: Rithika.k
#RegisterNumber: 212224230230
# 1-Norm of a Matrix

#EXP.7-CR-Norm of a matrix
##NAME:RITHIKA.K
##REG.NO:212224230230

import numpy as np
def one_norm(matrix):
    arr = np.array(matrix)
    norm_value = np.linalg.norm(arr, 1)  # 1-Norm (column-wise maximum absolute sum)
    return norm_value
matrix =eval(input())
result = one_norm(matrix)
print(f"{result:.2f}")
# 2-Norm of a Matrix
'''
Program to find 2-norm of a matrix.
Developed by: Rithika.k
RegisterNumber: 212224230230
'''
import math
import numpy as np
def l2_norm(matrix):
    A = np.array(matrix, dtype=float)
    return np.linalg.norm(A, 2)
mat1 = eval(input())
print(f"{l2_norm(mat1):.2f}")

# Infinity Norm of a Matrix
'''
Developed by: Rithika.k
RegisterNumber: 212224230230
'''
def infinity_norm(matrix):
   
    row_sums = [sum(abs(val) for val in row) for row in matrix]
    return max(row_sums)
mat =eval(input())
print(f"{infinity_norm(mat):.2f}")  # 8.00
```
## Output:
### 1-Norm of a Matrix
<img width="1376" height="964" alt="image" src="https://github.com/user-attachments/assets/45638f69-c57f-45d0-b6e0-f2da3950e8f3" />
### 2-Norm of a Matrix
<img width="1236" height="990" alt="image" src="https://github.com/user-attachments/assets/afd1743f-0815-4e17-ab64-6e5ebfa47627" />
### Infinity Norm of a Matrix
<img width="1433" height="982" alt="image" src="https://github.com/user-attachments/assets/728479d7-6d48-4e03-8d57-8411a609ee0f" />

## Result
Thus the program for 1-norm, 2-norm and Infinity norm of a matrix are written and verified.
