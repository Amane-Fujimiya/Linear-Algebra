---
tags:
  - HUS
  - linear_algebra
  - mathematics
---
# I. Definition

Given vector space $E$, and $A=\{\vec{V}_{i}\}$, $i=\{1,\dots,m\}$. Then the sub-system $B \subset A$ is  **maximally linear independent** if including any more vector $\vec{V}_{j}$ such that $\vec{V}_{j} \in A \setminus B$ will result in a linear dependent system. 

Basically speaking, if $A$ is a vector system, and $B$ is a subset of that system, of which $B$ is linear independent, then adding more vectors from those vectors that is not in $B$, but in $A$ results in a linear dependent set. Most of the time a maximal linear independent system of vectors will be the basis. But this is applicable to any other vector systems. 

We would like to pick an example, including 
$$
V_{set} =
\begin{cases}
e_{1}=(1,0,0) \\
e_{2} = (0,1,0) \\
e_{3} = (0,0,1) \\
\end{cases}
$$ In $\mathbb{R}^3$, the system of vector is linear independent. Extend this into $\mathbb{R}^4$, we gain 
$$
V_{\mathbb{R}^{4}}=
\begin{cases}
e_{1} = (1,0,0,0) \\
e_{2} = (0,1,0,0) \\
e_{3} = (0,0,1,0) \\
e_{4} = (0,0,0,1)
\end{cases}
$$ This is a subset of a non-linear independent system $V'_{\mathbb{R}^4}$, that is
$$
V'_{\mathbb{R}^{4}}= 
\begin{cases}
e_{1} = (1,0,0,0) \\
e_{2} = (0,1,0,0) \\
e_{3} = (0,0,1,0) \\
e_{4} = (0,0,0,1) \\
e_{5} = (2,3,9,0) \\
e_{5} = (1,1,4,12) \\
\dots \\
e_{n} = (x_{1},x_{2},x_{3},x_{4})
\end{cases}
$$ of which all elements from $e_{5}$ to $e_{n}$ adding into $V_{\mathbb{R}^4}$ will result in a linear dependent system. Of course, we would like to see that the other vectors aside from $e_{1}\to e_{4}$ are results from the linear combination of 4 beginning vectors. Hence, we can also say that the other vectors is redundant to our purpose. Most of the time, we do not need them, since they are a variant of the basis of the system. 

Theoretically speaking, in a system of vectors, what is the best optimized number of vectors that can be used in linear combination to expresses vectors in the system? Or, you would want to understand in a good term - what is the maximum sub-vector system that represent all vectors in the original system. 

The number of vectors in a maximal linear independent vector system is equal, and that is the **rank** of a vector system $A$, denoted $$\operatorname{rank}(A)=n$$
# II. Properties
### Property I
If all vectors in $A$ can be expressed using linear combination from $B$, then $$\operatorname{rank}(A)\leq \operatorname{rank}(B)$$
### Property II
For all $\vec{V}_{j}\in A$ that can be expressed by $\vec{B}_{i}\in B$ and reversed, then $$rank(A)=rank(B)$$
### Property III
Non-rank-changing operator: 
- Removing $\vec{0}\in A$,
- Changing the order of vectors, that is $\vec{V_{i}}\to \vec{V}_{j}, \forall i\neq j$
- Multiply a vector by a scalar, $\vec{V}\rightarrow k \vec{V}; \forall k \in K, k\neq 0$. 
- Adding a vector to the choosing vector, $\vec{V}\rightarrow \vec{V}+\vec{U}, \vec{U}\in A$. 
