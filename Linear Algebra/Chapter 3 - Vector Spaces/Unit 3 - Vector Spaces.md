---
tags:
  - HUS
  - linear_algebra
  - mathematics
---
## I. Vectors Spaces
### 1. Definition
Given a set $E$, then $E$ is called a $K$-vector spaces, or a linear spaces on field $K$ if $E$ is equipped with two inner and outer operations $(+,\cdot)$ respectively, addition scalar multiplication such that $$\begin{cases}
E(+) & \text{addition of}\: x_{i} \in E \\ \\
E(\cdot) & \text{multiplication of}\: x_{i}\in E\: \text{and}\: y_{i}\in K \\
\end{cases}$$ Both operations must also satisfy 
$$
\begin{cases}
(E,+) \: \text{is an Abelian group} \\ \\

\lambda(x+y)=\lambda x + \lambda y, &\forall x,y \in E, \forall \lambda \in K\\ \\

(\lambda + \beta)x=\lambda x + \beta x, &\forall \lambda, \beta \in K, \forall x \in E \\
 \\
\lambda(\beta x)= (\lambda\beta)x & \forall \lambda, \beta \in K, x\in E \\
 \\
1\cdot x = x& \forall x \in E \\
\end{cases}
$$
Each of the element of $E$ is a vector. The zero vector of vector space $E$ is denoted $\theta$, and the counter/inverse vector is denoted $-\vec{x}$ of $\vec{x}$. Both of them exist only one, with $\theta$ being a single distinct element, and $-x + (x)=\theta, \forall x \in E$, that is, for every vector $x$ there is only one inverse vector $-x$. We often use two types of notation for element vectors in vector spaces, either with arrows on top or not, and Greek symbols for special vectors. 
#### 1.1 Properties from definition
In accordance, we present some properties of vector spaces $E$. 
1. $\theta x = \theta, \forall x\in E$
2. $\alpha \theta = \theta, \forall \alpha \in K$
3. $\alpha \cdot x = \theta$ if and only if $\alpha = 0$ or $\theta = x$
4. $\alpha (-x) = -(\alpha )x, \forall \alpha \in K, x\in E$
#### 1.2 Widely seen vector spaces
We have some widely seen, and widely used vector spaces we will encounter in different forms. First one is the $\mathbb{R}^{n}$ vector space: $$\mathbb{R}^{n}=\{(x_{1},x_{2},x_{3},x_{4},\dots,x_{n})|x_{i}\in\mathbb{R}, \forall i \in [1,n]\}$$ Secondly, is the polynomial vector spaces $$P(x)=\{a_{0}+a_{1}x+a_{2}x^{2}+\dots+a_{n}x^{n}|a_{i} \in \mathbb{R}\}$$ and the matrices vector spaces $$M_{n}(x)=\{\text{matrices of the same order n}\}$$

### Vector Subspace
Just as same as fields and ring, we have the definition of vector subspace. A vector space $(E,+, \circ)$ on field $K$ has a subspace with $V\subset E$ if $$\forall x,y\in V, \forall k \in K,
\begin{cases}
x+y\in V \\
k x \in V
\end{cases}
$$ Loosely saying, $V$ is a subspace in $E$ if the operation contains itself, returning the value inside the space, of which the space is also a subset of the bigger space, $E$. 

Formally, we would like to write it as a definition 

> [!def] Definition of Vector Subspace
> A set $A\neq \varnothing$, of vector space $E$ on $K$ is called a vector subspace of $E$ if it satisfies
> 1. $\forall \vec{x},\vec{y}\in A$ then $\vec{x}+\vec{y}\in A$
> 2. $\forall \vec{x}, \forall \lambda \in K$ then $\lambda x \in A$

