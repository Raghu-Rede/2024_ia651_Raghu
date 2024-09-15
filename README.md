# 2024_Deep Learning (CS47001_F24)_Raghu Sai Nath Reddy
### Question 1
# Matrix Multiplication README

## Overview

This document explains the computation of the matrix product \( R = A \times B \) given two matrices \( A \) and \( B \). The matrices are:

Matrix \( A \):
\[
A =
\begin{bmatrix}
7 & 2 & 1 \\
10 & 5 & 0 \\
7 & 3 & 2 \\
4 & 8 & 9
\end{bmatrix}
\]

Matrix \( B \):
\[
B =
\begin{bmatrix}
12 & 3 & 0 \\
10 & 2 & 4 \\
6 & 8 & 3
\end{bmatrix}
\]

## Matrix Multiplication Steps

### 1. Confirm Matrix Dimensions

- Matrix \( A \) is \( 4 \times 3 \) (4 rows, 3 columns).
- Matrix \( B \) is \( 3 \times 3 \) (3 rows, 3 columns).
- The product matrix \( R \) will be \( 4 \times 3 \) (4 rows, 3 columns).

### 2. Calculate Each Element of Matrix \( R \)

Each element \( r_{ij} \) in matrix \( R \) is computed using:
\[
r_{ij} = \sum_{k=1}^{3} a_{ik} \cdot b_{kj}
\]
where \( a_{ik} \) is the element in the \( i \)-th row and \( k \)-th column of \( A \), and \( b_{kj} \) is the element in the \( k \)-th row and \( j \)-th column of \( B \).

#### Calculation of Elements

- **First Row of \( R \)**:
  \[
  r_{11} = (7 \ 12) + (2 \ 10) + (1 \ 6) = 84 + 20 + 6 = 110
  \]
  \[
  r_{12} = (7 \ 3) + (2 \ 2) + (1 \ 8) = 21 + 4 + 8 = 33
  \]
  \[
  r_{13} = (7 \ 0) + (2 \ 4) + (1 \ 3) = 0 + 8 + 3 = 11
  \]

- **Second Row of \( R \)**:
  \[
  r_{21} = (10 \times 12) + (5 \times 10) + (0 \times 6) = 120 + 50 + 0 = 170
  \]
  \[
  r_{22} = (10 \times 3) + (5 \times 2) + (0 \times 8) = 30 + 10 + 0 = 40
  \]
  \[
  r_{23} = (10 \times 0) + (5 \times 4) + (0 \times 3) = 0 + 20 + 0 = 20
  \]

- **Third Row of \( R \)**:
  \[
  r_{31} = (7 \times 12) + (3 \times 10) + (2 \times 6) = 84 + 30 + 12 = 126
  \]
  \[
  r_{32} = (7 \times 3) + (3 \times 2) + (2 \times 8) = 21 + 6 + 16 = 43
  \]
  \[
  r_{33} = (7 \times 0) + (3 \times 4) + (2 \times 3) = 0 + 12 + 6 = 18
  \]

- **Fourth Row of \( R \)**:
  \[
  r_{41} = (4 \times 12) + (8 \times 10) + (9 \times 6) = 48 + 80 + 54 = 182
  \]
  \[
  r_{42} = (4 \times 3) + (8 \times 2) + (9 \times 8) = 12 + 16 + 72 = 100
  \]
  \[
  r_{43} = (4 \times 0) + (8 \times 4) + (9 \times 3) = 0 + 32 + 27 = 59
  \]

### Final Matrix \( R \)

Combining all computed elements, the resulting matrix \( R \) is:
\[
R =
\begin{bmatrix}
110 & 33 & 11 \\
170 & 40 & 20 \\
126 & 43 & 18 \\
182 & 100 & 59
\end{bmatrix}
\]

