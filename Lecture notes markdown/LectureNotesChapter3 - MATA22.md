\title{
CHAPTER 3
}

\section{Distances and Angles}

\section{Scalar Product}

In this chapter we extend our vector geometry toolbox to be able to treat concepts like length, angles, distance and orthogonality in the three dimensional space. To this end we introduce a powerful tool in linear algebra, namely the scalar product, also called dot product or inner product. This is basically a rule that associates a number (scalar) to each pair of vectors in a very clever way.

We start by assuming a fixed length scale in the three dimensional space such that each vector $u$ has a determined length, denoted $\|u\|$. Angles between vectors are given in radians and by the angle between two vectors $u$ and $v$ we mean the angle between 0 and $\pi$ radians formed by $u$ and $v$ when set to emerge from a common point.

![](https://cdn.mathpix.com/cropped/2022_12_13_3d25a35f27ee0c7d36edg-01.jpg?height=300&width=480&top_left_y=1422&top_left_x=779)

We are now properly equipped to state the following definition:

Definition 1. Let $\mathbf{u}, \mathbf{v}$ be two vectors in space and let $\theta$ be the angle between them (in the interval $0 \leq \theta \leq \pi)$. Their scalar product is the number $(\mathbf{u} \mid \mathbf{v})$ defined by

$$
(\mathbf{u} \mid \mathbf{v})=\|\mathbf{u}\| \cdot\|\mathbf{v}\| \cdot \cos \theta .
$$

If $\mathbf{u}=\mathbf{0}$ or $\mathbf{v}=\mathbf{0}$, the angle $\theta$ is not defined, but in these cases we define $(\mathbf{u} \mid \mathbf{v})=0$.

The word "scalar" is a synonym for "number"; the term "scalar product" is used because the result $(\mathbf{u} \mid \mathbf{v})$ is a real number and not a vector. Now consider the case when $\mathbf{v}=\mathbf{e}$ is a unit vector, i.e., $\|\mathbf{e}\|=1$. If $\theta$ is the angle between $\mathbf{u}$ and $\mathbf{e}$, then

$$
(\mathbf{u} \mid \mathbf{e})=\|\mathbf{u}\| \cos \theta .
$$

![](https://cdn.mathpix.com/cropped/2022_12_13_3d25a35f27ee0c7d36edg-02.jpg?height=420&width=311&top_left_y=576&top_left_x=777)

We shall find an important geometric interpretation of this formula: Place $\mathbf{u}$ and e so that they emanate from the same point and let $\ell$ be a line through this point, with direction vector e. The orthogonal projection of $\mathbf{u}$ of $\ell$ (See Chapter 2, end of Section 2) can be written as

$$
\mathbf{u}^{\prime \prime}=(\|\mathbf{u}\| \cos \theta) \mathbf{e} .
$$

(This can be verified by an elementary trigonometrical argument - we ask the reader to work out the details.)

Comparing the formulae (1) and (2), we can write

$$
\mathbf{u}^{\prime \prime}=(\mathbf{u} \mid \mathbf{e}) \cdot \mathbf{e},
$$

and thus the number $(\mathbf{u} \mid \mathbf{e})$ is the coordinate of the orthogonal projection $\mathbf{u}^{\prime \prime}$ in the basis $\mathbf{e}$ for $\ell$.

If $\mathbf{v} \neq \mathbf{0}$ is not a unit vector, we write

$$
(\mathbf{u} \mid \mathbf{v})=\|\mathbf{v}\| \cdot(\mathbf{u} \mid \mathbf{e}),
$$

where $\mathbf{e}=\frac{1}{\|\mathbf{v}\|} \cdot \mathbf{v}$ is a unit vector. Thus, the absolute value $|(\mathbf{u} \mid \mathbf{v})|$ is equal to the length of $\mathbf{v}$ times the length of the orthogonal projection of $\mathbf{u}$ on a line with direction vector $\mathbf{v}$.

Note that the sign of $(\mathbf{u} \mid \mathbf{v})$ is positive if the angle between $\mathbf{u}$ and $\mathbf{v}$ is acute, and negative if it is obtuse. 

\section{Properties of the scalar product.}

The scalar product satisfies the following rules. ( $\mathbf{u}, \mathbf{v}, \mathbf{w}$ denote arbitrary vectors.)

(I) $(\mathbf{u} \mid \mathbf{v})=(\mathbf{v} \mid \mathbf{u})$

(II) $(\mathbf{u}+\mathbf{v} \mid \mathbf{w})=(\mathbf{u} \mid \mathbf{w})+(\mathbf{v} \mid \mathbf{w})$

(III) $(t \mathbf{u} \mid \mathbf{v})=t(\mathbf{u} \mid \mathbf{v}), \quad t \in \mathbb{R}$

(IV) $(\mathbf{u} \mid \mathbf{u}) \geq 0$ with $(\mathbf{u} \mid \mathbf{u})=0$ if and only if $\mathbf{u}=\mathbf{0}$

(V) $\|\mathbf{u}\|=\sqrt{(\mathbf{u} \mid \mathbf{u})}$

The rule (I) is called symmetry of the scalar product; (II) and (III) together are called linearity in the first argument; (IV) is called positive definiteness.

The properties (I),,(III), (IV) and (V) are immediate; (II) can be seen in the following way: If $\mathbf{w}=\mathbf{e}$ is a unit vector, then, by the geometrical interpretation of the scalar product, we can see that (II) means precisely that

$$
(\mathbf{u}+\mathbf{v})^{\prime \prime}=\mathbf{u}^{\prime \prime}+\mathbf{v}^{\prime \prime} .
$$

That this is the case was shown at the end of Chap. 2, Sect. 2. This proves that (II) holds when $\mathbf{w}$ is a unit vector. For general w, we now get (II) by applying the unit vector case to the vector $\mathbf{e}$ in the formula $(\mathbf{u} \mid \mathbf{w})=\|\mathbf{w}\| \cdot(\mathbf{u} \mid \mathbf{e})$.

REMARK 2. Note that linearity in the second argument follows from the symmetry and the linearity in the first argument. In particular, we have $(\mathbf{u} \mid t \mathbf{v})=t(\mathbf{u} \mid \mathbf{v})$.

As an application of the scalar product, we prove a well-known theorem. We say that two vectors $\mathbf{u}, \mathbf{v}$ are orthogonal to each other if $(\mathbf{u} \mid \mathbf{v})=0$. (This means that the angle $\theta=\pi / 2$, or that one of $\mathbf{u}$ or $\mathbf{v}$ is the zero vector.)

THEOREM 3. (Pythagoras' Theorem) If $\mathbf{u}$ and $\mathbf{v}$ are orthogonal, then

$$
\|\mathbf{u}+\mathbf{v}\|^{2}=\|\mathbf{u}\|^{2}+\|\mathbf{v}\|^{2} .
$$

![](https://cdn.mathpix.com/cropped/2022_12_13_3d25a35f27ee0c7d36edg-03.jpg?height=209&width=353&top_left_y=1972&top_left_x=840)

PROOF. If $\mathbf{u}, \mathbf{v}$ are any vectors (orthogonal or not), then by the computational rules above

$$
\begin{aligned}
\|\mathbf{u}+\mathbf{v}\|^{2} & =(\mathbf{u}+\mathbf{v} \mid \mathbf{u}+\mathbf{v}) \\
& =(\mathbf{u} \mid \mathbf{u})+(\mathbf{u} \mid \mathbf{v})+(\mathbf{v} \mid \mathbf{u})+(\mathbf{v} \mid \mathbf{v}) \\
& =\|\mathbf{u}\|^{2}+2(\mathbf{u} \mid \mathbf{v})+\|\mathbf{v}\|^{2}
\end{aligned}
$$

Hence if $(\mathbf{u} \mid \mathbf{v})=0$, then

$$
\|\mathbf{u}+\mathbf{v}\|^{2}=\|\mathbf{u}\|^{2}+\|\mathbf{v}\|^{2}
$$

The scalar product can often be used to give easier proofs to well-known theorems from Euclidean geometry that involve orthogonality, angles and distance relationships. The following statement is one such example.

Example 1. An angle inscribed in a semicircle is a right angle.

In order to prove this let us introduce some notations. Let $\mathcal{C}$ be a circle with centre $M$ and radius $r$, and $P, Q$ and $R$ be three different points on the circle such that $\overrightarrow{P R}$ is a diameter.

![](https://cdn.mathpix.com/cropped/2022_12_13_3d25a35f27ee0c7d36edg-04.jpg?height=350&width=396&top_left_y=1348&top_left_x=824)

We prove that the inscribed angle $\angle P Q R$ is a right angle by showing that the scalar product $(\overrightarrow{Q P} \mid \overrightarrow{Q R})$ is equal to zero.

We have that $\overrightarrow{Q P}=\overrightarrow{Q M}+\overrightarrow{M P}$ and $\overrightarrow{Q R}=\overrightarrow{Q M}+\overrightarrow{M R}$ which gives

$$
\begin{aligned}
(\overrightarrow{Q P} \mid \overrightarrow{Q R}) & =((\overrightarrow{Q M}+\overrightarrow{M P}) \mid(\overrightarrow{Q M}+\overrightarrow{M R}))= \\
& =(\overrightarrow{Q M} \mid \overrightarrow{Q M})+(\overrightarrow{Q M} \mid \overrightarrow{M R})+(\overrightarrow{M P} \mid \overrightarrow{Q M})+(\overrightarrow{M P} \mid \overrightarrow{M R})
\end{aligned}
$$

Since $\|\overrightarrow{P R}\|=2 r$ and the centre $M$ is the midpoint of the segment $\overrightarrow{P R}$ we have that $\overrightarrow{P M}=\overrightarrow{M R}$ and hence, $\overrightarrow{M P}=-\overrightarrow{M R}$. This yields

$(\overrightarrow{M P} \mid \overrightarrow{Q M})=(-\overrightarrow{M R} \mid \overrightarrow{Q M})=-(\overrightarrow{Q M} \mid \overrightarrow{M R}) \quad$ and $\quad(\overrightarrow{M P} \mid \overrightarrow{M R})=-(\overrightarrow{M R} \mid \overrightarrow{M R})$ The equality (3) can also be written as:

$$
\begin{aligned}
(\overrightarrow{Q P} \mid \overrightarrow{Q R}) & =(\overrightarrow{Q M} \mid \overrightarrow{Q M})+(\overrightarrow{Q M} \mid \overrightarrow{M R})-(\overrightarrow{Q M} \mid \overrightarrow{M R})-(\overrightarrow{M R} \mid \overrightarrow{M R}) \\
& =\|\overrightarrow{Q M}\|^{2}-\|\overrightarrow{M R}\|^{2}=r^{2}-r^{2}=0
\end{aligned}
$$

which concludes the proof.

\section{Exercises.}

1. Let $\theta$ be the angle between the sides $A B$ and $B C$ in a triangle $A B C$. Prove the law of cosines:

$$
\|\overrightarrow{A C}\|^{2}=\|\overrightarrow{A B}\|^{2}+\|\overrightarrow{B C}\|^{2}-2\|\overrightarrow{A B}\|\|\overrightarrow{B C}\| \cos \theta .
$$

(Observe that this reduces to Pythagoras' Theorem when $\theta=\pi / 2$.)

2. Let $u$ and $v$ be two non-zero vectors such that $\|u+v\|=\|u-v\|$. Show that the angle $\theta$ between the two vectors $u$ and $v$ is right.

3. Let $u$ and $v$ be two non-zero vectors such that $u+3 v$ is orthogonal to $2 u-v$ and $u+7 v$ is orthogonal to $2 u+v$. Determine the angle $\theta$ between the vectors $u$ and $v$.

4. Denote by $a$ and $b$ the side-lengths in a parallelogram, and by $c$ and $d$ the lengths of the diagonals. Prove the parallelogram law:

$$
c^{2}+d^{2}=2\left(a^{2}+b^{2}\right) .
$$



\section{Scalar Product and Orthonormal Bases}

\section{Orthonormal basis for a plane.}

Let $M$ be a plane and $\mathbf{e}_{1}, \mathbf{e}_{2}$ a basis for $M$. If

$$
\mathbf{u}=x_{1} \mathbf{e}_{1}+x_{2} \mathbf{e}_{2} \quad \text { and } \quad \mathbf{v}=y_{1} \mathbf{e}_{1}+y_{2} \mathbf{e}_{2}
$$

are two vectors in $M$, then by the rules (I)-(III) for the scalar product,

$$
(\mathbf{u} \mid \mathbf{v})=x_{1} y_{1}\left(\mathbf{e}_{1} \mid \mathbf{e}_{1}\right)+\left(x_{1} y_{2}+x_{2} y_{1}\right)\left(\mathbf{e}_{1} \mid \mathbf{e}_{2}\right)+x_{2} y_{2}\left(\mathbf{e}_{2} \mid \mathbf{e}_{2}\right)
$$

If the basis vectors $\mathbf{e}_{1}, \mathbf{e}_{2}$ are orthogonal and have length 1 , then the expression $(\mathbf{u} \mid \mathbf{v})$ becomes particularly simple. In this case $\left(\mathbf{e}_{1} \mid \mathbf{e}_{1}\right)=\left(\mathbf{e}_{2} \mid \mathbf{e}_{2}\right)=1$ and $\left(\mathbf{e}_{1} \mid \mathbf{e}_{2}\right)=0$, and thus

![](https://cdn.mathpix.com/cropped/2022_12_13_3d25a35f27ee0c7d36edg-06.jpg?height=520&width=464&top_left_y=922&top_left_x=798)

A basis for a plane consisting of two orthogonal unit vectors is called an orthonormal basis (in short: $O N$-basis) for the plane.

\section{Orthonormal basis for the three dimensional space.}

The corresponding definition in three dimensions is the following. We say that three vectors $\mathbf{e}_{1}, \mathbf{e}_{2}, \mathbf{e}_{3}$ are pairwise orthogonal if

$$
\left(\mathbf{e}_{j} \mid \mathbf{e}_{k}\right)=0, \quad \text { when } j \neq k .
$$

Three vectors $\mathbf{e}_{1}, \mathbf{e}_{2}, \mathbf{e}_{3}$ are said to form an orthonormal basis for three-dimensional space if (i) they have unit length, and (ii) they are pairwise orthogonal. We can sumarise the definition of orthonormal basis by the equation

$$
\left(\mathbf{e}_{j} \mid \mathbf{e}_{k}\right)=\left\{\begin{array}{lll}
0 & \text { if } & j \neq k \\
1 & \text { if } & j=k
\end{array} .\right.
$$

If $\mathbf{e}_{1}, \mathbf{e}_{2}, \mathbf{e}_{3}$ form an orthonormal basis and

$$
\mathbf{u}=x_{1} \mathbf{e}_{1}+x_{2} \mathbf{e}_{2}+x_{3} \mathbf{e}_{3} \quad \text { and } \quad \mathbf{v}=y_{1} \mathbf{e}_{1}+y_{2} \mathbf{e}_{2}+y_{3} \mathbf{e}_{3}
$$

then

$$
(\mathbf{u} \mid \mathbf{v})=x_{1} y_{1}+x_{2} y_{2}+x_{3} y_{3} .
$$

When $\mathbf{u}=\mathbf{v}$ this reduces to

$$
\|\mathbf{u}\|^{2}=x_{1}^{2}+x_{2}^{2}+x_{3}^{2} .
$$

This can be regarded as the three-dimensional version of the theorem of Pythagoras.

![](https://cdn.mathpix.com/cropped/2022_12_13_3d25a35f27ee0c7d36edg-07.jpg?height=420&width=523&top_left_y=663&top_left_x=758)

(u is here the sum of three pairwise orthogonal vectors $x_{1} \mathbf{e}_{1}, x_{2} \mathbf{e}_{2}, x_{3} \mathbf{e}_{3}$.)

Example 1. Suppose that $\mathbf{u}$ and $\mathbf{v}$ have coordinates

$$
\mathbf{u}=(4,1,1) \text { and } \mathbf{v}=(2,2,-1)
$$

with respect to some orthonormal basis. We shall determine the angle $\theta$ between $\mathbf{u}$ and $\mathbf{v}$. For this purpose we use (5) and (6) to compute

$$
\begin{aligned}
(\mathbf{u} \mid \mathbf{v}) & =4 \cdot 2+1 \cdot 2+1 \cdot(-1)=9 \\
\|\mathbf{u}\| & =\sqrt{16+1+1}=3 \sqrt{2} \\
\|\mathbf{v}\| & =\sqrt{4+4+1}=3 .
\end{aligned}
$$

Since $(\mathbf{u} \mid \mathbf{v})=\|\mathbf{u}\|\|\mathbf{v}\| \cos \theta$, this gives

$$
\cos \theta=\frac{(\mathbf{u} \mid \mathbf{v})}{\|\mathbf{u}\| \mathbf{v} \|}=\frac{9}{3 \sqrt{2} \cdot 3}=\frac{1}{\sqrt{2}} .
$$

This means that $\theta=\pi / 4$.

Example 2. The formula (4) can be used to prove many trigonometrical identities. (As we know, the de Moivre formula for multiplication of complex numbers provides another way to do this.)

As an example, we shall now show the following version of the addition formula for cosines:

$$
\cos (\alpha-\beta)=\cos \alpha \cos \beta+\sin \alpha \sin \beta .
$$

To this end, let $\mathbf{e}_{1}, \mathbf{e}_{2}$ be an orthonormal basis for the plane and put

$$
\mathbf{u}=(\cos \alpha) \mathbf{e}_{1}+(\sin \alpha) \mathbf{e}_{2} \quad, \quad \mathbf{v}=(\cos \beta) \mathbf{e}_{1}+(\sin \beta) \mathbf{e}_{2} .
$$

Since $\mathbf{u}$ and $\mathbf{v}$ then have length 1 , while the angle between them is $|\alpha-\beta|$, the definition of scalar product shows that

$$
(\mathbf{u} \mid \mathbf{v})=\cos (\alpha-\beta) .
$$

(We have here used the fact that $\cos$ is even: $\cos (\alpha-\beta)=\cos (\beta-\alpha)$.)

On the other hand, by (4), we have

$$
(\mathbf{u} \mid \mathbf{v})=\cos \alpha \cos \beta+\sin \alpha \sin \beta .
$$

Comparing the two expressions for $(\mathbf{u} \mid \mathbf{v})$, we infer that the formula (7) holds.

\section{Exercises.}

5. A triangle in space has vertices at the points $(1,0,2),(0,-1,1)$, and $(2,1,2)$ according to some orthonormal basis. Compute all side-lengths and cosines of angles in the triangle.

6. Consider the vectors $v_{1}=(1,3, a), v_{2}=(1,1,-a)$ and $v_{3}=(b,-a, 1)$ with respect to some orthonormal basis. Determine all real numbers $a, b$ such that the vectors are mutually orthogonal.

7. Let $\mathbf{e}_{1}, \mathbf{e}_{2}, \mathbf{e}_{3}$ be an orthonormal basis in space. Suppose that the vector $\mathbf{u}$ makes the angle $\pi / 4$ to the vector $\mathbf{e}_{1}$ and the angle $\pi / 3$ to the vector $\mathbf{e}_{2}$. What are the possible angles between $\mathbf{u}$ and $\mathbf{e}_{3}$ ? 

\section{Computing Distances and Angles}

A coordinate system $O \mathbf{e}_{1} \mathbf{e}_{2} \mathbf{e}_{3}$ where $\mathbf{e}_{1}, \mathbf{e}_{2}, \mathbf{e}_{3}$ is an orthonormal basis is called an orthonormal system or an $O N$-system. In this section we fix an ON-system and assume that all points are represented in that system.

![](https://cdn.mathpix.com/cropped/2022_12_13_3d25a35f27ee0c7d36edg-09.jpg?height=428&width=528&top_left_y=556&top_left_x=755)

The distance between two points $P=(x, y, z)$ and $Q=\left(x_{0}, y_{0}, z_{0}\right)$ is then given by

$$
\|\overrightarrow{P Q}\|=\sqrt{\left(x-x_{0}\right)^{2}+\left(y-y_{0}\right)^{2}+\left(z-z_{0}\right)^{2}} .
$$

\section{Distance between a point and a line}

Consider a line $\ell$ and a point $P$ which is not on the line. By the distance between $P$ and $\ell$ we mean the shortest possible distance between $P$ to a point $R \in \ell$. A geometric consideration shows that the closest point $R$ is determined by the condition that $\overrightarrow{P R}$ is orthogonal to the direction vector of $\ell$.

![](https://cdn.mathpix.com/cropped/2022_12_13_3d25a35f27ee0c7d36edg-09.jpg?height=391&width=534&top_left_y=1496&top_left_x=755)

Example 1. Let $\ell$ be the line through the points $Q=(-2,1,1)$ and $S=(0,-1,2)$, and let $P=(1,2,1)$. We shall compute the distance from $P$ to $\ell$.

First note that $\ell$ has direction vector $\overrightarrow{Q S}=(2,-2,1)$, so it has the parametric representation

$$
\ell:\left\{\begin{array}{l}
x=-2+2 t \\
y=1-2 t \\
z=1+t
\end{array}\right.
$$

We now seek the closest point $R \in \ell$ to $P$. To this end let $R=(-2+2 t, 1-2 t, 1+t)$ and we must determine $t$ so that $\overrightarrow{P R}$ is orthogonal to the direction vector $(2,-2,1)$ of $\ell$. That is, we shall have

$$
0=(\overrightarrow{P R} \mid \overrightarrow{Q S})=(-3+2 t) \cdot 2+(-1-2 t) \cdot(-2)+t \cdot 1=9 t-4 .
$$

This gives $t=4 / 9$ and $\overrightarrow{P R}=\frac{1}{9}(-19,-17,4)$. The distance from $P$ to $\ell$ is thus

$$
\|\overrightarrow{P R}\|=\frac{1}{9} \sqrt{19^{2}+17^{2}+4^{2}}=\frac{\sqrt{74}}{3} .
$$

\section{Distance from a point to a plane}

Let $\pi$ be a plane in space, $Q$ a point in $\pi$, and $\mathbf{n}$ a unit normal vector to $\pi$. (This means that $\mathbf{n}$ has unit length and points in a direction orthogonal to $\pi$.) The distance $d$ between a point $P$ and $\pi$ is again defined as the smallest distance

![](https://cdn.mathpix.com/cropped/2022_12_13_3d25a35f27ee0c7d36edg-10.jpg?height=420&width=507&top_left_y=1064&top_left_x=771)

between $P$ to some point in $\pi$. We assert that

$$
d=|(\mathbf{n} \mid \overrightarrow{Q P})| .
$$

To prove this, it suffices to note that the orthogonal projection of the vector $\overrightarrow{Q P}$ on $\mathbf{n}$ is equal to $(\mathbf{n} \mid \overrightarrow{Q P}) \cdot \mathbf{n}$. The length of the latter vector must thus equal to the sought distance, which proves (8).

Now suppose that $Q=\left(x_{0}, x_{y}, z_{0}\right), P=(x, y, z)$, and $\mathbf{n}=(A, B, C)$. Then

$$
(\mathbf{n} \mid \overrightarrow{Q P})=A\left(x-x_{0}\right)+B\left(y-y_{0}\right)+C\left(z-z_{0}\right) \text {. }
$$

If we put

$$
D=A x_{0}+B y_{0}+C z_{0},
$$

then (8) can be written

$$
d=|A x+B y+C z-D| .
$$

But $P$ belongs to $\pi$ precisely when $d=0$, i.e., when

$$
A x+B y+C z=D .
$$

We have shown that an arbitrary plane can be described by a linear equation of the type (10). If $P=(x, y, z)$ is not in $\pi$, then its distance to $\pi$ is given by (9).

REMARK 4. The argument above shows that if we have a plane of the form (10), then $\mathbf{n}=(A, B, C)$ is a normal vector. Above we assumed that $\mathbf{n}$ is a unit vector, i.e., that

$$
A^{2}+B^{2}+C^{2}=1 .
$$

If this is not satisfied, one must first normalise the equation (10) by dividing with $\sqrt{A^{2}+B^{2}+C^{2}}$. The distance formula then becomes

$$
d=\frac{|A x+B y+C z-D|}{\sqrt{A^{2}+B^{2}+C^{2}}} .
$$

Example 2. We shall determine an equation for the plane $\pi$ which passes through the point $(1,-1,2)$ and has the normal

$$
\ell:\left\{\begin{array}{l}
x=1+3 t \\
y=3+2 t \\
z=2-t
\end{array} .\right.
$$

The direction vector of $\ell$, i.e. the vector $(3,2,-1)$ must then be a normal vector of $\pi$. Since the point $(1,-1,2)$ belongs to $\pi$, the equation of the plane becomes

$$
3(x-1)+2(y-(-1))+(-1)(z-2)=0,
$$

i.e.,

$$
3 x+2 y-z=-1 .
$$

The distance from the point $P=(5,6,7)$ to $\pi$ is thus (see (11))

$$
\frac{|3 \cdot 5+2 \cdot 6-1 \cdot 7+1|}{\sqrt{3^{2}+2^{2}+1^{2}}}=\frac{21}{\sqrt{14}} \text {. }
$$



\section{Distance between two lines}

Given two lines which do not intersect, we define the distance between them to be the smallest possible distance between one point on the first line and one on the second one. The following example comprises a method to compute such a distance.

Example 3. Consider the lines $\ell_{1}$ and $\ell_{2}$ having parametric representations

$$
\ell_{1}:\left\{\begin{array}{l}
x=-3+2 t \\
y=\quad t \\
z=1-t
\end{array} \quad ; \quad \ell_{2}:\left\{\begin{array}{l}
x=3+t \\
y=4+3 t \\
z=2+2 t
\end{array}\right.\right.
$$

We shall compute the (shortest) distance between $\ell_{1}$ and $\ell_{2}$. Direction vectors for the two lines are $(2,1,-1)$ and $(1,3,2)$. Let $\pi$ be the plane parallel to these directions, which passes through the point $(-3,0,1)$ on $\ell_{1}$. Then $\ell_{1} \subset \pi$ and also, $\pi$ is parallel to $\ell_{2}$. Hence the distance $d$ between $\ell_{1}$ and $\ell_{2}$ must equal to the distance from an arbitrary point on $\ell_{2}$ to $\pi$. A parametric representation of $\pi$ is

![](https://cdn.mathpix.com/cropped/2022_12_13_3d25a35f27ee0c7d36edg-12.jpg?height=211&width=506&top_left_y=1133&top_left_x=777)

Elimination of $s$ and $t$ gives the equation

$$
x-y+z=-2
$$

for the plane $\pi$. The distance from the point $(3,4,2)$ on $\ell_{2}$ to $\pi$ is, according to $(11)$

$$
d=\frac{|3-4+2+2|}{\sqrt{1+1+1}}=\frac{3}{\sqrt{3}}=\sqrt{3}
$$

The distance between the lines is thus $\sqrt{3}$.

\section{Angle between two planes}

If $\pi_{1}, \pi_{2}$ are two planes, we define the angle between them to be the angle between the corresponding normal vectors. (In general there are two possibilities for the angle, depending on the mutual orientations of the normal vectors: see the example below.)

Example 4. Suppose that

$$
\pi_{1}: x-2 y-2 z=-3 \quad \pi_{2}: x+4 y+z=5 .
$$

Corresponding normal vectors are $\mathbf{n}_{1}=(1,-2,-2)$ and $\mathbf{n}_{2}=(1,4,1)$. The angle $\theta$ between the planes then satisfies

$$
\cos \theta=\frac{\left(\mathbf{n}_{1} \mid \mathbf{n}_{2}\right)}{\left\|\mathbf{n}_{1}\right\|\left\|\mathbf{n}_{2}\right\|}=\frac{1 \cdot 1+(-2) \cdot 4+(-2) \cdot 1}{\sqrt{1^{2}+2^{2}+2^{2}} \cdot \sqrt{1^{2}+4^{2}+1^{2}}}=-\frac{1}{\sqrt{2}} .
$$

This gives $\theta=3 \pi / 4$. This is the obtuse angle between the planes. There is also another possibility, namely if we substitute $-\mathbf{n}_{1}$ for $\mathbf{n}_{1}$ above. This leads to the acute angle $\pi-\theta=\pi / 4$.

\section{Angle between a line and a plane}

To determine the angle between a line $\ell$ and a plane $\pi$, one first computes the acute angle $\psi$ between $\ell$ and a normal vector to $\pi$. The angle $\varphi$ between $\ell$ and $\pi$ is defined by $\varphi+\psi=\pi / 2$.

![](https://cdn.mathpix.com/cropped/2022_12_13_3d25a35f27ee0c7d36edg-13.jpg?height=334&width=545&top_left_y=1042&top_left_x=752)

Example 5. Suppose that

$$
\ell:\left\{\begin{array}{l}
x=2+t \\
y=3+t \\
z=1+4 t
\end{array} \quad ; \quad \pi: 4 x-11 y-5 z=-2 .\right.
$$

Let $\theta$ denote the angle between the direction vector $(1,1,4)$ of $\ell$ and the normal vector $(4,-11,-5)$ of $\pi$. Then

$$
\cos \theta=\frac{1 \cdot 4+1 \cdot(-11)+4 \cdot(-5)}{\sqrt{1^{2}+1^{2}+4^{2}} \cdot \sqrt{4^{2}+11^{2}+5^{2}}}=-\frac{1}{2} .
$$

This gives $\theta=2 \pi / 3$, which is obtuse. Hence the acute angle between $\ell$ and the normal to $\pi$ is $\psi=\pi-\theta=\pi / 3$. The angle between $\ell$ and $\pi$ is thus

$$
\varphi=\pi / 2-\psi=\pi / 6 \text {. }
$$



\section{Exercises.}

8. Compute the distance between the point $(1,2,3)$ and the line

$$
\left\{\begin{array}{l}
x=1-t \\
y=-4+2 t \\
z=3-t
\end{array}\right.
$$

9. The line $\ell$ is the intersection between the planes $x+2 y-2 z=5$ and $2 x-y+z=0$. Determine the point on $\ell$ which is closest to the origin.

10. The line $\ell$ passes through the point $(1,2,3)$ and is perpendicular to the plane $2 x-3 y+z=-3$. Find the distance between $\ell$ and the point $(4,5,6)$.

11. Determine, in the form $A x+B y+C z=D$, the equation of the plane which consists of all points which have equal distance to the points $(1,2,0)$ and $(-1,0,2)$.

12. Find the distance from the plane $3 x-4 y+12 z=13$ to the points $(0,0,0)$ and $(2,1,3)$. Are these points on the same or on opposite sides of the plane?

13. a) Determine, in the form $A x+B y+C z=D$, an equation for the plane $M$ which passes through the points $(2,-3,0)$ and $(2,-2,2)$, and is parallel to the line $x=2-t, y=1+t, z=2-t$.

b) Find the distance between the point $(3,-1,0)$ and $M$.

14. Find the point closest to the point $(-2,-2,-1)$ in the plane passing through the points $(1,3,-1),(1,1,0),(-1,3,2)$.

15. a) Prove that the lines

$$
\ell_{1}:\left\{\begin{array}{l}
x=1+t \\
y=2-t \\
z=3+2 t
\end{array} \quad \text { and } \quad \ell_{2}:\left\{\begin{array}{l}
x=3+t \\
y=2+t \\
z=2-3 t
\end{array}\right.\right.
$$

intersect at a point.

b) Find the distance between the point $(3,4,5)$ and the plane spanned by $\ell_{1}$ and $\ell_{2}$. 16. A ray of light is emitted from the point $(3,-2,-1)$ and reflected off the plane $x-2 y-2 z=0$. The reflected ray passes the point $(4,-1,-6)$. At which point does the ray hit the plane?

17. Determine the distance between the lines

a) $(x, y, z)=t(-3,3,1)$ and $(x, y, z)=(-1,0,0)+t(1,1,1)$.

b) $(x, y, z)=(1,2,3)+t(0,1,1)$ and $(x, y, z)=(1,1,1)+t(2,3,1)$.

18. Consider the lines

$$
\ell_{1}:\left\{\begin{array}{l}
x=8-3 t \\
y=2-t \\
z=-3+t
\end{array} \quad \text { and } \quad \ell_{2}:\left\{\begin{array}{l}
x=-12-t \\
y=4-2 t \\
z=1+t
\end{array} .\right.\right.
$$

Determine, in the form $A x+B y+C z=D$, an equation for the plane which is parallel to $\ell_{1}$ and $\ell_{2}$ and has the same distance to the two lines.

19. a) Determine, in the form $A x+B y+C z=D$, an equation for the plane $M$ which passes through the points $(2,-1,3),(1,2,-2)$, and $(1,0,2)$.

b) Determine the angle between $M$ and the plane $2 x+y-z=-1$.

20. Determine the angle between the plane $x+2 y-z=0$ and the line $(x, y, z)=$ $(3,5,-1)+t(1,1,0)$

21. A tetrahedron has corners $A=(-1,2,0), B=(1,3,-1), C(1,1,0)$, and $D(-1,3,-2)$. Determine the angle between the plane containing the side $B C D$ and the line containing the edge $A B$.

\section{Answers to Exercises}

3. $\theta=2 \pi / 3$

5. The side-lengths are $3, \sqrt{3}$, and $\sqrt{2}$. The cosines of angles are $-\sqrt{2 / 3}$, $5 /(3 \sqrt{3})$, and $2 \sqrt{2} / 3$.

6. $a=\pm 2, b=\pm 4$

7. $\pi / 3$ or $2 \pi / 3$.

8. $\sqrt{12}$.

9. $(1,1,-1)$.

10. $3 \sqrt{3}$.

11. $x+y-z=0$.

12. 1 and $25 / 13$ respectively. The points are on opposite sides of the plane.

13. a) $3 x-2 y+z=12$. b) $1 / \sqrt{14}$.

14. $(1,-1,1)$. 15. a) Intersection-point: $(2,1,5)$. b) $16 / \sqrt{30}$.

16. $(2,1,0)$.

17. a) $1 / \sqrt{14}$. b) $1 / \sqrt{3}$

18. $x+2 y+5 z=-1$.

19. a) $x+2 y+z=3$. b) $\pi / 3$.

20. $\pi / 3$.

21. $\pi / 6$.