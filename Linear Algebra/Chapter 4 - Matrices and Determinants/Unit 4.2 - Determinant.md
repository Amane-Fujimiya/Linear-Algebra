---
tags:
  - HUS
  - linear_algebra
  - mathematics
---
Given a $2\times 2$ matrix $A$, we defined the determinant of $A$ as $$\det(A)= \det \begin{bmatrix}
A_{11} & A_{12} \\
A_{21} & A_{22} 
\end{bmatrix}= A_{11}A_{22} - A_{12}A_{21}$$
For a $3 \times 3$ matrix $B$, we defined the determinant as follow: $$
\begin{split}
\det(B) &= \det \begin{bmatrix}
b_{1} & b_{2} & b_{3} \\
b_{4} & b_{5} & b_{6} \\
b_{7} & b_{8} & b_{9} 
\end{bmatrix}\\
& = 
b_{1} \det \begin{bmatrix}
b_{5} & b_{6} \\
b_{8} & b_{9}
\end{bmatrix}- b_{2} \det \begin{bmatrix}
b_{4} & b_{6} \\
b_{7} & b_{9}
\end{bmatrix}+b_{3} \det \begin{bmatrix}
b_{4} & b_{5} \\
b_{7} & b_{8}
\end{bmatrix}\\
& = b_{1} (b_{5}b_{9}-b_{6}b_{8}) - b_{2} (b_{4}b_{9}-b_{6}b_{7}) + b_{3} (b_{4}b_{8}-b_{5}b_{7})
\end{split}
$$
Note that 
- The determinant $\det(B)$ of a 3-dimensional matrix is the combination of its smaller square matrices, called minors. 
- Calculating can be memorized effectively as blocking the row and column that the first entry (the one that is the basis of all) is in, then take the determinant of a minor containing all other rows and columns. 
- We alternate signs throughout the computation. 

# General Formula for Determinant - Laplace Expansion for Recursive Expansion

In general, Laplace formula is a good generalization of determinant for any given $n \times n$ matrices, as follow: 

> [!def] Laplace Expansion
> Given a $n \times n$ matrix $B$, we define the general formula for determinant of $B$ along the $i^{th}$ row is $$\det(B)=\sum_{j=1}^{n} (-1)^{i+j} b_{\:i,\:j} \cdot m_{\:i,\:j} $$ with $m_{\:i,\:j}$ the determinant of the minor (or submatrix) that does not contain the $ith$ row and $j th$ column. Similarly, if we expand throughout the $j^{th}$ column, then the general formula is defined as $$\det(B) = \sum_{i=1}^{n} (-1)^{i+j} b_{\:i,\:j} \cdot m_{\:i,\:j}$$

# Property of Determinant

We will lists some of the properties (or most of them) and some proof. 

First, we will have to define (again for reference) the row operation: 

> [!def] Row operation
> The row operation consists of the following 
> 1. Switches two rows.
> 2. Multiply a row by a number $k\in \mathbb{R}$ such that $k\neq 0$.
> 3. Replace a row by a multiple of another row added to itself. 

We then begin with our theorems and properties. 

> [!thm] Theorem 1
> Let $A$ be an $n \times n$ matrix and let $B$ be a matrix which results from switching two rows of $A$. Then $$\det(A)=-\det(B)$$

> [!thm] Multiply a row by a scalar 
> Let $A$ be an $n \times n$ matrix and let $B$ be a matrix which results from multiplying some rows of $A$ by a scalar $k$. Then $$\det(B)=k \det (A)$$

> [!thm] Theorem of Scalar Multiplication (general)
> Let $A$ and $B$ be $n \times n$ matrices and $k$ a scalar. such that $B = kA$. Then $$\det(B)= k^{n}\det(A)$$

> [!thm] Adding a multiple of a row to another row
> Let $A$ be and $n \times n$ matrix and let $B$ be a matrix which results rom adding a multiple of a row to another row. then $$\det(A)=\det(B)$$

> [!thm] Determinant of a Product
> Let $A$ and $B$ be two $n \times n$ matrix. Then $$\det(AB)=\det(A)\det (B)$$

> [!thm] Determinant of the Transpose
> Let $A$ be a matrix where $A^{T}$ is the transpose of $A$. Then $$\det(A^{T})=\det(A)$$

> [!thm] Determinant of the Inverse
> Let $A$ be an $n \times n$ matrix. Then $A$ is invertible if and only if $\det)(A)\neq 0$. If this is satisfied, then $$\det(A^{-1})=\frac{1}{\det(A)}$$

## Important Property (and Proof)

Here are some properties that go with their proofs, of which determinant has. 

> [!lem] Lemma 1
> If $A$ is an $n \times n$ matrix, such that one of its row $i \leq n$, then $\det(A)=0$ 

> [!lem] Lemma 2
> Assume $A$, $B$ and $C$ are $n \times n$ matrices that for ome $1 \leq i \leq n$ satisfy the following.
> 1. $jth$ rows of all three matrices are identical, for $j \neq i$. 
> 2. Each entry in the $jth$ row of $A$ is the sum of corresponding entries in $jth$ rows of $B$ and $C$. 
> Then we have $$\det(A)=\det(B) + \det(C)$$

> [!lem] Let $A$ and $B$ be $n \times n$ matrices. 
> - If $A$ is obtained by interchanging $ith$ and $jth$ rows of $B$ ($i\neq j$) then $$\det(A)=-\det(B)$$
> - If $A$ is obtained by multiplying $ith$ row of $B$ by $k$ then $$\det(A)=k\det(B)$$
> - if two rows of $A$ are identical then $\det(A)=0$
> - If $A$ is obtained by multiplying $ith$ row of $B$ by $k$ and adding it to $jth$ row of $B$ $(\forall i \neq j)$ then $$\det(A)=\det(B)$$

> [!thm] Uniformity of Determinant
> Expanding an $n \times n$ matrix along any row or column gives the same result, which is the determinant. 
### Proof 

We will prove this lemma using mathematical induction. 
If $n =2$ then the upper lemma is correct. 

Let $n \geq 3$ be such that every matrix of size $n-1 \times n-1$ with a row consisting of zeroes has determinant equal to zero. Let $i$







___
# Reference 

- https://math.libretexts.org/Courses/Lake_Tahoe_Community_College/A_First_Course_in_Linear_Algebra_(Kuttler)/03%3A_Determinants/3.02%3A_Properties_of_Determinants

