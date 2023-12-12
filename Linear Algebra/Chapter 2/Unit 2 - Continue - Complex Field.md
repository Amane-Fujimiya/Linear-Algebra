---
tags:
  - HUS
  - linear_algebra
  - mathematics
---
# 2.2 Complex Field 
## 2.2.1 Structure
### 2.2.2.1 Definition

> [!def] Definition of Complex Set 
> A complex set $\mathbb{C}$ is a set $(\mathbb{R}\times\mathbb{R},+,\cdot)$ defined as: $$\mathbb{C} = \mathbb{R}\times \mathbb{R}= \{(x,y)\:|\:x, y \in \mathbb{R}\}$$

### 2.2.2.2 Properties of Complex Field 
Suppose we are given two complex numbers $z_{1} = (x_{1},y_{1}), z_{2}=(x_{2},y_{2})\in \mathbb{C}$, then $$z_{1}=z_{2}\iff x_{1}= x_{2} \:\land y_{1}=y_{2}$$
#### Addition and multiplication operation
Given two complex numbers $z_{1} = (x_{1},y_{1}), z_{2}=(x_{2},y_{2})\in \mathbb{C}$, we have $$z_{1}+z_{2}= (x_{1}+x_{2},y_{1}+ y_{2})$$
and $$z_{1}z_{2}= (x_{1}x_{2}-y_{1}y_{2},x_{1}y_{2}+x_{2}y_{1})$$
These two operators and the set $\mathbb{C}$ combined to give us a **complex field** $(\mathbb{C},+,\cdot)$. 

In this complex field, there are several parts inside that contributes to the properties

#### Properties (Main one)
$(\mathbb{C},+,\cdot)$ has: 
- An identity element $e = (0,0)$. 
- A complement element $\overline{z}=-(-x,-y)$.
- A unit element $i = (1,0)$ so that $$iTz = z$$
- An inverse element of $z=(x,y)$ such that $$z^{-1}=\frac{1}{z}=\left( \frac{x}{x^2+y^2},-\frac{y}{x^{2}+y^{2}} \right)$$ thus $$z\cdot z^{-1}=(1,0)=i$$
### 2.2.2.3 Representation of Complex Numbers
#### Equation form (basic)
We write the number $z=(a,b)$ in binary form as $$z=x + iy$$ with $i^{2} = -1$. Geometrically, we see that each complex number is an element of a field consists of two numbers, of which we separate it to real part $x$ and complex part $iy$. On graph, the complex part is the $Oy$ coordinate axis for 2D Cartesian coordinate system, and $x$ is the $Ox$ axis, as always. 

#### Trigonometric form 
For trigonometric form, we use polar coordinate representation of point, of which each value $z$ is a point on the 2D plane: $$z = r\cos{(\theta)}+r\sin{(\theta)}$$
Here $r$ is the distance from point $z$ to the polar, called module of $z$, denoted $|z|$, and is evaluated as $$|z| = \sqrt{x^{2}+y^{2}}=r$$
and the angle it makes with the $Ox$ axis is the angle $\theta$, evaluated using $$\tan{\theta}=\frac{y}{x}\longrightarrow \theta = \arctan{\left( \frac{y}{x} \right)}$$
and is called argument of $z$. Therefore, we have $$Arg(z)=\theta + 2k\pi$$ $2k\pi$ is necessary because when it is represented in polar coordinate, similar to trigonometric, a rotation of $2\pi$ (full circle) will return to the same position. Thus the angle with the value that can be presented as such will always point to a single position no matter the amount of rotation angle it gets. 

Multiplication and Division of complex number in trigonometric form can be written as
$$\frac{z_{1}}{z_{2}}=\frac{|z_{1}|}{|z_{2}|}\cdot (\cos{(\theta_{1}-\theta_{2})+i \sin{(\theta_{1}-\theta_{2})}})$$
and $$ z_{1}\cdot z_{2}= |z_{1}||z_{2}|\cdot [\cos{(\theta_{1}+\theta_{2})+i\sin{(\theta_{1}+\theta_{2})}}] $$
#### Conjugate of Complex Number 
A number $z^{*}$ is the conjugate of $z$, evaluated as $$z^{*}=a-bi=r[\cos{(\theta)}-\sin{(\theta)}]$$
### 2.2.2.4 De Moivre's formula
The De Moivre's formula stated that for all complex number $z$ and angle $x$, with integer $n$, then the below identity is true $$ z^{n} = r^{n}{\big (}\cos x+i\sin x{\big )}^{n}=r^{n}(\cos nx+i\sin nx)$$
### 2.2.2.5 $\sqrt[n]{z}$ of complex number $z = |z|(\cos{(x)}+i\sin{(x)})$

We have the general formula for this case as $$\sqrt[n]{z}= z_{k} = \sqrt[n]{|z|}\left[\cos{ \frac{\phi+k2\pi}{n} } + i \sin{\frac{\phi+k2\pi}{n} }\right]$$
### 2.2.2.6 Additional formula for calculating $sin(x)$ and $cos(x)$ for trigonometric form 
We have $$z = |z|(\cos{(\theta)}+ i \sin{(\theta)})$$ then we can calculate $$|z| = \sqrt{x^{2}+y^{2}}$$ while $$\sin(\theta)=\frac{y}{|z|}\quad \text{and} \quad \cos{(\theta)}=\frac{x}{|z|}$$
A key note while converting from algebraic form to trigonometric form is as follow: 
> [!note] Attention for missing cases 
> In missing cases, i.e, $z= 1+ 0i$, it is safe and recommended to use rather the above formula for $\sin(x)$ and $\cos(x)$ for the value of $\theta$ instead of $arctan()$, because the returning value can be both undetermined, or inaccurate

