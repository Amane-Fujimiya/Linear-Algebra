---
tags:
  - mathematics
  - linear_algebra
  - HUS
---
## II. Set relations
### Descartes Product of sets
Given two sets $X$ and $Y$, then the Cartesian product (or Descartes product) $X \times Y$ is defined as $$\displaystyle A\times B=\{(a,b)\mid a\in A\ {\mbox{ and}}\ b\in B\}$$
Generally, for a set of sets $S_{i}$ with $i \in I$ $$S_{i}=\{S_{1,}S_{2}, S_{3},\cdots\}$$
The Cartesian product of elements in $S_{i}$ is $$\prod_{i=1}^{n} S_{i} = \{x = (x_{1}, x_{2}, \cdots , x_{n}): x_{i} \in S_{i,}i = 1,2,\cdots,n\}$$
If $S_{1}=S_{2}=\cdots S_{n}$ then we have $S_{1}\times S_{2} \times \cdots \times S_{n}= S^{n}$. This is called n-nary Cartesian/Descartes product of $S_i$. 

### Relations
> Definition: Given a set $X$, then each $S \subset X \times X$ is an relation on $X$

If the ordered pair $(x,y)\in S$ then we say that $x$ is in relation $S$ with $y$, denoted $xSy$. Then we have: 
> Suppose $S$ is an relation on $X$, then 
> - $S$ is called reflexive relation if $x S x, \forall x \in X$. 
> - S is called symmetric if $xSy$ then $ySx$. 
> - S is called transitive if $xSy$ and $ySz$ then $xSz$. 
> - S is called anti-symmetric if $xSy$ and $ySx$ then $x=y$. 

#### 1. Equivalent relation
> Definition: An equivalent relation is a relation that has reflective, symmetric and transitive properties. 

Notation for equivalent relation is $\sim$, then $xSy \rightarrow x \sim y$ for equivalent relation
For each $x$, we set $$\bar{x}=\{x' \in X: x' \sim x \}$$
then $\bar{x}$ is called an equivalent class with $x$ as it main. By reflective properties then $$x \in \bar{x}$$
then $$\bar{x} \neq \varnothing,\: \bigcup_{x \in X} \bar{x}=X$$
**Class separation**: The family of subsets $\{A_{i}\}_{i \in I}$ of $X$ is called a class separation of $X$ if $A_{i}\neq \varnothing$ for $\forall i \in I$. A property of this is that $$A_{i}\cap A_{j}=\varnothing\:\: if\:\: \left(i \neq j, \bigcup_{i \in I} = X\right) $$
The set of all equivalence classes of $X$ is denoted $X \setminus \sim$. Notationally, $$X\setminus \sim = \{\bar{x}| x \in X\}$$
#### 2. Ordering relation
An ordering relation on a set is a relation that is reflexive, transitive, and anti-symmetric.
An ordering relation is often denoted $\leq$, and has these following properties: 
> [!lem] Ordering relation properties
> 1. $x \leq x, \forall x \in X$
> 2. $x\leq y, y \leq z \Rightarrow x \leq z$
> 3. $x \leq y, y \leq x \Rightarrow x = y$

If $x \leq y$ then we say that $x$ stands before $y$, or the reverse. If $x \leq y$ and $x \neq y$ then we say that $x$ is totally behind $y$ and we write $x < y$. 

A set $X$ that has an ordering relation is called an ordered set and denoted $(X, \leq)$. If for all $x,y \in X$ we always have $x \leq y$ or $y \leq x$ then the set is a totally ordered set (totality of a set).