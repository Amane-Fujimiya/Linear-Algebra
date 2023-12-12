---
tags:
  - mathematics
  - HUS
  - linear_algebra
---
# Definition
Given a set $X=\{a_{11},a_{21},\dots,a_{mn}\}$, we have the matrix of elements of set $X$, denoted $M_{m \times n}$ or $M_{m \times n}(X)$ is the matrix of size $m \times n$, defined as: 
$$
M_{m \times n}(X) =  \mathbf {A} ={\begin{bmatrix}a_{11}&a_{12}&\cdots &a_{1n}\\a_{21}&a_{22}&\cdots &a_{2n}\\\vdots &\vdots &\ddots &\vdots \\a_{m1}&a_{m2}&\cdots &a_{mn}\end{bmatrix}}={\begin{pmatrix}a_{11}&a_{12}&\cdots &a_{1n}\\a_{21}&a_{22}&\cdots &a_{2n}\\\vdots &\vdots &\ddots &\vdots \\a_{m1}&a_{m2}&\cdots &a_{mn}\end{pmatrix}}
$$ 
of which the matrix $\mathbf{A}$ is the matrix, written for convenience (nobody want to write all those wiggly things), and $a_{mn}\in X$. 
# Types of Matrices 
First of all, we have the zero matrix, $0$, of which all elements are zero:
$$
M_{0} =
\begin{bmatrix}
0 & 0 & \cdots  & 0 \\
0 & 0 & \cdots  & 0 \\ 
\vdots &\vdots &\ddots &\vdots \\
0 & 0 & \cdots &  0\\
\end{bmatrix}
$$
Then the column matrix, of which consists of only $m$ rows: $$A_{R}= \begin{bmatrix}
a_{1} \\
a_{2} \\
a_{3} \\
\vdots \notag \\ 
a_{m}
\end{bmatrix}$$ and row matrix consists of $n$ columns only. $$A_{C}=\begin{bmatrix}
a_{1} & a_{2} & \cdots & a_{n}
\end{bmatrix}$$
There is also square matrix, of which rows and columns are equal. A square matrix has $n\times n$ size, constructed as 
$$SM_{n\times n}=\begin{bmatrix}
a_{11} & a_{12} & \cdots & a_{1n} \\
a_{21} & a_{22} & \cdots & a_{2n} \\
\vdots & \vdots & \ddots & \vdots  \\
a_{n_{1}} & a_{n_{2}} & \cdots & a_{nn}
\end{bmatrix}$$

