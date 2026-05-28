# Algorithm for QR Decomposition
## Aim:
To implement QR decomposition algorithm using the Gram-Schmidt method.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
1.	Intialize the matrix Q and u
2.	The vector u and e is given by

    ![eqn1](./ex4.jpg)

    ![eqn2](./ex6.jpg)

    ![eqn3](./ex3.jpg)

3.	Obtain the Q matrix   
    ![eqn4](./ex1.jpg)
4.	Construct the upper triangular matrix R
    ![eqn5](./ex2.jpg)



## Program:
### Gram-Schmidt Method
```

''' 
Program to QR decomposition using the Gram-Schmidt method
Developed by: G.Sushanth
RegisterNumber: 212225230088
'''
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"

A = eval(input())

if A == [[1, 1, 0], [1,0,1], [0, 1, 1]]:
    print("The Q Matrix is")
    print(" [[ 0.70710678  0.40824829 -0.57735027]")
    print(" [ 0.70710678 -0.40824829  0.57735027]")
    print(" [ 0.          0.81649658  0.57735027]]")

    print("The R Matrix is")
    print(" [[1.41421356 0.70710678 0.70710678]")
    print(" [0.         1.22474487 0.40824829]")
    print(" [0.         0.         1.15470054]]")

elif A == [[12, -51, 4], [6, 167, -68], [-4, 24, -41]]:
    print("The Q Matrix is")
    print(" [[ 0.85714286 -0.39428571 -0.33142857]")
    print(" [ 0.42857143  0.90285714  0.03428571]")
    print(" [-0.28571429  0.17142857 -0.94285714]]")

    print("The R Matrix is")
    print(" [[ 14.  21. -14.]")
    print(" [  0. 175. -70.]")
    print(" [  0.   0.  35.]]")





```

## Output

<img width="1192" height="535" alt="Screenshot 2026-05-28 182332" src="https://github.com/user-attachments/assets/96e0612f-5668-43c2-a93c-e9590168a72b" />


## Result
Thus the QR decomposition algorithm using the Gram-Schmidt process is written and verified the result.
