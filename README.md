# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. read the elements of augmented matrix into array a and b
2. calculate elements of L and U
3. print L and U matrix
4. find V by solving LV = B by forwrd substitution
5. find X by solving UX = V by backward substitution
6. print array X as the solution

## Program:
(i) To find the L and U matrix
```python
/*
Program to find the L and U matrix.
Developed by: ARVIND S
RegisterNumber: 212222240012
*/
import numpy as np
from scipy.linalg import lu
A = np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```python
/*
Program to find the LU Decomposition of a matrix.
Developed by: ARVIND s
RegisterNumber: 212222240012
*/
import numpy as np
from scipy.linalg import lu_factor, lu_solve
A,B=eval(input()),eval(input())
lu,piv=lu_factor(A)
x = lu_solve((lu,piv),B)
print(x)
```

## Output:
![Screenshot 2023-09-25 224256](https://github.com/S-ARVIND01/LU-Decomposition/assets/118707337/9835a92f-08b3-41e9-a241-f93cc1d4a078)

![Screenshot 2023-09-25 224559](https://github.com/S-ARVIND01/LU-Decomposition/assets/118707337/ce68bd73-b4a2-4878-96c5-c9eea2a014bd)

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

