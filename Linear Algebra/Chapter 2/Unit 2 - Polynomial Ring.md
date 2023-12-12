---
tags:
  - HUS
  - mathematics
  - linear_algebra
---
## 1. Definition
A polynomial ring is a ring of polynomials such as $P(n)$, and each element of the ring is defined as: 
$$P(n)=a_{n}x^{n}+\cdots + a_{1}x^{1}+a_{0}=\sum\limits_{i=0}^{n}a_{i}x^{i}$$
For two polynomials $P(n)$ and $G(m)$ to be equal, then $$a_{n}=b_{m},\forall m,n \in I = \{1,\cdots,n\}$$
The degree of a polynomial is denoted $d^{\:\circ} P(n)$ and evaluated to $n$, or $$d^{\:\circ} P(n)=n$$
### 1.1 Ring operations
Given a polynomial ring $(K,+,\cdot)$, this ring has two operation $+$ and $\cdot$ defined as below

> [!def] Polynomial Summation Operation
> Given $$P(n)=\sum\limits^{n}_{k=0}a_{k}x^{k}$$ and $$G(m)=\sum\limits^{n}_{k=0}b_{k}x^{k}$$ with $k\in I =\{1,\cdots,n\}$, the operation $P(n)+G(n)$ is defined to be $$P(n)+G(m)= \sum\limits_{k=0}^{n}(a_{k}+b_{k})x_{k}=\sum\limits_{k=0}^{n} C_{k}x^{k}\:, \: \forall m \leq n, C_{k}= a_{k}+b_{k}$$

> [!def] Polynomial Product Operation
> Given $$P(n)=\sum\limits^{n}_{k=0}a_{k}x^{k}$$ and $$G(m)=\sum\limits^{n}_{k=0}b_{k}x^{k}$$ with $k\in I =\{1,\cdots,n\}$, the operation $P(n)\cdot G(n)$ is defined to be $$P(n)\cdot G(n)= \sum\limits^{n+m}_{s=0}\left[\sum\limits_{R(k,l): k + l = s} (a_{k}b_{l})x^{s}\right] = \sum\limits_{s=0}^{n+m} D_{s} x^{s} \: \text{with} \: \left(D_{s}= \sum\limits_{R(k,l): k+l = s} a_{k}b_{l}\right) $$

### 1.2 Polynomial Division and Euclidean Division Algorithm for Polynomial 
Given $G(x)$ and $P(x)$ as two polynomial in ring $(S,+,\cdot)$, we have the division of them, $$\frac{P(x)}{G(x)}$$ defined as $$\frac{P(x)}{G(x)}= H(x), R(x) \: \text{such that}\: P(x) = H(x)G(x) + R(x) $$ with $d^{\:\circ}R(x)< d^{\:\circ}G(x)$. Same for Euclidean division of normal number, $P(x)$ is the dividend (the one being divided), $G(x)$ is the divisor (the one that divides the dividend) and $H(x)$ is the quotient, while $R(x)$ is the remainder polynomial. 
#### 1.2.1 Division Algorithm 
All elementary school long division. Divide by the highest degree variable, then multiply back the divisor and take the dividend subtract the divisor, and repeat the process. This is called polynomial long division, albeit there is indeed another one called short division.

### 1.2(2) Root of polynomial 
#### Definition
A element $\alpha\in K$ is called the root of a polynomial with degree $n>0$ if we replace $\alpha$ for $x$, we have $$f(x)=a_{n}\alpha^{n} + \cdots + a_{1}\alpha + a_{0}=0$$
Then, we have a statement about this

> [!summary] Statement 1
> The element $\alpha \in K$ is the root of $f(x)\in K[x]$ with degree $n >0$ if and only if $$f(x) | (x-\alpha)$$


> [!def] Definition of multiple root
> For polynomial $f(x)\in K[x]$ with $n >0$, the element $\alpha \in K$ is called a multiple root if $$f(x)\:|\: (x-\alpha)^k$$ but not for $(x-\alpha)^{k+1}$
> 

From all of this, we can say that a polynomial $f(x)$ with $n>0$ be its degree **does not have more than $n$ root, even with multiple root** 

