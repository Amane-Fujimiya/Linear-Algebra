---
tags:
  - linear_algebra
  - HUS
  - mathematics
---
# Unique Solution of $2 \times 2$ system 
The $2 \times 2$ system $$\begin{cases}
ax+by=e \\
cx+dy=f
\end{cases}$$
Has a unique solution providing $\Delta = ad-bc$ which is non-zero, then $$
x=\frac{de-bf}{ad-bc} \quad y = \frac{af-ce}{ad-bc}
$$
This is called **Cramer's rule** for $2 \times 2$ system. 

## Determinant of Order $2$. 
The system above can be written in augmented matrix form: $$
\begin{bmatrix}
x \\
y
\end{bmatrix}
\begin{bmatrix}
a & b \\
c & d
\end{bmatrix}
=\begin{bmatrix}
e \\
f
\end{bmatrix}
$$
We denoted as from [[Unit 4.2 - Determinant]] the determinant of a $2 \times 2$ system as matrix: $$A=\begin{bmatrix}
a&b \\
c& d 
\end{bmatrix}$$
of which $$
\det(A) =
\begin{vmatrix}
a & b \\
c & d
\end{vmatrix}= ad-bc
$$ The product $ad$ is the product of the main diagonal line. 

Cramer's rule in this case can be represented using the notation of linear algebra: 
$$
x=  \frac{\begin{vmatrix}
e & b \\
f & d
\end{vmatrix}}{\begin{vmatrix}
a & b \\
c & d
\end{vmatrix}}
\quad ; \quad 
y=\frac{\begin{vmatrix}
a & e \\
c & f
\end{vmatrix}}{\begin{vmatrix}
a & b \\
c & d
\end{vmatrix}}
$$
## Generalization of Cramer's rule
