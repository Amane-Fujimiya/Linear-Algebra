---
tags:
  - HUS
  - linear_algebra
  - mathematics
---
## II. Linear Combination, Linear Independence and Dependence
### 1. Definition
Let $E$ be a vector spaces on $K$. Then, given a set $A$ contains $$A=\{\vec{V}_{1}, \vec{V}_{2},\cdots ,\vec{V}_{n} \}\: ,n \in [1,n]$$
Then, the equation $$L_{n} = \lambda_{1} \vec{V}_{1}+ \lambda_{2}\vec{V}_{2}+\cdots+ \lambda_{n}\vec{V}_{n}=\sum\limits_{i=1}^{n}\lambda_{i}\vec{V}_{i}\: \: \forall \lambda_{i}\in K$$ is called the **linear combination** of $A$ - a system of vectors. 

A interesting property of linear combination is that - if you have a set of vectors $A=\{V_{i}\}$, $B=\{U_{j}\}$ and $C=\{W_{k}\}$, then if $A$ can be represented by $B$, and $B$ can be represented by $C$, the $A$ can be represented by $C$. One tip to think of linear combination is the operation of combining vectors with additional steps - and a generalizing step. 

### 2. Linear independence and dependence
A system of vectors $$A=\{\vec{V}_{1}, \vec{V}_{2},\cdots ,\vec{V}_{n} \}\: ,n \in [1,n]$$ is called **linear dependent** if there exist scalars $\lambda_{1}, \cdots, \lambda_{n}$ not all *zero* such that $$L_{n} = \lambda_{1} \vec{V}_{1}+ \lambda_{2}\vec{V}_{2}+\cdots+ \lambda_{n}\vec{V}_{n}=\sum\limits_{i=1}^{n}\lambda_{i}\vec{V}_{i}=\textbf{0}$$
with $\textbf{0}$ the zero vector. This implies that at least one of the scalars is non-zero, that is $a_{1}\neq 0$ and the equation is able to be written as $$\vec{V}_{1} = \frac{-a_{2}}{a_{1}}\vec{V}_{2}+\cdots+\frac{-a_{k}}{a_{1} }\vec{V}_{k},\:\forall k>1$$
If $k=1$, then $\vec{V}_{1}=\textbf{0}$, and with $\lambda_{i}=a_{i}$

A sequence/system of vectors $A$ is called linear independent if it is not dependent, that is, 
$$\lambda_{1} \vec{V}_{1}+ \lambda_{2}\vec{V}_{2}+\cdots+ \lambda_{n}\vec{V}_{n}=\sum\limits_{i=1}^{n}\lambda_{i}\vec{V}_{i}=\textbf{0}$$ can only be satisfied by $\lambda_{i}=0$ for $i = 1,\cdots,n$. This implies that no vector in the sequence can be represented as a linear combination of the remaining vectors in the sequence. If a sequence of vectors contains the same vector twice, it is necessarily dependent. 

### 2. Properties
We then have a property of linear independent sequences

> [!warning] Property 1
> All subsets of a set of linear independent vectors are linear independent

> [!caution] Property 2
> If the subset $A$ of a set $S$ is linear dependent then the mother set $S$ is also linear dependent. 

Also, 

> [!caution] Property 3
> $\{\vec{0}\}$ is a linear dependent vector system.

and
> [!caution] Property 4
> A system of vectors $$A=\{\vec{V}_{1}, \vec{V}_{2},\cdots ,\vec{V}_{n} \}$$ with $n \geq 2$ is linear dependent if and only if there is a vector $\vec{V}_{i}$ in $A$ such that $\vec{V}_{i}$ can be represented by other vectors in the system.

### 3 Expanding the definition of linear independence
A vector set $S$ in vector space $V$ is linear independent if for all finite vector sets in $S$, $$\{ \vec{V}_{1}, \vec{V}_{2},\dots, \vec{V}_{m} \}\subset S$$ for $\vec{v}_{i}\neq \vec{v}_{j}, \forall i \neq j$
 

