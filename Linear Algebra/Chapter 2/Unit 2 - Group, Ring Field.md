---
tags:
  - mathematics
  - linear_algebra
  - HUS
---
## U2.1 Group, Ring, Field
### 2.1.1. Binary operation
#### Definition
> [!def] Definition
> Suppose $X$ is a set. then a mapping $\theta: X \times X \longrightarrow X$ is a binary operation on $X$.

Then $\theta(x,y)$ is the result of $x$ and $y$, or the product of those two. 
#### Binary properties
Considering a binary operation $\theta$ on $X$, then $\theta$ is called: 
- Associative if $$(x\cdot y)\cdot z=x\cdot(y\cdot z), \forall x,y,z\in X$$
- Symmetric if $$x\cdot y = y \cdot x, \forall x,y \in X$$
- There exists an identity element $e$ that $$\forall e,x \in X, e\cdot x=x \cdot e = x$$
From the third conditional, we then have a proposition: 
> [!thm] Proposition 
> For all binary operation and set $X$, there is only one identity element. 

The proof is easy because by definition, we suppose an element $e'$ which is also an identity element. Then because of that $e\cdot e' = e'$ and this is equal to $e$. Thus $e'$ and $e$ are the same. QED. 
##### Inverse element
An element $x \in X$ is called an inverse element if there exists $y \in X$ that $$x\cdot y = y \cdot x = e$$
> [!thm] Proposition 2
> If the binary operation $\theta$ has associative properties then for each $x \in X$, there exists only one inverse element denoted $x^{-1}$

#### Internal binary operation
Definition of internal binary operation can be as follow: 

> [!def] Definition 2.2
> A binary operation on a non-empty set $S$ is any mapping $$f: S \times S \longrightarrow S$$
> such operation with $x,y\in S$ and the operation $f$ result in $f(x,y)\in S$ is called an **internal binary operation**, denoted $T$

Thus, the binary operation $f: x,y\mapsto x+y$ is an internal binary operation in $\mathbb{R}$.
#### External binary operation
In cases that we want the cartesian product to contain another set, i.e., the mapping of of both set onto one other, we can define the inverse of an internal binary operation: 

> [!def] Definition 2.3
> A binary operation on $S\notin \varnothing$ $$f: S \times F \longrightarrow S$$ with F is another set. 
> Comprehensively, this is similar as $x\in S$, $y \in F$ then $f(x,y)\in S$, then the binary operation is called an **external binary operation**, denoted $\perp$ 

#### Homomorphism and Isomorphism
A homomorphism is a map between two algebraic structure of the same type that preserve the operation of the structures. 

> [!def] Homomorphism 
> A mapping $f:E\longrightarrow F$ with $F$ as a set with an internal binary operation $T$, and a set $E$ with binary operation $T'$, and both have an external binary operation $\perp$ on a set $\Omega\not\subseteq F,E$. Then, $f$ is a homomorphism if it satisfies: $$f(x\:T\:y) = f(x)\:T'\:f(y), \forall x,y \in E$$ and $$f(\lambda \perp x) = \lambda \perp ' f(x) \forall x \in E, \forall \lambda \in \Omega$$

For this, we can say that $E$ and $F$ have a homomorphism $f$ with them. If a homomorphism is also bijective, that is, one-on-one correspondence, then the homomorphism $g$ is called an isomorphism. For this, it means that for each $h: E \longrightarrow F$ there exists a mapping $h':F\longrightarrow E$ that satisfies all the aforementioned properties.

After this, now we have the tools to appropriately describe three main types of algebraic structure: group, ring and field. 
### 2.1.2 Group
> [!def] Definition
> Let $G$ be a non-empty set with binary operation $T$. Then $(G,T)$ is called a group if the following holds: 
> - (G1) Binary operation $T$ is associative: $$xT(yTz)= (xTy)Tz$$
> - (G2) $G$ has an identity element with respect to $T$, that is $\exists e\in G, \forall x \in G, xTe = eTx = x$
> - (G3) $\forall x \in G, \exists h \in G$ such that $gTh=hTg=e$, meaning $h$ is an inverse element of $g$ and reverse. 

If a group is also commutative, that is $$xTy = yTx\:\forall e \in G$$ then we call it an **Abelian group**. 

