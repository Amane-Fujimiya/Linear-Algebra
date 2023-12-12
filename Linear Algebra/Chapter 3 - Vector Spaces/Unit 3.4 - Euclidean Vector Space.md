---
tags:
  - HUS
  - mathematics
  - linear_algebra
---
# I. Definition
A vector space $E$ on $\mathbb{R}$ is called a Euclidean vector space if it is equipped with another operation called dot/scalar product, as a linear transformation function $$\varphi: E\times E \longrightarrow \mathbb{R}$$ such that $$(\vec{x},\vec{y})\to \varphi (\vec{x},\vec{y})\equiv (\vec{x} \cdot \vec{y}) = \sum_{i=1}^{n} (x_{i} y_{i}) $$ and satisfies some properties given
$$
\begin{cases}
(( \vec{x}+ \vec{x'} )\cdot \vec{y}) = ( \vec{x} \cdot \vec{y} ) + (\vec{x'} \cdot  \vec{y})  \\
\lambda  \vec{x} \cdot  \vec{y} = \lambda (\vec{x} \cdot  \vec{y}) & \forall  \vec{x},  \vec{y} \in E, \lambda \in \mathbb{R} \\
\vec{x} \cdot  \vec{x} \geq 0 \longrightarrow \vec{x} \cdot  \vec{x} = 0 \implies \vec{x} = \vec{0}  \\  
[\vec{x} \cdot  (\vec{y}+  \vec{y'})] = (\vec{x}\cdot  \vec{y}) + (\vec{x}\cdot  \vec{y'}) \\
(\vec{x}\cdot \lambda  \vec{y}) = \lambda (\vec{x} \cdot  \vec{y})
\end{cases}
$$
# II. Features of Euclidean Space
For each vector, the length is $$|\vec{x}|=||\vec{x}|| = \sqrt{ \vec{x}\cdot  \vec{x} }=\sqrt{ \left(\sum_{i=1}^{n} x_{i}\right)^{2} }$$
The angle $\theta$ between two intersecting vectors $\vec{x},  \vec{y} \neq \vec{0}$ is defined as $$\cos{(\theta)}=\frac{\vec{x}\cdot  \vec{y}}{||\vec{x}||\cdot ||\vec{y}\mid}= \frac{\left(\displaystyle\sum_{i=1}^{n} (x_{i} y_{i})\right)}{\displaystyle\sqrt{ \left(\sum_{i=1}^{n} x_{i}\right)^{2} \left(\sum_{i=1}^{n} y_{i}\right)^{2}}}$$
### Cauchy-Schwarz Inequality for Vector 
If $\vec{x},  \vec{y}\in E$, then $$||\vec{x}\cdot  \vec{y}|| \leq ||\vec{x}|| \cdot ||\vec{y}||$$ The proof can be found [[Proof of Cauchy-Schwarz Inequality|here]]. 
From this, we also get that $$\left|\sum_{i=1}^{n} (x_{i} y_{i})\right|\leq \sqrt{ \left(\sum_{i=1}^{n} x_{i}\right)^{2}} \cdot \sqrt{ \left(\sum_{i=1}^{n} y_{i}\right)^{2}}$$ and $$\left|\int_{a}^{b} g(t)f(t) \, dt \right| \leq  \left| \sqrt{\int_{a}^{b} f^{2}(t) \, dt } \right| \cdot  \left|\sqrt{\int_{a}^{b} g^{2}(t) \, dt }\right| $$
of which can be expressed as $$\left|\lim_{ n \to \infty } \sum^{n}_{i=1} g(x_{i})f(x_{i}) \Delta x \right|\leq \left|\lim_{ n \to \infty } \sum^{n}_{i=1} f(x_{i}) \Delta x \right| \cdot \left|\lim_{ n \to \infty } \sum^{n}_{i=1} g(x_{i}) \Delta x \right|$$
### Triangle Inequality 
For all $\vec{x}, \vec{y} \in E$, we have the triangle inequality: $$||\vec{x} + \vec{y}|| \leq ||\vec{x}|| + ||\vec{y}||$$
### Pythagoras Theorem
For all $\vec{x},\vec{y}\in E$, we have $\vec{x}\cdot  \vec{y}=0$ if $$||\vec{x}+\vec{y}||^{2}=||\vec{x}||^{2}+||\vec{y}||$$
### Orthogonality of Vector System 
If a vector system $W$ contains $$W=\{\vec{u}_{1}, \vec{u}_{2},\dots,\vec{u}_{n}\}$$ of which $\vec{u_{n}}\neq \vec{0}$ and each of them is mutually orthogonal, that is $\vec{u}_{1} \cdot \vec{u_{2}}=0, \vec{u_{2}}\cdot  \vec{u}_{3}=0$ and so on. Then the system is linear independent. 
**Proof**: Suppose we have 
$$\sum_{i=1}^k \lambda_{i}\vec{u}_{i}=\vec{0}$$ This turns into 
$$
\begin{split}
\sum_{i=1}^{k} \lambda_{i}\vec{u}_{i} & \iff \sum_{i=1}^{k} \lambda_{i}\vec{u}_{i} \vec{u}_{j} =  \vec{0} \cdot  \vec{u}_{j} \\
& \iff \sum_{i=1}^{k} \lambda_{i}(\vec{u}_{i} \cdot  \vec{u}_{j}) = 0\\
& \iff \lambda_{i} ||\vec{u}_{j}||^{2}=0 \rightarrow \lambda_{i} = 0 \quad \forall j \in \{1,\dots,k\}, k = n
\end{split}
$$
We also see that in this proof, we have $j$ as the additional variable, of which is not strongly defined: $$\lambda_{i} (\vec{u}_{i} \cdot  \vec{u}_{j}) \longrightarrow \begin{cases}
\forall i \neq j \\
\forall i = j
\end{cases}$$
But because we are considering Euclidean vector space, hence $\vec{u}_{i} \cdot \vec{u}_{j}=0\: \forall i = j$. Hence the result will stay the same for any redundancy. Thus the proof is concluded. 
