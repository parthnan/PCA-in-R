# PCA-in-R
Simple program for applying Principal Component Analysis on Grayscale Image Data in R.
Takes in any image like the one attached(obama.png), and applies PCA on it, via the Singular Value Decomposition function SVD() in R.
The input is a 256 by 256 pixel image, which is compressed to a 30 by 30 pixel image by the line "D20 = D[1:30,1:30]".

The calculations done in this script are : 
1. Decompose 256 by 256 data matrix A into U,D,V such that A=UDV^⊤, and D is 256 by 256 diagonal matrix, U is 30 by 256 and V is 256 by 30 (via SVD function).

2. Take only the largest 30 constants in D and remove the other elements, so that D is now 30 by 30,  by the line "D20 = D[1:30,1:30]".

3. Reformulate an approximation of  A by UDV^⊤=A and print.

![alt text](https://raw.githubusercontent.com/parthnan/PCA-in-R/master/PCAexample.png)

