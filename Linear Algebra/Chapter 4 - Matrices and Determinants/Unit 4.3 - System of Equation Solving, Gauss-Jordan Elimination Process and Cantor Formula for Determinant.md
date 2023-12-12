---
tags:
  - linear_algebra
  - mathematics
  - HUS
---
# System of Equation - Generalization
As far as we are concerned of, we can see that we want to deal with system of equation the matrix way. As such, we would like to define of a system of n-equations as 
$$
S_{n}=
{\displaystyle {\begin{cases}a_{11}x_{1}+a_{12}x_{2}+\dots +a_{1n}x_{n}+b_{1}=b_{1}\\a_{21}x_{1}+a_{22}x_{2}+\dots +a_{2n}x_{n}+b_{2}=b_{2}\\\vdots \\a_{m1}x_{1}+a_{m2}x_{2}+\dots +a_{mn}x_{n}+b_{m}=b_{n},\end{cases}}}
$$
Of which can be represented by matrix as an **augmented coefficient matrix**, $(A|B)$ such that 
$$
(A|B) = \begin{bmatrix}
x_{1}  \\
x_{2}  \\
x_{3} \\
\vdots \\
x_{n}
\end{bmatrix}
\begin{bmatrix}
a_{11} & a_{12} & a_{13} & \cdots & a_{1n} \\
a_{21} & a_{22} & a_{23} & \cdots & a_{2n} \\
a_{31} & a_{32} & a_{33} & \cdots & a_{3n} \\
\vdots & \vdots & \vdots & \ddots & \vdots \\
a_{m1} & a_{m2} & a_{m3} & \cdots  & a_{mn} 
\end{bmatrix}
= \begin{bmatrix}
b_{1}  \\
b_{2}  \\
b_{3} \\
\vdots \\
b_{n}
\end{bmatrix}
$$
Vector-wised, we can represent this as $$
{\displaystyle x_{1}{\begin{bmatrix}a_{11}\\a_{21}\\\vdots \\a_{m1}\end{bmatrix}}+x_{2}{\begin{bmatrix}a_{12}\\a_{22}\\\vdots \\a_{m2}\end{bmatrix}}+\dots +x_{n}{\begin{bmatrix}a_{1n}\\a_{2n}\\\vdots \\a_{mn}\end{bmatrix}}={\begin{bmatrix}b_{1}\\b_{2}\\\vdots \\b_{m}\end{bmatrix}}}
$$
We called all of this as the linear algebra expression of equation. Essentially, $\mathbf{A}\mathbf{x}=\mathbf{B}$. From there, given the following setting: $$
\begin{cases}
\vec{\alpha_{i}}= (a_{1i}& a_{2i} & a_{3i} & \cdots & a_{ni}) \\
 \\
\vec{\beta}=(b_{1}&b_{2}& b_{3}& \cdots & b_{n})
\end{cases}
$$
We have $$\sum_{i=1}^{p} \vec{\alpha_{i}}x_{i} = \vec{\beta}$$
# Rank of a matrix 
Because of the essence that rank of a matrix, or a system of vectors, of which you can thought of it, is the number of linear independent vectors within such system. Hence, we will need to have a way to determine linear independence of a system.
## Reduce Row-Echelon Form (RREF)
Given a matrix $A$, we say the matrix is in reduced echelon form if it has this composition $$\begin{bmatrix}
1& a_{1} & a_{2} &a_{3} & \cdots & a_{n} \\
0 & 1 & a_{2} & a_{3}  & \cdots & a_{n} \\
0 & 0 & 1 & a_{3} & \cdots & a_{n} \\
\vdots & \vdots & \vdots & \vdots & \ddots & \vdots \\
0 & 0 & 0 & 0 & \cdots & 1
\end{bmatrix}$$
With all the main diagonal line being of identity element $1$, and all other to the left being $0$. 

In general, a matrix is in **reduced row-echelon form** if it satisfies the following:
1. In each row, the left-most nonzero entry is 1 and the column that contains this 1 has all other entries equal to 0. This 1 is called a leading 1.
    
2. The leading 1 in the second row or beyond is to the right of the leading 1 in the row just above.
    
3. Any row containing only 0's is at the bottom.

# Kronecker - Capelli Theorem
The general system of equation 
$$
\begin{array}{ccc}
a_{11} x_1 + \cdots + a_{1n}x_n &=& b_1 \\
\vdots & \vdots & \vdots \\
a_{n1} x_1 + \cdots + a_{nn}x_n &=& b_n
\end{array}
$$
is compatible, i.e. has one or more solution if and only if $$\operatorname{rank}(\mathbf{A})=\operatorname{rank}\mathbf{\bar{A}}$$ of which $\mathbf{A}$ is the coefficient matrix $\mathbf{A}=(A_{ij})$ and $\mathbf{\bar{A}}$ is the augmented matrix formed by adding $\mathbf{A}$ and the column of free term $b_{i}$ 

