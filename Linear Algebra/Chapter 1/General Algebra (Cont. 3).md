---
tags:
  - linear_algebra
  - mathematics
  - HUS
---
## 2. Function images
### Definition 
> [!def] Definition
> A map $f$ from $X$ to $Y$, denoted $f: X \longrightarrow Y$ or $X \longrightarrow^{f} Y$ is a rule that bind each $x \in X$ with exactly one $y = f(x) \in Y$.

#### Composition of maps
Given two maps $f: X \longrightarrow Y$ and $g: Y \longrightarrow Z$, the product or composition of two maps $f$ and $g$ is $g \circ f: X \longrightarrow Z$ and is defined as $$g \circ f = g(f(x)), \forall x \in X$$
The image of $A \subseteq X$ through the map $f$ is the set $$f(A)= \{f(x):x\in A\}$$
Denoted as $Imf=f(X)$, the set $Imf$ is called image of mapping $f$. 
The inverse image of $D \subseteq Y$ is the set $$f^{-1}(D)=\{x\in X: f(x)\in D\}$$
#### Types of mappings
For a mapping, there are three types of mapping, which is injective, bijective and surjective. We will then go to define such mapping style. 
##### Injection mapping
A map $f$ is injective if $$\forall x , x' \in X, x \neq x' \Rightarrow f(x)\neq f(x')$$
This can be written also as $$\forall x, x' \in X, f(x)=f(x')\Rightarrow x = x'$$
##### Surjection mapping
A map $f$ is surjective if $$Imf=Y$$
In more detail, that is $$\forall y\in Y,\exists x\in X{\text{ such that }}y=f(x).$$
##### Bijection mapping
A map $f$ is bijective if $f$ is both surjective and injective. Comprehensively,
$$\displaystyle \forall y\in Y,\exists !x\in X{\text{ such that }}y=f(x)$$
> [!important] Composition of injection, bijection and surjection
> Composition of injective mappings are an injective mapping, so do surjective, thus we also have bijection mappings to have bijective compositions

#### Reverse Mapping
Suppose $f: X \longrightarrow Y$ is a bijective mapping from $X$ to $Y$. Then for each $y \in Y$, there exists one and only $x\in X$ so that $f(x)=y$. Then we have a mapping $g: Y \longrightarrow X$ defined as $$\forall y \in Y, x \in X: g(y) = x, f(x) = y \Longrightarrow g \circ f= i_{X}, f \circ g = i_{Y}$$
Here, we have the mapping called identity mapping, which will be talked later on, at least right after this section. 
##### Identity Mapping/Function
The **_identity function_** on any nonempty set $A$ maps any element back to itself: $$I_{A}=i_{A}:A \longrightarrow A, I_{A}(x)=x$$
___
Then, the mapping $g$ is called a reverse mapping of $f$ and denoted $f^{-1}$

### Equivalence functions (same 'force' relation)
#### Definition
> [!def] Equivalence functions
> Two sets $X$ and $Y$ is called equivalent, that is $X \sim Y$ if there exists a bijective relation $f: X \longrightarrow Y$. 

___
We will inspect some properties of equivalence function, by defining a mapping $E_{n}$, that is $$f: E_{n}\rightarrow A, f(k)=a_{k} \forall k \in K=\{1, 2,\cdots, n\}$$
