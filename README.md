# Deep Learning_Raghu Sai Nath Reddy_HW1P2
### Question 2
# Solving a System of Linear Equations

## Problem Statement

We need to solve the following system of linear equations:

1. \( 3x + 4y = -2 \)
2. \( 5x + 3y = 4 \)

## Matrix Representation

The system can be represented in matrix form as:

\[ AX = B \]

where:

- \( A = \begin{bmatrix} 3 & 4 \\ 5 & 3 \end{bmatrix} \)
- \( X = \begin{bmatrix} x \\ y \end{bmatrix} \)
- \( B = \begin{bmatrix} -2 \\ 4 \end{bmatrix} \)

## Solution Method

To solve for \( X \), we use the matrix inverse method:

\[ X = A^{-1}B \]

### Finding the Inverse of Matrix \( A \)

The inverse of a 2x2 matrix \( A = \begin{bmatrix} a & b \\ c & d \end{bmatrix} \) is given by:

\[ A^{-1} = \frac{1}{ad - bc} \begin{bmatrix} d & -b \\ -c & a \end{bmatrix} \]

#### Step-by-Step Calculation

1. **Calculate the Determinant of \( A \):**

   \[
   \text{det}(A) = ad - bc = (3 \cdot 3) - (4 \cdot 5) = 9 - 20 = -11
   \]

2. **Compute the Inverse of \( A \):**

   \[
   A^{-1} = \frac{1}{-11} \begin{bmatrix} 3 & -4 \\ -5 & 3 \end{bmatrix} = \begin{bmatrix} \frac{-3}{11} & \frac{4}{11} \\ \frac{5}{11} & \frac{-3}{11} \end{bmatrix}
   \]

### Solve for \( X \)

Multiply \( A^{-1} \) by \( B \):

\[
X = A^{-1}B = \begin{bmatrix} \{-3}{11} & \{4}{11} \\ \{5}{11} & \{-3}{11} \end{bmatrix} \begin{bmatrix} -2 \\ 4 \end{bmatrix}
\]

#### Calculation:

\[
\begin{bmatrix} \{-3}{11} & \{4}{11} \\ \{5}{11} & \{-3}{11} \end{bmatrix} \begin{bmatrix} -2 \\ 4 \end{bmatrix} = \begin{bmatrix} \frac{-3 \cdot (-2) + 4 \cdot 4}{11} \\ \{5 \cdot (-2) + (-3) \cdot 4}{11} \end{bmatrix} = \begin{bmatrix} \frac{6 + 16}{11} \\ \{-10 - 12}{11} \end{bmatrix} = \begin{bmatrix} \{22}{11} \\ \{-22}{11} \end{bmatrix} = \begin{bmatrix} 2 \\ -2 \end{bmatrix}
\]

## Solution

The solution to the system of linear equations is:

\[
X = \begin{bmatrix} x \\ y \end{bmatrix} = \begin{bmatrix} 2 \\ -2 \end{bmatrix}
\]

Thus, the values of \( x \) and \( y \) that satisfy both equations are \( x = 2 \) and \( y = -2 \).

