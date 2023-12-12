---
tags:
  - HUS
  - linear_algebra
  - mathematics
---
### 1.3 GCD of Polynomial 
Definition: The common divisor of two Polynomial $P(x)$ and $G(x)$ is $d(x)$ such that $$d
\mathrel{\vdots} P(x)\quad \text{and} \quad d \mathrel{\vdots} G(x)$$
Then $d(x)$ is called GCD of $P(x)$ and $G(x)$ if $D(x)$ is divisible to all common divisor of $P(x)$ and $G(x)$ 
A property of $d(x)$ is presented. Suppose that $$d
\mathrel{\vdots} P(x)\quad \text{and} \quad d \mathrel{\vdots} G(x)$$ then $$d \mathrel{\vdots} [P(x)\pm G(x)]$$ and $$d\mathrel{\vdots}F(x)\cdot G(x)$$
### 1.4 Properties of GCD of Polynomial
> [!note] Property 2. 
> Each GCD of a pair of polynomial $P(x), G(x)\neq 0$ is different by one zeroth order $(n=0)$ factor. 

> [!note] Property 3.
> If $d(x)$ is the GCD of $P(x)$ and $G(x)$, then $a\cdot d(x)$ is also a GCD of $P(x), G(x)$ with $a \in K, a \neq 0$

> [!important] Norm form of GCD
> If $P(x)$ and $G(x)$ both has a GCD, then there exists only one norm form, or original form of the GCD. This is from the property 3 of which $a\cdot d(x)$ is also a GCD, thus $d(x)$ is the original GCD and exists only one. 

The **norm form - original GCD** is denoted as $$(f(x)\:;\:g(x))$$ for every two polynomials $f(x),g(x)$
Apart from those, we will also have a general theorem for GCD of polynomials: 

> [!thm] Existence of GCD
> There is always GCD for every pair $P(x)\neq 0$, $G(x)\neq 0$

#### Prime polynomial 
Two polynomials are called **prime polynomial** if for $f(x),g(x)\neq 0; f(x), g(x) \in K[x]$, then they have $$(f(x)\:;\: g(x))=1$$
From this, we have a theorem: 

> [!thm] Theorem of prime polynomial
> Two polynomials $f(x)\neq 0$ and $g(x)\neq 0$ are both prime polynomial if and only if there is two polynomial $u(x),v(x)\in K[x]$ such that $$f(x)u(x)+g(x)v(x)=1$$ 

### 1.5 Irreducible Polynomials
A polynomial $P(x)\neq 0$ of degree $n$ is called **irreducible** if it cannot be factored into $$P(x)=P_{1}(x)\cdot P_{2}(x)$$  of which $$0<d^{\circ}(P_{1}(x), P_{2}(x))<n$$
From this, we also can say that all degree 1 polynomials are irreducible. And hence, all polynomial with degree $n\geq2$ irreducible on $K[x]$ will have no root in $K[x]$, that is, undefined in such ring. Thus the irreducible property of polynomial depends on the property of ring $K$. 