#### Subgroup
> [!def] Subgroup definition
> Let $G$ be a group. Then for $H\subseteq G$ we called $H \neq \varnothing$ a subgroup of $G$ if, for $H$ with binary operation $T$, 
> - $x,y\in H$ then $xTy\in H$
> - $x\in H$ then $x^{-1}\in H$
> - $e\in G$ then $e\in H$
> 
> Further in, if $H\neq G$ then we say $H$ is a **proper subgroup** of $G$.

### 2.1.3 Group Homomorphism, Group Isomorphism
#### Group Homomorphism
> [!def] Group Homomorphism Definition
> Given $E,F$ as groups. A homomorphism from $E$ to $F$ is a function mapping $f:E\longrightarrow F$ such that $$f(xTy)=f(x)T'f(y),\forall x,y \in G$$ with $T$ as the binary operation on $E$ and $T'$ on $F$. This is called a **group homomorphism**

Group homomorphism is often referred to as group map for short. 
#### Group Isomorphism
> [!def] Group Isomorphism Definition
> If a group homomorphism $f: E \longrightarrow F$ is also bijective, then $f$ is called a group isomorphism, with two group $(E,*)$ and $(F,\odot)$ Two groups are isomorphic if there exists an isomorphism from one to the other, written as $$(E,*)\cong (F,\odot)$$

### 2.1.4 Ring
> [!def] Ring definition
> An algebraic structure $(R,+,\cdot)$ is called a ring if for $R\neq \varnothing$ and two binary operation $+$ and $\cdot$, such that 
> 
> **Addition**: $(R,+)$ is an Abelian group. that is: 
> - $\forall a,b,c\in R, a+(b+c)=(a+b)+c$
> - $\exists e\in R,\forall a \in R \rightarrow a+e=e+a=a$
> - $\forall a \in R, \exists! -a \in R\:\text{such that}\:a+(-a)=(-a)+a=0$
> - $\forall a,b \in R, a+b=b+a$
> 
> **Multiplication**: 
> - $\forall a,b,c\in R$, we have $a\cdot(b\cdot c)=(a\cdot b)\cdot c$
> 
> **Addition and multiplication together** 
> - $\forall a,b,c \in R$, $$a\cdot (b+c)=a\cdot b + a \cdot c$$ and $$(a+b)\cdot c=a\cdot b+ b\cdot c$$

#### Subring 
> [!def] Subring definition
> Let $R$ be a ring and $S\subset R$ be a subset. We say $S\subset R$ is a subring if 
> - $S$ is closed under addition and multiplication: $$r,s\in S\implies r+s, r\cdot s \in S$$
> - $S$ is closed under additive inverses: $$r\in S \implies r^{-1} \in S$$
> - $S$ contains the identity $1_{R}\in S$

Here, the word closed means that for all operation, the result is also in the set of the subring. 

#### Commutative Ring
> [!def] Definition of Commutative Ring
> A commutative ring $(K,+,\cdot)$ is a ring that the multiplication binary operation is commutative: $$x\cdot y = y \cdot x ;\forall x, y \in K$$

#### Ring Homomorphism 
Given $(K, +, \cdot)$ and $(K',+,\cdot)$ are the given rings. We said that $$f: K \longrightarrow K'$$ is a ring homomorphism if $$f(x+y)=f(x)+f(y)$$
and $$f(x\cdot y)= f(x)\cdot f(y)$$
As we see, each ring homomorphism is a mapping that conserves the mathematical operation of the structure. 
If $f$ is also bijective then we say that $f: K \longrightarrow K'$ is a **ring isomorphism**. 

### 2.1.5 Field
> [!def] Definition of a field 
> A structure $(R,+,\cdot)$ where $+$ and $\cdot$ are two binary operation on $R$ is a field if 
> (A). $(R,+)$ is an Abelian group. 
> (B). $(R\setminus \{0\},\cdot)$ is an Abelian group. 
> (C). The distributive laws hold. 

A more "easy definition" of a field is as followed. 

> [!def] Field definition
> A field is a **commutative ring** $(K, +,\cdot)$ with unit $1 \neq 0$, and $$\forall x \neq 0, \exists x^{-1}\in K\: \text{such that}\: x\cdot x^{-1}=1$$

#### Subfield 
Given that $(K,+,\cdot)$ is a field. Then the subfield of $(K,+,\cdot)$ is a ring $P\neq \{0\}$ that satisfy: $$\forall x \in P,\: \text{if}\: x \neq 0 \implies x^{-1}\in P$$







