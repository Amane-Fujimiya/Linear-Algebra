---
tags:
  - linear_algebra
  - mathematics
  - HUS
---
# Unit I. Set and Relations
## I. Set 
A set is a collections of objects, either algebraic structures, rigorous mathematics, or plain simple objects such as a collection of collected apples during harvest seasons. 

A set $X$ will have its collection of objects inside. If an object $x$ is inside $X$, or $x$ in $X$, we write it as $$x \in X$$
with the notation $\in$ as the representation.
### Describing a set 
To describe a set, we use some way of listing the set: 
#### 1. Listing elements of a set 
Example includes: 
$$\mathbb{N}=\{0,1,2,\cdots\}$$
of natural numbers set $\mathbb{N}$. For integer $\mathbb{Z}$, then $$\mathbb{Z}=\{0,\pm1,\pm2,\cdots\}$$
and for rational number: $$\mathbb{Q}=\left\{r= \frac{m}{n}:m,n\in \mathbb{Z},n \neq 0 \right\}$$

#### 2. Identification of set's properties
If a set $E$ includes elements with some types of properties, we write $$E=\{x:T(x)\}$$
For example, the set $P$ of all even numbers is $$E=\{x:x=2k,k\in \mathbb{Z}\}$$
This is explained as for all even number, there is a properties that $x=2k$ for all $k\in \mathbb{Z}$, that is, $x$ must have an even factor of $2$. 
___

### Subset. Empty set
For any set $X$, given another set $A$. $A$ is the subset of $X$ if $x\in A$ then $x \in X$, denoted $$A \subseteq X$$ or $$X \supseteq A$$
The first notation is the subset notation, the second one establish a reverse relation, called superset, that is $X$ is a superset of $A$. If $A \subseteq X$, and we have $y \in X$ but $y \notin A$, then $A$ is a proper subset of $X$, denoted $$A\subset X$$
An empty set is a set that contains no elements. It is denoted as $\varnothing$. Conventionally, $\varnothing \in X$ for all $X$. 

Two sets $A$ and $B$ is equal if $A \subseteq B$ and $B \subseteq A$, then $A = B$. 

### II. Logic notations

A mathematical statements can be either right or wrong, no more. To simplify and generalize the wording (and to shorten the sentence), we use those notations: 
1. $S \Rightarrow T$ means $S$ is right then $T$ is right. 
2. $S \iff T$ means that $S$ is right then $T$ is right and the reverse is true. 
3. $\forall x \in X: S$ means for all $x$ in $X$ there is a statement $S$. 
4. $\exists x \in X:S'(\exists! x \in X: S)$ means that there exists one and only $x \in X$ so that $S$ is right. 

