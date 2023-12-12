---
tags:
  - mathematics
  - linear_algebra
  - HUS
---
## III. Logics operation
Given two sets $A$ and $B$, some operations on them are

### 1. Union
Union of $A$ and $B$ is $$A\: \cup B = \{x: x \in A \: or \: x \in B\}$$
### 2. Intersection 
Intersection of $A$ and $B$ is $$A \cap B = \{x:x\in A \: and \: x \in B\}$$
### 3. Difference
The difference between $A$ and $B$ is $$A \setminus B =\{x: x\in A \: and \: x \notin B\}$$
If $A \cap B = \varnothing$, then $A$ and $B$ are disjoint. If $A \subseteq X$ then the notation $C_{X}A= X \setminus A$ is the complement of $A$ in $X$. 
___
The union of a family of sets is denoted as $$\bigcup_{i \in I} A_{i} = \{x: \exists i \in I, x \in A_{i}\}$$
The intersection of a family of sets is denoted as $$\bigcap_{i\in I} A_{i}=\{x: x\in A_{i}, \forall i \in I\}$$
### 4. Properties of set operation
#### Commutativity 
$$
\begin{align}
A \cup B = B \cup A \\ \\
A \cap B = B \cap A
\end{align}
$$
#### Associativity 
$$
\begin{align} \\
(A\cup B)\cup C = A \cup (B \cup C)  \\
(A \cap B) \cap C = A \cap (B \cap C)
\end{align}
$$
#### Distributivity 
$$
\begin{align} \\
A \cup (B \cap C) = (A \cup B) \cap (A \cup C) \\
A \cap (B \cup C) = (A \cap B) \cup (A \cap C)
\end{align}
$$
#### De Morgan Theorem
We have: 
$$X\setminus \left(\bigcup_{i \in I} A_{i}  \right)=\bigcap_{i \in I} (X \setminus A)$$

$$X\setminus\left(\bigcap_{i \in I} A_{i}\right)= \bigcup_{i \in I} (X \setminus A_{i})$$

