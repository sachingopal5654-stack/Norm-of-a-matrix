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
Python
# Register No: 26011448
# Developed By: Sachin G
```
# 1-Norm of a Matrix
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
A=np.array(eval(input()))
norm1=np.linalg.norm(A,1)
norm="{:.2f}".format(norm1)
print(norm)

# 2-Norm of a Matrix
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
a=np.array(eval(input()))
b=np.linalg.norm(a,2)
c="{:.2f}".format(b)
print(c)

# Infinity Norm of a Matrix
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import ast
matrix = ast.literal_eval(input())
infinity_norm = max(sum(abs(val)for val in row)for row in matrix)
print(f"{infinity_norm:.2f}")

```
## Output:
### 1-Norm of a Matrix
<img width="1235" height="836" alt="Screenshot 2026-11-16 155339" src="https://github.com/user-attachments/assets/86d53640-fa8d-4c1e-be83-64e37da45f82" />


### 2-Norm of a Matrix
<img width="1238" height="846" alt="Screenshot 2026-11-16 155512" src="https://github.com/user-attachments/assets/837fdb83-5c5b-4a36-a13f-c7e88414bd9f" />


### Infinity Norm of a Matrix
<img width="1230" height="843" alt="Screenshot 2026-11-16 155559" src="https://github.com/user-attachments/assets/a3355f16-1f7f-4965-b1ff-fd046b9f5d7e" />


## Result
Thus the program for 1-norm, 2-norm and Infinity norm of a matrix are written and verified.
