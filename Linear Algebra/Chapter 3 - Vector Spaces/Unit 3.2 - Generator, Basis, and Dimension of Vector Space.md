## I. Generator 
### Definition

Given a system of vectors $V$ of $E$, if all vectors in vector space $E$ can be represented by linear transformation from $V$, then $V$ is the generator of $E$. Intuitively, if any vector inside a vector space can be constructed, or represented using a system of linear combination, that is, combining vectors, then that system of vector is the generator. 

For example, the vector space $\mathbb{R}^{3}$ on $\mathbb{R}$ has the following system as generator: $$V_{\mathbb{R}^{3}}=\{e_{1}: (1,0,0); e_{2}: (0,1,0);e_{3}:(0,0,1)\}$$ since the combination $$e_{1}\lambda_{1}+e_{2}\lambda_{2}+e_{3}\lambda_{3} = \vec{x}, \vec{x}=(x_{1},x_{2},x_{3})$$ is valid. Considerably, we can write the vector $\vec{x}$ in vector space as $$\vec{x}=\begin{pmatrix}
1 \\
0 \\
0
\end{pmatrix}x_{1}+\begin{pmatrix}
0 \\
1 \\
0
\end{pmatrix}x_{2}+\begin{pmatrix}
0 \\
0 \\
1
\end{pmatrix}x_{3}$$ of which all the column matrices are $e_{1},e_{2}$ and $e_{3}$ accordingly. 

If L is the vector space generated from $\{V\}$, then we denoted $$L=
\mathcal{L}(\{\vec{V}_{i}\})$$
## II. Basis 

A basis is like a base of a building - anything of the building will be constructed from that. In vector space, we can see that a basis works the same way: anything is constructed using the basis. 

Hence, the definition of a basis is a system of vectors that is both a **generator** and **linear independent**. Formally, we will write them as

> [!thm] Basis Definition
> The vector system $S=\{\vec{V}_{i}\}, i=\bar{1,n}$ is a basis of $E$ if and only if (iff) for all $\vec{Q}\in E$, we can construct them from $S$, that is $$\vec{Q}= \sum_{i=1}^{n} \lambda_{i}\vec{V}_{i} $$

For this definition, we will use necessity and sufficiency for better understanding. 

> We say that **the statement A is a necessary and sufficient condition for the statement B when B is true if and only if A is also true**. That is, either A and B are both true, or they are both false. Note that if A is necessary and sufficient for B , then B is necessary and sufficient for A.

Hence, we will have our definition divided: 

1. Necessity: $S=\{\vec{V}_{i}\}$ is a basis, that means there exists only a unique $S$. 
2. Sufficiency: There is only one $S$, hence $S$ is a basis.

This is the definition given on class, but one should remind yourself that a basis is not unique. That is, there are more than one basis for any vector space, but the number of basis vector, the component vectors inside is the same. They just have to span the space, and be linear independent. 

#### Appendix I: Span of vector spaces 

The linear span of a set $S$ of vector in vector space $E$ is defined as the set of all linear combinations of the vectors in $S$. Given a vector space $E$ over field $F$, The span of a set $S$ of vectors (not necessary finite) is defined to be the intersection $W$ of all subspaces of $E$ containing $S$. Formulationally, we have  $$\operatorname {span} (S)=\left\{{\left.\sum _{i=1}^{k}\lambda _{i}\mathbf {v} _{i}\;\right|\;k\in \mathbb {N} ,\mathbf {v} _{i}\in S,\lambda _{i}\in K}\right\}$$
### II.1. Theorem and Consequences
#### Theorem 1
In vector space $E$, defined two vector systems $$\{\vec{u}_{1},\vec{u}_{2},\dots,\vec{u}_{m}\}\quad (1)$$ and $$\{\vec{V}_{1}, \vec{V}_{2},\dots,\vec{V}_{s}\}\quad (2)$$
If the first vector system is linear independent and each vector of $(1)$ can be represented by linear combination of $(2)$, then we say that $m\leq s$. Hence, we also have that if both $(1)$ and $(2)$ is linear independent, and the linear combination representation is available from $(1)\to (2)$ and reverse, $(2)\to (1)$ then we say that two vector systems are equal. 

From this, we have a theorem: 

> [!def] Theorem II.1.1
> If vector space $E$ has a finite basis including $n$ vectors, then all other basis also have $n$ vectors. 

Proof: Suppose that $E$ has a basis $\{f_{i}\}$, we have also $\{u_{j}\}$ such that for $i\in I = \{1,\dots,n\}$, $j\in J=\{1,\dots,m\}$, then $m>n$. Then because $\{f_{i}\}$ is a basis, $\{u_{i}\}$ can be represented by $\{f_{i}\}$. Hence $m\leq n$. But from the previous supposition, we have that $m>n$. Such claims is then contradictory hence the opposite must true. Q.E.D. 
___
## III. Dimension of Vector Space
The number $n$ of a basis is the dimension of a vector space. Formally, we denoted them as $$\operatorname {dim(S)}=n$$ of which $S$ is the vector space. Hence the dimension of a vector space is the total vectors required to describe any vectors in that space, hence it is also the number of vector in a basis of that vector space. 

If $K[x]$ is a infinite dimensional vector space, then $$\operatorname{dim}(K[x])=+\infty$$ and for zero vector $\vec{0}$, then $\operatorname{dim}(\vec{0})=0$. 
___
### II.1. (Continue) Theorem and Consequences 
We will continue with some of the theorem from vector spaces and basis.

> [!def] Theorem II.1.2 
> Given $E$, and $\operatorname{dim}(E)=nk^{2}$ Then we can add $(n-k)$ vectors into a $k$-vector linear independent vector system $$Sub=\{\vec{V}_{1}, \vec{V}_{2},\dots ,\vec{V}_{n}\}, \quad k < n$$ so the vector system becomes a basis of $E$. 

> [!thm] Theorem II.1.3
> If $E$ is a vector space with $\operatorname{dim}(E)=nk^{2}$ then 
> - The number of linear independent vectors that can be extracted from $E$ are $n$. 
> - Each vector system with $n$ vectors is a basis of $E$.
> - If $F$ is a subspace of $E$ then $\operatorname{dim}(F)\leq n$, equality happens only when $F=E$. 

