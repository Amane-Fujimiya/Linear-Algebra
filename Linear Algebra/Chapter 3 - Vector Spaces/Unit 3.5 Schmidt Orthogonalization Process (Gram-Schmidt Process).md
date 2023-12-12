---
tags:
  - HUS
  - mathematics
  - linear_algebra
---
# Definition and Procedure
The Gram-Schmidt Process of Orthogonalization is the procedure for generating, or creating from a spanned vectors set a orthogonal vectors set. That is formally:
> [!attention] Lemma 1.
> If $S= \{\vec{V}_{1}, \vec{V}_{2},\dots,\vec{V}_{n}\}$ a linear independent system of vectors in $V$, then there exists an orthonormal vector system $\{e_{1},e_{2},\dots,e_{n}\}$ such that $$span(\{\vec{V}_{1}, \vec{V}_{2},\dots,\vec{V}_{n}\})=span(\{e_{1},e_{2},\dots,e_{n}\})$$ that is, the orthonormal vector system spans or cover the same spaces of the original linear independent system. 

The proof for this lemma will be provided [here](https://math.libretexts.org/Bookshelves/Linear_Algebra/Book%3A_Linear_Algebra_(Schilling_Nachtergaele_and_Lankham)/09%3A_Inner_product_spaces/9.05%3A_The_Gram-Schmidt_Orthogonalization_procedure#). As for now, we will elaborate on the procedure. 

To create an orthonormal system of vectors, we first also have to distinguish between orthogonal and orthonormal. Suppose we have two vectors, $\vec{v}$ and $\vec{u}$, then they are orthogonal if their inner product is $0$, or $$\langle \vec{v}, \vec{u} \rangle= 0$$ and this also means that $\vec{v}\vec{\perp}u$, and $\theta(\vec{v},\vec{u})=90^{\circ}$. 
Orthonormality is defined differently, that is given two or more vectors, $(v_{1},v_{2}, v_{3},\dots v_{n})$, then they are orthonormal if: 
- They are mutually orthogonal, that is, if a vector system $W$ contains $$W=\{\vec{u}_{1}, \vec{u}_{2},\dots,\vec{u}_{n}\}$$ of which $\vec{u_{n}}\neq \vec{0}$ and each of them is mutually orthogonal, that is $\vec{u}_{1} \cdot \vec{u_{2}}=0, \vec{u_{2}}\cdot  \vec{u}_{3}=0$ and so on. In this case, we have our vectors $(v_{1},v_{2}, v_{3},\dots v_{n})$ in consideration. 
- The magnitude of each vectors is equal to 1, which is the unit/normal vector according to each vectors, and is calculated by $$unit(v_{1}) = \frac{v_{1}}{\lvert  \rvert \lvert v_{1} \rvert  } $$
Given two vectors, $v$ and $u$, the projection of $v$ on $u$ is defined as $$proj_{u}(v)= \frac{\langle v,u\rangle}{\langle u,u\rangle} u$$ where $\langle v,u\rangle$ denotes the inner (dot) product between $u$ and $v$. This effectively means that $proj_{u}(v)$ is the orthogonal projection of $v$ onto the line spanned by $u$. 

Given $k$ vectors $\vec{v}_{1},\dots \vec{v}_{n}$, the Gram-Schmidt procedure defines the vectors $e_{1},e_{2},\dots,e_{n}$ as
$$
\begin{split}
\vec{e}_{1 }&= \vec{v}_{1}\\
\vec{e}_{2} & = \vec{v}_{2}  - proj_{\vec{e}_{1}}(\vec{v}_{2}) = \vec{v}_{2}- \frac{\langle \vec{v}_{2},\vec{e}_{1}\rangle}{\langle \vec{e}_{1},\vec{e}_{1}\rangle} \vec{e}_{1}\\
\vec{e}_{3} & = \vec{v_{3}} - proj_{\vec{e}_{2}}(v_{3}) - proj_{\vec{e}_{1}}(\vec{v_{3}})\\
&\;\;\vdots \notag \\
\vec{e}_{k} &= \vec{v}_{k} - \sum_{i=1}^{k-1} proj_{\vec{e}_{i}} (\vec{v}_{k})
\end{split}
$$
This effectively takes the line spanned by each dimension of each vectors used, without overlapping of one another. For example, given a system of vector $$\left(T=\begin{bmatrix} 
14 \\
5 \\
9
\end{bmatrix}
,
\begin{bmatrix}
24 \\
48 \\
17
\end{bmatrix}
,
\begin{bmatrix}
11 \\
12 \\
5
\end{bmatrix}
\right)
$$ The total space spanned by the linear combination of these vectors is $\mathbb{R}^3$. Now, we use the Gram-Schmidt orthogonalization procedure to calculate the overall calculation (of which I will not do), we would see that what we are doing is just essentially aligning each vectors to another, with the first vector being the base of reference, the second one aligned orthogonally with the first, and the last one aligned orthogonally with both the first and second. This is always true since from Lemma 1, we see that orthogonal pairs do exists between vectors. 

Now, the last operation would be to take the normalization of those vectors $(e_{1}, e_{2},\dots e_{n})$, by using $$\vec{u}_{k} = \frac{\vec{e}_{k}}{||\vec{e}_{k}||}$$ per definition of the normal (or unit) vector of a vector. Hence we have the orthonormal system $(\vec{u}_{1}, \vec{u}_{2}, \dots , \vec{u}_{n})$ of which satisfy the conditions and, the Gram-Schmidt Procedure is complete. 

Finally, we would like to have a geometric representation of the procedure, for a little bit of intuition. 
![[Gram-Schmidt_orthonormalization_process.gif|center]]
___
# Reference
- https://math.libretexts.org/Bookshelves/Linear_Algebra/Book%3A_Linear_Algebra_(Schilling_Nachtergaele_and_Lankham)/09%3A_Inner_product_spaces/9.05%3A_The_Gram-Schmidt_Orthogonalization_procedure#
- https://math.libretexts.org/Bookshelves/Linear_Algebra/Book%3A_Linear_Algebra_(Schilling_Nachtergaele_and_Lankham)/05%3A_Span_and_Bases/5.01%3A_Linear_Span
- https://byjus.com/maths/gram-schmidt-orthonormalization-process/#:~:text=The%20Gram%2DSchmidt%20process%20is,space%20as%20the%20original%20set.
- https://people.tamu.edu/~yvorobets//MATH304-2011A/Lect3-05web.pdf
- https://en.wikipedia.org/wiki/Linear_span#:~:text=In%20mathematics%2C%20the%20linear%20span,independent%20vectors%20span%20a%20plane.
- https://en.wikipedia.org/wiki/Orthonormality
- https://en.wikipedia.org/wiki/Gram%E2%80%93Schmidt_process#:~:text=The%20Gram%E2%80%93Schmidt%20process%20also,...%2C%20un.
 