# Transpose of a Matrix
Given a matrix $$A=\begin{bmatrix}
a_{1}\\  
a_{2}  \\
\vdots  \\
a_{n}
\end{bmatrix}$$
The transpose of $A$, denoted $A^{T}$ is simply a "flip" from a column matrix to a row matrix. Then, $$
A=\begin{bmatrix}
a_{1}\\  
a_{2}  \\
\vdots  \\
a_{n}
\end{bmatrix} 
\longrightarrow 
A^{T} =\begin{bmatrix}
a_{1}&  
a_{2}  &
\cdots  &
a_{n}
\end{bmatrix}
$$ Transpose is like a reverse or mirror mapping, if one wants to say. And rather, it is applicable for square matrix. Given a square matrix as above, $$SM_{n\times n}=\begin{bmatrix}
a_{11} & a_{12} & \cdots & a_{1n} \\
a_{21} & a_{22} & \cdots & a_{2n} \\
\vdots & \vdots & \ddots & \vdots  \\
a_{n_{1}} & a_{n_{2}} & \cdots & a_{nn}
\end{bmatrix}$$ then the construction of $SM_{n\times n}^{T}$ is such that $$SM_{n\times n}^{T}=\begin{bmatrix}
a_{11} & a_{21} & \cdots & a_{n_{1}} \\
a_{12} & a_{22} & \cdots & a_{n2} \\
\vdots & \vdots & \ddots & \vdots  \\
a_{1n} & a_{2n} & \cdots & a_{nn}
\end{bmatrix}$$ of which all elements are flipped symmetric to the main left to right diagonal line. 
# Elementary Matrix Operation
Given two matrix, $A$ and $B$ of the same size, we have: $$A\pm B=\begin{bmatrix}a_{11}\pm b_{11}&a_{12}\pm b_{12}&\cdots &a_{1n}\pm b_{1n}\\a_{21}\pm b_{21}&a_{22}\pm b_{22}&\cdots &a_{2n}\pm a_{2n}\\\vdots &\vdots &\ddots &\vdots \\a_{m1}\pm b_{m1}&a_{m2}\pm  b_{m2}&\cdots &a_{mn}\pm b_{mn}\end{bmatrix}$$
Next, if we take $A$ and multiply the matrix to a scalar $\lambda \in \mathbb{R}$, then $$\lambda A = \begin{bmatrix}\lambda a_{11}&\lambda a_{12}&\cdots & \lambda a_{1n}\\\ \lambda a_{21}& \lambda a_{22}&\cdots & \lambda a_{2n}\\\vdots &\vdots &\ddots &\vdots \\\ \lambda a_{m1}& \lambda a_{m2}&\cdots & \lambda a_{mn}\end{bmatrix}$$
A matrix multiplication operation can be defined, quite special. If $A$ and $B$ are two vectors that have: $column(A)=row(B)$, that is the number of rows of $B$ is equal to the amount of columns that $A$ has, then the multiplication of $AB$, is another matrix $C=AB$. Formally, if we have $A_{m \times n}$ and $B_{n \times p}$, defined as $$\mathbf {A} ={\begin{pmatrix}a_{11}&a_{12}&\cdots &a_{1n}\\a_{21}&a_{22}&\cdots &a_{2n}\\\vdots &\vdots &\ddots &\vdots \\a_{m1}&a_{m2}&\cdots &a_{mn}\\\end{pmatrix}},\quad \mathbf {B} ={\begin{pmatrix}b_{11}&b_{12}&\cdots &b_{1p}\\b_{21}&b_{22}&\cdots &b_{2p}\\\vdots &\vdots &\ddots &\vdots \\b_{n1}&b_{n2}&\cdots &b_{np}\\\end{pmatrix}}$$
Then, the product $C=AB$ is a matrix of size $m \times p$, defined as $$ \mathbf {C} =\begin{pmatrix}a_{11}b_{11}+\cdots +a_{1n}b_{n1}&a_{11}b_{12}+\cdots +a_{1n}b_{n2}&\cdots &a_{11}b_{1p}+\cdots +a_{1n}b_{np}\\a_{21}b_{11}+\cdots +a_{2n}b_{n1}&a_{21}b_{12}+\cdots +a_{2n}b_{n2}&\cdots &a_{21}b_{1p}+\cdots +a_{2n}b_{np}\\\vdots &\vdots &\ddots &\vdots \\a_{m1}b_{11}+\cdots +a_{mn}b_{n1}&a_{m1}b_{12}+\cdots +a_{mn}b_{n2}&\cdots &a_{m1}b_{1p}+\cdots +a_{mn}b_{np}\\\end{pmatrix}$$ That is, for the each element of the matrix $C$, we takes $$c_{ij}=a_{i1}b_{1j}+a_{i2}b_{2j}+\cdots +a_{in}b_{nj}=\sum _{k=1}^{n}a_{ik}b_{kj}$$ of which for $i=\{1,\dots,m\}$ and $j = \{1,\dots,p\}$. So basically, each element of the first row of the first matrix, multiplies by their respective counterpart on the column of the second matrix, then add them all up. Putting into perspective, take $$A=\begin{bmatrix}
a_{1}\\  
a_{2}  \\
\vdots  \\
a_{n}
\end{bmatrix}$$
and $$B=\begin{bmatrix}
b_{1} & b_{2} & \cdots & b_{n}
\end{bmatrix}$$
Then their product is 
$$D=AB=\begin{bmatrix}
a_{1}\\  
a_{2}  \\
\vdots  \\
a_{n}
\end{bmatrix} \cdot \begin{bmatrix}
b_{1} & b_{2} & \cdots & b_{n}
\end{bmatrix} 
= a_{1}b_{1}+ a_{2}b_{2} + \dots + a_{n} b_{n} = \sum_{i=1}^{n} a_{i}b_{i}
$$
which is, coincidentally, the scalar product of two vectors. 



