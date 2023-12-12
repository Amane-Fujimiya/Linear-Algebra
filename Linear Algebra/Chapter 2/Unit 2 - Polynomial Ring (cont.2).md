---
tags:
  - mathematics
  - linear_algebra
  - HUS
---
### 1.6. Polynomial on $\mathbb{C}$
We assume the following theorem as right, which can be used as axiom. 
> [!thm] Axiom/Theorem 1.6.1 
> Every polynomial $p(x)$ with $d^{\circ}(P(x))=n>0$ on $\mathbb{C}$ has complex root.

Consider $g(x)$ as a complex polynomial, with $d^{\circ} (g(x))=n>0$, then by axiom 1.6.1, we have that $g(x)$ has a complex root $a_{1}$. Then the polynomial can be written as: $$g(x)=(x-a_{1})q_{1}(x)$$ with $q_{1}(x)$ be a complex polynomial on $\mathbb{C}$. Then further assume that $q_{1}(x)$ is reducible, and has a complex root $a_2$, then $q_{1}(x)$ can be written as: $$q_{1}(x)= (x-a_{2})q_{2}(x)$$ Thus from here, we have that $$g(x)= (x-a_2)(x-a_{1})q_{2}(x)$$
Now, continuing this process assume that there is $q_{n}(x)$ to expand, then we will result in $$g(x)= b(x-a_{1})^{r_{1}}\cdots(x-a_{m})^{r_{m}}$$ with $b$ as the highest order coefficient, and $$r_{1}+\cdots r_{m}=n$$ additionally with $$a_{i}\neq a_{j}\: \forall i \neq j$$ $a_{i}$ is the rth complex root. 

### 1.7. Polynomial on $\mathbb{R}$
