\title{
CHAPTER 2
}

\section{Vectors}

\section{Basic Definitions}

This chapter together with the following two chapters are devoted to analytic geometry, also known as coordinate geometry, that is the study of geometry using systems of coordinates. By introducing a so called basis and coordinate system in the three dimensional space, one can represent a point using a triple of real numbers. Geometrical objects such as lines, planes, curves, etc. as well as geometrical relations in space can then be represented by means of algebraic equations and viceversa. In what follows we assume that the reader has a well-developed intuition about (the properties of) basic geometric objects such as points, lines and planes. We begin by introducing the concept of a vector.

\section{Vectors and Directed Line Segments.}

In order to define a vector we first need to introduce directed line segments. If $P$ and $Q$ are two points in space, we denote by $\overrightarrow{P Q}$ the directed line segment which starts at $P$ and ends at $Q$. A directed segment is determined by its starting point $P$, its direction, and its magnitude (or length).

Two directed segments $\overrightarrow{P Q}$ and $\overrightarrow{R S}$ are called equivalent (notation: $\overrightarrow{P Q} \sim \overrightarrow{R S}$ ) if they have the same direction and magnitude. This defines a so called equivalence relation on the set of directed line segments in space.

![](https://cdn.mathpix.com/cropped/2022_12_13_cabdc435b88729520c88g-01.jpg?height=323&width=436&top_left_y=1893&top_left_x=801)

Figure $1 . \mathrm{PQ}$ and RS equivalent directed segments The vector $\mathbf{u}$ which contains $\overrightarrow{P Q}$ is the set of all directed line segments in space that are equivalent to $\overrightarrow{P Q}$ (i.e. it is the equivalence class containing $\overrightarrow{P Q}$ ). In symbols:

$$
\mathbf{u}=\{\overrightarrow{R S}: \overrightarrow{R S} \sim \overrightarrow{P Q}\} .
$$

In this situation we say that the line segment $\overrightarrow{P Q}$ represents the vector $\mathbf{u}$.

The direction and the magnitude of the vector $\mathbf{u}$ is defined as the direction and magnitude of some representative $\overrightarrow{P Q}$. We will denote the length (or norm) of u by the symbol $\|\mathbf{u}\|$.

In practice, one often briefly writes $\mathbf{u}=\overrightarrow{P Q}$ instead of the using the bulky (but more precise) notation in (1). We will often, without further mention, use this convention in the following.

The zero vector is the vector $\mathbf{0}=\overrightarrow{P P}$; clearly $\|\mathbf{0}\|=0$. A vector $\mathbf{u}$ with $\|\mathbf{u}\|=1$ is called a unit vector.

\section{Vector Addition.}

The sum $\mathbf{u}+\mathbf{v}$ of two vectors is defined as follows. We choose a directed segment $\overrightarrow{P Q}$ representing $\mathbf{u}$, then a representative $\overrightarrow{Q R}$, with the same $Q$, of $\mathbf{v}$. Then the sum $\mathbf{u}+\mathbf{v}$ is given by the vector

$$
\mathbf{u}+\mathbf{v}=\overrightarrow{P R} .
$$

This definition is sometimes called the triangle rule for vector addition and it is obvious that it is independent of the start point $P$, i.e. of the choice of representative directed segments.

![](https://cdn.mathpix.com/cropped/2022_12_13_cabdc435b88729520c88g-02.jpg?height=320&width=436&top_left_y=1607&top_left_x=801)

Figure 2. The sum $u+v$

The above definition can be expressed in an alternative, equivalent way. Suppose that the vectors $\mathbf{u}$ and $\mathbf{v}$ are not parallel, set them to emerge from a common start point, $P$ say, and consider the parallelogram spanned by the two vectors. Then the sum $\mathbf{u}+\mathbf{v}$ is the vector associated to the directed diagonal with start point $P$. This definition is sometimes called the parallelogram law of addition. The addition of vectors satisfies the following (easily verified) rules:

(i) $\mathbf{u}+\mathbf{v}=\mathbf{v}+\mathbf{u}$ ("commutativity")

(ii) $\mathbf{u}+(\mathbf{v}+\mathbf{w})=(\mathbf{u}+\mathbf{v})+\mathbf{w}$ ("associativity")

(iii) If $\mathbf{u}+\mathbf{v}=\mathbf{u}+\mathbf{w}$ then $\mathbf{v}=\mathbf{w}$ ("the cancellation law")

(iv) $\mathbf{u}+\mathbf{0}=\mathbf{u}$ ("neutral element").

\section{Subtraction.}

If $\mathbf{u}=\overrightarrow{P Q}$ is a vector, we denote by $-\mathbf{u}$ the vector with the same magnitude but opposite direction, i.e., $-\mathbf{u}=\overrightarrow{Q P}$. It is clear that $\mathbf{u}+(-\mathbf{u})=\mathbf{0}$ for all $\mathbf{u}$. We define the difference between $\mathbf{u}$ and $\mathbf{v}$ by

$$
\mathbf{u}-\mathbf{v}=\mathbf{u}+(-\mathbf{v}) .
$$

\section{Multiplication by Scalars.}

Another basic but important operation that one can perform with vectors is multiplication by scalars. (Scalar is a synonym for "real number"). This operation models the change of length and/or reversing of direction of a vector.

Let $s \in \mathbb{R}$ and let $\mathbf{u}$ be a vector. Then the product $s \mathbf{u}$ is defined in the following way:

(1) If $s>0$ we define $s \mathbf{u}$ to be the vector with the same direction as $\mathbf{u}$ and magnitude $s\|\mathbf{u}\|$. (So $s \mathbf{u}$ is a "rescaled" version of $\mathbf{u}$.)

(2) If $s=0$ we define $s \mathbf{u}=\mathbf{0}$.

(3) If $s<0$ we define $s \mathbf{u}$ to be the vector with the direction opposite to $\mathbf{u}$ and length $|s| \mid \mathbf{u} \|$.

Note that if $\mathbf{u} \neq \mathbf{0}$, then the vector $\frac{1}{\|\mathbf{u}\|} \cdot \mathbf{u}$ is the unit vector with the same direction as $\mathbf{u}$.

The multiplication with scalars satisfies the following rules:

(a) $s(t \mathbf{u})=(s t) \mathbf{u}$,

(b) $(s+t) \mathbf{u}=s \mathbf{u}+t \mathbf{u}$,

(c) $s(\mathbf{u}+\mathbf{v})=s \mathbf{u}+s \mathbf{v}$.

(d) $0 \mathbf{u}=\mathbf{0}, 1 \mathbf{u}=\mathbf{u}, s \mathbf{0}=\mathbf{0}$.

Two non-zero vectors $\mathbf{u}, \mathbf{v}$ are called parallel if one of them can be written as a scalar multiple of the other one. We write $\mathbf{u} \| \mathbf{v}$ to denote that $\mathbf{u}$ and $\mathbf{v}$ are parallel. Example 1. Let $O, P, Q$ be three points in space and let $\mathbf{u}=\overrightarrow{O P}$ and $\mathbf{v}=\overrightarrow{O Q}$. Let $M$ be the mid-point of the segment $P Q$. We claim that

$$
\overrightarrow{O M}=\frac{1}{2}(\mathbf{u}+\mathbf{v}) .
$$

![](https://cdn.mathpix.com/cropped/2022_12_13_cabdc435b88729520c88g-04.jpg?height=323&width=442&top_left_y=608&top_left_x=798)

FIGURE 3

To prove this, observe that

$$
\overrightarrow{O P}+\overrightarrow{P Q}=\overrightarrow{O Q}
$$

i.e.,

$$
\overrightarrow{P Q}=\overrightarrow{O Q}-\overrightarrow{O P}=\mathbf{v}-\mathbf{u}
$$

This gives that

$$
\overrightarrow{O M}=\overrightarrow{O P}+\frac{1}{2} \overrightarrow{P Q}=\mathbf{u}+\frac{1}{2}(\mathbf{v}-\mathbf{u})=\frac{1}{2}(\mathbf{u}+\mathbf{v}) .
$$

A simple geometric consequence of this is that the diagonals of a parallelogram divide each other into equal parts. Namely, if $S$ is the fourth corner in the parallelogram with sides $\mathbf{u}$ and $\mathbf{v}$, then $\overrightarrow{O S}=\mathbf{u}+\mathbf{v}$. It thus follows from (1) that $M$ lies halfway between $O$ and $S$.

Example 2. Let $O, P, Q, R$ be four points in space and let

$$
\mathbf{u}=\overrightarrow{O P} ; \quad \mathbf{v}=\overrightarrow{O Q} ; \quad \mathbf{w}=\overrightarrow{O R} \text {. }
$$

By the centre of mass of the triangle $P Q R$ we mean the point $N$ defined by

$$
\overrightarrow{O N}=\frac{1}{3}(\mathbf{u}+\mathbf{v}+\mathbf{w}) .
$$

The three medians of the triangle $P Q R$ intersect at the point $N$. Recall that a median of a triangle is a line segment connecting a vertex to the midpoint of the opposite side.

In order to prove this let $M$ be the midpoint of the segment $P Q$. Then (by (1))

$$
\overrightarrow{R M}=\overrightarrow{O M}-\overrightarrow{O R}=\frac{1}{2}(\mathbf{u}+\mathbf{v})-\mathbf{w}=\frac{1}{2}(\mathbf{u}+\mathbf{v}-2 \mathbf{w}) .
$$



![](https://cdn.mathpix.com/cropped/2022_12_13_cabdc435b88729520c88g-05.jpg?height=322&width=439&top_left_y=316&top_left_x=802)

Moreover,

$$
\overrightarrow{R N}=\overrightarrow{O N}-\overrightarrow{O R}=\frac{1}{3}(\mathbf{u}+\mathbf{v}+\mathbf{w})-\mathbf{w}=\frac{1}{3}(\mathbf{u}+\mathbf{v}-2 \mathbf{w}) .
$$

We have shown that

$$
2 \overrightarrow{R M}=3 \overrightarrow{R N},
$$

so $N$ lies on the median $R M$ and divides it according to the ratio $2: 1$. By symmetry of the expression (2), the point $N$ is also on the other medians.

\section{Exercises.}

1. Let $A$ and $B$ be two points and $O$ a third point. Let $\mathbf{a}=\overrightarrow{O A}, \mathbf{b}=\overrightarrow{O B}$, and let $M$ be the midpoint of the line segment $A B$. Express the following

![](https://cdn.mathpix.com/cropped/2022_12_13_cabdc435b88729520c88g-05.jpg?height=71&width=1290&top_left_y=1382&top_left_x=431)

2. Simplify the following sums:
a) $\overrightarrow{O B}+\overrightarrow{B D}+\overrightarrow{D C}$
c) $\overrightarrow{A B}+\overrightarrow{O A}+\overrightarrow{B D}$
b) $\overrightarrow{A C}+\overrightarrow{C O}+\overrightarrow{O B}$
d) $\overrightarrow{B D}-\overrightarrow{B A}+\overrightarrow{D L}$

3. Prove that a point $N$ is the centre of mass of a triangle $P Q R$ if and only if

$$
\overrightarrow{N P}+\overrightarrow{N Q}+\overrightarrow{N R}=\mathbf{0} \text {. }
$$

4. Let $A B C$ be a triangle, $A_{1}$ the midpoint on $B C, B_{1}$ the midpoint on $A C$, and $C_{1}$ the midpoint of $A B$. Prove that the vectors $\overrightarrow{A A_{1}}, \overrightarrow{B B_{1}}$, and $\overrightarrow{C C_{1}}$ can be used to form a triangle.

5. A median in a tetrahedron is the line segment from a vertex to the centre of mass of the opposite side. Let $O$ be an arbitrary point and $P Q R S$ a tetrahedron. Prove that the medians of $P Q R S$ intersect at a point $T$ which is given by

$$
\overrightarrow{O T}=\frac{1}{4}(\overrightarrow{O P}+\overrightarrow{O Q}+\overrightarrow{O R}+\overrightarrow{O S}) .
$$

The point $T$ is called the centre of mass of the tetrahedron. 

\section{Bases and coordinates}

We are now properly equipped to begin our journey in analytic geometry and introduce the concepts of bases and coordinate systems. We start by defining basis for a line.

\section{Basis for a line.}

Let $\ell$ be a line in space. We say that a vector $\mathbf{u}$ is parallel to $\ell$, or simply that $\mathbf{u}$ belongs to $\ell$, if $\mathbf{u}$ can be represented by a directed line segment of $\ell$. Thus by " $\mathbf{u} \in \ell$ ", we really mean that some representative of $\mathbf{u}$ belongs to $\ell$. We hence use the phrase "belongs to" in slightly different meanings. This should not cause confusion, as long as the reader is aware of the distinction.

![](https://cdn.mathpix.com/cropped/2022_12_13_cabdc435b88729520c88g-07.jpg?height=314&width=317&top_left_y=954&top_left_x=839)

Definition 1. Fix a line $\ell$ and let $\mathbf{e} \neq \mathbf{0}$ be a vector in $\ell$. For any other vector $\mathbf{u}$ in $\ell$ there is then an unique real number $x$ such that

$$
\mathbf{u}=x \mathbf{e} .
$$

The vector $\mathbf{e}$ is called a basis for the line $\ell$ and $x$ is the coordinate of $\mathbf{u}$ with respect to the basis $\mathbf{e}$.

\section{Basis for a plane.}

As above, we say that a vector $\mathbf{u}$ belongs to a plane $M$ if $\mathbf{u}$ can be represented by a line segment in $M$. Let $\mathbf{e}_{1}, \mathbf{e}_{2}$ be two non-parallel vectors in a plane $M$. We claim that each vector $\mathbf{u}$ in $M$ can be written

$$
\mathbf{u}=x_{1} \mathbf{e}_{1}+x_{2} \mathbf{e}_{2}
$$

where $x_{1}$ and $x_{2}$ are real numbers.

To show this, we first choose two lines $\ell_{1}$ and $\ell_{2}$ in $M$ such that $\mathbf{e}_{1}$ is in $\ell_{1}$ and $\mathbf{e}_{2}$ is in $\ell_{2}$. Let $O$ be the point of intersection between $\ell_{1}$ and $\ell_{2}$. To help our geometric intuition, we will in the following fix $O$ as our "origin", and place all vectors in $M$ so that they emanate from the point $O$ (that is $\mathbf{e}_{1}=\overrightarrow{O P_{1}}$ for some point $P_{1}$ on $\ell_{1}$, $\mathbf{u}=\overrightarrow{O P}$, and so on.)

![](https://cdn.mathpix.com/cropped/2022_12_13_cabdc435b88729520c88g-08.jpg?height=323&width=377&top_left_y=489&top_left_x=836)

We then decompose $\mathbf{u}$ into a sum

$$
\mathbf{u}=\mathbf{u}_{1}+\mathbf{u}_{2}
$$

where $\mathbf{u}_{1}$ is on $\ell_{1}$ and $\mathbf{u}_{2}$ is on $\ell_{2}$. As in (1) we can then write

$$
\mathbf{u}_{1}=x_{1} \mathbf{e}_{1} \quad \text { and } \quad \mathbf{u}_{2}=x_{2} \mathbf{e}_{2}
$$

for some uniquely determined real numbers $x_{1}$ and $x_{2}$. This proves (2).

Definition 2. Two non-parallel vectors $\mathbf{e}_{1}, \mathbf{e}_{2}$ in a plane $M$ are called a basis for $M$. Given a vector $\mathbf{u} \in M$, the numbers $x_{1}$ and $x_{2}$ in (2) are uniquely determined; they are called the coordinates of $\mathbf{u}$ with respect to the basis $\mathbf{e}_{1}$, $\mathbf{e}_{2}$. If the basis is fixed, and no misunderstandings can arise, we can suppress the basis vectors in (2), and simply write

$$
\mathbf{u}=\left(x_{1}, x_{2}\right) .
$$

\section{Basis for the three-dimensional space.}

To describe all vectors in space in a similar way, we need three vectors $\mathbf{e}_{1}, \mathbf{e}_{2}, \mathbf{e}_{3}$ which are non-coplanar (i.e. they do not lie in one and the same plane). We assert that every vector $\mathbf{u}$ can be written as

$$
\mathbf{u}=x_{1} \mathbf{e}_{1}+x_{2} \mathbf{e}_{2}+x_{3} \mathbf{e}_{3}
$$

where $x_{1}, x_{2}, x_{3}$ are real numbers, uniquely determined by $\mathbf{u}$.

To prove this, we proceed in two steps. First, let $M$ be a plane containing $\mathbf{e}_{1}$ and $\mathbf{e}_{2}$ and let $\ell$ be a line containing $\mathbf{e}_{3}$. Let $O$ be the point of intersection between $\ell$ and $M$; in the following we place all vectors so that they emanate from $O$. We decompose $\mathbf{u}$ into a sum

$$
\mathbf{u}=\mathbf{u}^{\prime}+\mathbf{u}^{\prime \prime}, \quad \mathbf{u}^{\prime} \in M, \mathbf{u}^{\prime \prime} \in \ell .
$$

Applying (2) and (1) we can write $\mathbf{u}^{\prime}=x_{1} \mathbf{e}_{1}+x_{2} \mathbf{e}_{2}$ and $u^{\prime \prime}=x_{3} \mathbf{e}_{3}$ for some (unique) real numbers $x_{1}, x_{2}, x_{3}$. This proves (3). 

![](https://cdn.mathpix.com/cropped/2022_12_13_cabdc435b88729520c88g-09.jpg?height=423&width=526&top_left_y=309&top_left_x=759)

DEfinition 3. Three vectors $\mathbf{e}_{1}, \mathbf{e}_{2}, \mathbf{e}_{3}$ which are non-coplanar are called a basis for three-dimensional space. If $\mathbf{u}$ is a vector in space then the numbers $x_{1}$, $x_{2}, x_{3}$ in (3) are called the coordinates of $\mathbf{u}$ with respect to the basis $\mathbf{e}_{1}, \mathbf{e}_{2}$, $\mathbf{e}_{3}$. If the basis is understood, we can abbreviate the notation (3) and write

$$
\mathbf{u}=\left(x_{1}, x_{2}, x_{3}\right) .
$$

We also say that three non-coplanar vectors $\mathbf{e}_{1}, \mathbf{e}_{2}, \mathbf{e}_{3}$ are linearly independent and we call a vector $\mathbf{u}$ as in (3) a linear combination of these vectors.

Example. Let $O P Q R$ be a tetrahedron. The vectors $\mathbf{e}_{1}=\overrightarrow{O P}, \mathbf{e}_{2}=\overrightarrow{O Q}, \mathbf{e}_{3}=\overrightarrow{O R}$ then form a basis for three-dimensional space. Let $N$ be the centre of mass of the triangle $P Q R$. By Example 2 in the previous section, we then have

$$
\overrightarrow{O N}=(1 / 3,1 / 3,1 / 3)
$$

with respect to this basis. What are the coordinates of the basis vectors $\mathbf{e}_{1}, \mathbf{e}_{2}, \mathbf{e}_{3}$ ?

\section{Computing with coordinates.}

When we have a fixed basis for three-dimensional space, we can perform vector addition and multiplication by scalars by computing directly with coordinates relative to this basis. If

$$
\mathbf{u}=x_{1} \mathbf{e}_{1}+x_{2} \mathbf{e}_{2}+x_{3} \mathbf{e}_{3} \quad \mathbf{v}=y_{1} \mathbf{e}_{1}+y_{2} \mathbf{e}_{2}+y_{3} \mathbf{e}_{3} \quad \text { and } \quad s \in \mathbb{R}
$$

then

$$
\begin{aligned}
\mathbf{u}+\mathbf{v} & =\left(x_{1} \mathbf{e}_{1}+x_{2} \mathbf{e}_{2}+x_{3} \mathbf{e}_{3}\right)+\left(y_{1} \mathbf{e}_{1}+y_{2} \mathbf{e}_{2}+y_{3} \mathbf{e}_{3}\right) \\
& =\left(x_{1}+y_{1}\right) \mathbf{e}_{1}+\left(x_{2}+y_{2}\right) \mathbf{e}_{2}+\left(x_{3}+y_{3}\right) \mathbf{e}_{3} .
\end{aligned}
$$

and

$$
\begin{aligned}
s \mathbf{u} & =s\left(x_{1} \mathbf{e}_{1}+x_{2} \mathbf{e}_{2}+x_{3} \mathbf{e}_{3}\right) \\
& =\left(s x_{1}\right) \mathbf{e}_{1}+\left(s x_{2}\right) \mathbf{e}_{2}+\left(s x_{3}\right) \mathbf{e}_{3} .
\end{aligned}
$$

Thus, we may write:

$$
\begin{gathered}
\mathbf{u}+\mathbf{v}=\left(x_{1}, x_{2}, x_{3}\right)+\left(y_{1}, y_{2}, y_{3}\right)=\left(x_{1}+y_{1}, x_{2}+y_{2}, x_{3}+y_{3}\right) \\
s \mathbf{u}=s\left(x_{1}, x_{2}, x_{3}\right)=\left(s x_{1}, s x_{2}, s x_{3}\right)
\end{gathered}
$$

\section{Projections.}

In the decomposition (4) of a vector $\mathbf{u}$, the vector $\mathbf{u}^{\prime}$ is called the projection of $\mathbf{u}$ parallel to the line $\ell$ on the plane $M$, and $\mathbf{u}^{\prime \prime}$ is called the projection of $\mathbf{u}$ parallel to $M$ on $\ell$.

If the line $\ell$ is normal to the plane $M$, then the projection $\mathbf{u}^{\prime}$ is called the orthogonal (or "right angled") projection of $\mathbf{u}$ on $M$.

![](https://cdn.mathpix.com/cropped/2022_12_13_cabdc435b88729520c88g-10.jpg?height=420&width=528&top_left_y=999&top_left_x=755)

If we decompose both $\mathbf{u}$ and $\mathbf{v}$ in this way, we find

$$
\mathbf{u}+\mathbf{v}=\left(\mathbf{u}^{\prime}+\mathbf{v}^{\prime}\right)+\left(\mathbf{u}^{\prime \prime}+\mathbf{v}^{\prime \prime}\right)
$$

which means that

$$
(\mathbf{u}+\mathbf{v})^{\prime}=\mathbf{u}^{\prime}+\mathbf{v}^{\prime} \quad \text { and } \quad(\mathbf{u}+\mathbf{v})^{\prime \prime}=\mathbf{u}^{\prime \prime}+\mathbf{v}^{\prime \prime},
$$

which reads "the projection of a sum of vectors equals the sum of the projections of the individual summands".

\section{Exercises.}

6. Let $O P Q R$ be a tetrahedron and introduce a basis for 3 -space by $\mathbf{e}_{1}=\overrightarrow{O P}$, $\mathbf{e}_{2}=\overrightarrow{O Q}, \mathbf{e}_{3}=\overrightarrow{O R}$. Let $A$ be the mid-point of the segment $O P$ and $B$ the mid-point of the segment $Q R$. Also, let $C$ be the mid-point on the segment $A B$. Determine the coordinates of the vectors $\overrightarrow{O A}, \overrightarrow{O B}$, and $\overrightarrow{O C}$ relative to the basis $\mathbf{e}_{1}, \mathbf{e}_{2}, \mathbf{e}_{3}$. 

\section{Linear Dependence}

In this section we introduce some basic terminology that will allow us to express relations between vectors in a more precise way. The concepts discussed below can be extended beyond the three-dimensional space.

Definition 4. Let $\mathbf{u}_{1}, \mathbf{u}_{2}, \ldots, \mathbf{u}_{k}$ be a collection of vectors. A vector $\mathbf{u}$ of the form

$$
\mathbf{u}=\lambda_{1} \mathbf{u}_{1}+\cdots+\lambda_{k} \mathbf{u}_{k},
$$

where $\lambda_{1}, \ldots, \lambda_{k}$ are real numbers, is called a linear combination of the vectors $\mathbf{u}_{1}, \ldots, \mathbf{u}_{k}$.

The collection $\mathbf{u}_{1}, \mathbf{u}_{2}, \ldots, \mathbf{u}_{k}$ is called linearly dependent if there are real numbers $\lambda_{1}, \ldots, \lambda_{k}$, not all equal to zero, such that

$$
\lambda_{1} \mathbf{u}_{1}+\cdots+\lambda_{k} \mathbf{u}_{k}=\mathbf{0} .
$$

Otherwise, i.e., if

$$
\lambda_{1} \mathbf{u}_{1}+\cdots+\lambda_{k} \mathbf{u}_{k}=\mathbf{0} \quad \Rightarrow \quad \lambda_{1}=\lambda_{2}=\cdots=\lambda_{k}=0,
$$

we say that the collection is linearly independent.

Example 1. The fact that two vectors $\mathbf{u}_{1}, \mathbf{u}_{2}$ are linearly dependent means precisely that there are $\lambda_{1}, \lambda_{2}$, not both zero, such that $\lambda_{1} \mathbf{u}_{1}+\lambda_{2} \mathbf{u}_{2}=\mathbf{0}$.

If $\lambda_{1} \neq 0$ this implies $\mathbf{u}_{2}=t \mathbf{u}_{1}$ where $t=-\lambda_{2} / \lambda_{1}$, so $\mathbf{u}_{1}$ and $\mathbf{u}_{2}$ are parallel. The same conclusion holds if $\lambda_{2} \neq 0$. Conversely, if $\mathbf{u}_{1}$ and $\mathbf{u}_{2}$ are parallel, say if $\mathbf{u}_{1}=t \mathbf{u}_{2}$, then the relation $1 \cdot \mathbf{u}_{1}+(-t) \mathbf{u}_{2}=\mathbf{0}$ shows that $\mathbf{u}_{1}, \mathbf{u}_{2}$ are linearly dependent.

Thus, two vectors are linearly dependent if and only if they are parallel.

The example above has the following generalisation for arbitrary collections of vectors.

THEOREM 5. A collection $\mathbf{u}_{1}, \ldots, \mathbf{u}_{k}$ is linearly dependent if and only if (at least) one $\mathbf{u}_{j}$ can be written as a linear combination of the other $\mathbf{u}_{i}$ 's.

Proof. $(\Rightarrow)$ Assume that $\mathbf{u}_{1}, \ldots, \mathbf{u}_{k}$ are linearly dependent. Then there are real numbers $\lambda_{1}, \ldots, \lambda_{k}$, not all zero, such that

$$
\lambda_{1} \mathbf{u}_{1}+\lambda_{2} \mathbf{u}_{2}+\cdots+\lambda_{k} \mathbf{u}_{k}=\mathbf{0} .
$$

We can without loss of generality assume that $\lambda_{1} \neq 0$. But then

$$
\mathbf{u}_{1}=\left(-\lambda_{2} / \lambda_{1}\right) \mathbf{u}_{2}+\cdots+\left(-\lambda_{k} / \lambda_{1}\right) \mathbf{u}_{2},
$$

which shows that $\mathbf{u}_{1}$ is a linear combination of $\mathbf{u}_{2}, \ldots, \mathbf{u}_{k}$.

$(\Leftarrow)$ Suppose that some $\mathbf{u}_{j}$ is a linear combination of the other $\mathbf{u}_{i}$ 's. We can assume, without loss of generality, that $j=1$ and that

$$
\mathbf{u}_{1}=t_{2} \mathbf{u}_{2}+\cdots+t_{k} \mathbf{u}_{k},
$$

for some real numbers $t_{2}, \ldots, t_{k}$. Then

$$
1 \cdot \mathbf{u}_{1}+\left(-t_{2}\right) \mathbf{u}_{2}+\cdots+\left(-t_{k}\right) \mathbf{u}_{k}=\mathbf{0} .
$$

Since the coefficient of $\mathbf{u}_{1}$ is not zero, we infer that the collection is linearly dependent.

REMARK 6. If a collection $\mathbf{u}_{1}, \ldots, \mathbf{u}_{k}$ is linearly dependent, then any larger collection $\mathbf{u}_{1}, \ldots, \mathbf{u}_{k}, \mathbf{u}_{k+1}, \ldots, \mathbf{u}_{n}$ is also linearly dependent. This holds, since if

$$
\lambda_{1} \mathbf{u}_{1}+\cdots+\lambda_{k} \mathbf{u}_{k}=\mathbf{0}
$$

where not all $\lambda_{j}$ are zero, then

$$
\lambda_{1} \mathbf{u}_{1}+\cdots+\lambda_{k} \mathbf{u}_{k}+0 \mathbf{u}_{k+1}+\cdots+0 \mathbf{u}_{n}=\mathbf{0} .
$$

Example 2. Now suppose that three vectors $\mathbf{u}_{1}, \mathbf{u}_{2}, \mathbf{u}_{3}$ are linearly dependent. Then one of them, say $\mathbf{u}_{3}$, can be written as a linear combination of $\mathbf{u}_{1}$ and $\mathbf{u}_{2}$ :

$$
\mathbf{u}_{3}=t_{1} \mathbf{u}_{1}+t_{2} \mathbf{u}_{2} .
$$

Hence if $\mathbf{u}_{1}$ and $\mathbf{u}_{2}$ are in a plane $M$, then $\mathbf{u}_{3}$ is also in $M$. Conversely, if $\mathbf{u}_{1}, \mathbf{u}_{2}$, $\mathbf{u}_{3}$ belong to a plane $M$, then they are linearly dependent. To see this, it suffices to observe that either $\mathbf{u}_{1}, \mathbf{u}_{2}$ are linearly dependent, whence $\mathbf{u}_{1}, \mathbf{u}_{2}, \mathbf{u}_{3}$ is also linearly dependent by the remark above, or $\mathbf{u}_{1}, \mathbf{u}_{2}$ is a basis for a plane $M$, whence $\mathbf{u}_{3} \in M$ implies that $\mathbf{u}_{3}$ is a linear combination of $\mathbf{u}_{1}$ and $\mathbf{u}_{2}$.

Thus, three vectors are linearly dependent if and only if they are coplanar. Equivalently, three vectors are linearly independent if and only if they form a basis for 3-space.

Example 3. Assume that the vectors $\mathbf{u}_{1}, \mathbf{u}_{2}, \mathbf{u}_{3}$ have coordinates

$$
\mathbf{u}_{1}=(1,-2,2) \quad, \quad \mathbf{u}_{2}=(-2,3,1) \quad, \quad \mathbf{u}_{3}=(-1,3,2)
$$

with respect to some basis for 3-space. We shall investigate whether or not the vectors $\mathbf{u}_{1}, \mathbf{u}_{2}, \mathbf{u}_{3}$ form a basis. To this end, we consider the vector equation

$$
\lambda_{1} \mathbf{u}_{1}+\lambda_{2} \mathbf{u}_{2}+\lambda_{3} \mathbf{u}_{3}=\mathbf{0}
$$

which is equivalent to the linear system

$$
\left\{\begin{aligned}
\lambda_{1}-2 \lambda_{2}-\lambda_{3} & =0 \\
-2 \lambda_{2}+3 \lambda_{2}+3 \lambda_{3} & =0 \\
2 \lambda_{1}+\lambda_{2}+2 \lambda_{3} & =0
\end{aligned}\right.
$$

Solving this with the elimination method gives the only solution $\lambda_{1}=\lambda_{2}=\lambda_{3}=0$. Hence the collection $\mathbf{u}_{1}, \mathbf{u}_{2}, \mathbf{u}_{3}$ is linearly independent and (by the result of Example 2) it forms a basis for the three-dimensional space.

A collection of four or more vectors in 3-space is always linearly dependent. To show this, it is enough to prove that four vectors are linearly dependent, for then every larger collection is linearly dependent as well. Thus let $\mathbf{u}_{1}, \mathbf{u}_{2}, \mathbf{u}_{3}, \mathbf{u}_{4}$ be four arbitrary vectors in 3-space. Then either $\mathbf{u}_{1}, \mathbf{u}_{2}, \mathbf{u}_{3}$ are linearly dependent, and therefore so are $\mathbf{u}_{1}, \mathbf{u}_{2}, \mathbf{u}_{3}, \mathbf{u}_{4}$, or $\mathbf{u}_{1}, \mathbf{u}_{2}, \mathbf{u}_{3}$ is a basis for 3-space, whence $\mathbf{u}_{4}$ is a linear combination of $\mathbf{u}_{1}, \mathbf{u}_{2}, \mathbf{u}_{3}$. In either case, $\mathbf{u}_{1}, \mathbf{u}_{2}, \mathbf{u}_{3}, \mathbf{u}_{4}$ is linearly dependent.

Example 4. Consider the vectors $u_{1}=(3,4,2), u_{2}=(5,3,1), u_{3}=(4,1,7)$ and $v=(7,10,-2)$ with respect to a given basis for the three-dimensional space. One can show that the vectors $u_{1}, u_{2}, u_{3}$ are linearly independent in the same way as in the previous example. Then these vectors form another basis for the threedimensional space. Let us determine the coordinates of the vector $v=(7,10,-2)$ with respect to this new basis. The question is to determine $x_{1}, x_{2}, x_{3}$ such that $x_{1} u_{1}+x_{2} u_{2}+x_{3} u_{3}=v$, that is,

$$
x_{1}(3,4,2)+x_{2}(5,3,1)+x_{3}(4,1,7)=(7,10,-2)
$$

which we write as

$$
\left\{\begin{array}{l}
3 x_{1}+5 x_{2}+4 x_{3}=7 \\
4 x_{1}+3 x_{2}+x_{3}=10 \\
2 x_{1}+x_{2}+7 x_{3}=-2
\end{array} .\right.
$$

We use Gauss elimination, and choose to first eliminate $x_{2}$ using the third equation. Multiply the third equation by $(-5)$ and add the multiple to the first equation, respectively by $(-3)$ and add the multiple to the second equation. The system becomes

$$
\left\{\begin{array} { r l } 
{ - 7 x _ { 1 } - 3 1 x _ { 3 } } & { = 1 7 } \\
{ - 2 x _ { 1 } - 2 0 x _ { 3 } } & { = 1 6 } \\
{ 2 x _ { 1 } + x _ { 2 } + 7 x _ { 3 } } & { = - 2 }
\end{array} \Longleftrightarrow \left\{\begin{array}{rl}
7 x_{1}+31 x_{3} & =-17 \\
x_{1}+10 x_{3} & =-8 . \\
x s_{1}+s_{2}+7 x_{3} & =-2
\end{array}\right.\right.
$$

We now multiply the second equation by $(-7)$ and add the multiple to the first equation to eliminate $s_{1}$ :

$$
\left\{\begin{array}{rl}
-39 x_{3} & =39 \\
x_{1}+10 x_{3} & =-8 \\
2 x_{1}+x_{2}+7 x_{3} & =-2
\end{array} .\right.
$$

We get $x_{3}=-1$ from the first equation, which yields $x_{1}=2$ in the second equation and finally $x_{2}=1$. The vector $v$ has coordinates $(2,1,-1)$ with respect to the basis $u_{1}, u_{2}, u_{3}$.

Exercises. In the following exercises, vectors are expressed by their coordinates relative to some fixed basis $\mathbf{e}_{1}, \mathbf{e}_{2}, \mathbf{e}_{3}$.

7. Prove that the vector $\mathbf{v}=(2,-7,1)$ lies in a plane spanned by the vectors $\mathbf{u}_{1}=(2,-1,3)$ and $\mathbf{u}_{2}=(1,1,2)$. (A plane containing two linearly independent vectors is called a plane spanned by the vectors in question.) Determine the coordinates for $\mathbf{v}$ with respect to the basis $\mathbf{u}_{1}, \mathbf{u}_{2}$.

8. Are the vectors $(1,-2,1),(2,-1,-1),(-1,-4,5)$ coplanar?

9. Prove that the vectors $(1,1,2),(4,4,9),(2,3,7)$ form a basis for the threedimensional space. Determine the coordinates of the vector $(5,4,3)$ relative to this basis.

10. For which values of $k$ are the following sets of vectors linearly independent?

a) $\left(k, k^{2}, k^{3}\right),(2,2,2)$

b) $(1,1,1),(1, k, 2 k),(k, 1, k)$;

c) $(1,-1,-k),(2, k, 4),(k, 2,-4)$. 

\section{Equations for Lines and Planes}

In this section we introduce equations for lines and planes in the three-dimensional space. Lines and planes are sets of points fulfilling certain conditions. An equation for a line or a plane is just way of stating this conditions. To this end, we need a concrete representation of points in the three-dimensional space. This is introduced by means of a basis and a so-called system of coordinates.

Fix a point $O$ in three-dimensional space. An arbitrary point $P$ can then be described by the position vector $\overrightarrow{O P}$. For a given basis $\mathbf{e}_{1}, \mathbf{e}_{2}, \mathbf{e}_{3}$, there are then unique numbers $x_{1}, x_{2}, x_{3}$ such that

$$
\overrightarrow{O P}=x_{1} \mathbf{e}_{1}+x_{2} \mathbf{e}_{2}+x_{3} \mathbf{e}_{3} .
$$

We associate with the point $P$ the same triple of numbers $\left(x_{1}, x_{2}, x_{3}\right)$ that forms the coordinates of the position vector $\overrightarrow{O P}$ with respect to this basis. If the coordinate system is clear from the context, we can simply write

$$
P=\left(x_{1}, x_{2}, x_{3}\right) .
$$

The fixed point $O$ together with a given basis $\mathbf{e}_{1}, \mathbf{e}_{2}, \mathbf{e}_{3}$ are said to form the coordinate system $O \mathbf{e}_{1} \mathbf{e}_{2} \mathbf{e}_{3}$.

Remark 7. In a similar way we can describe points in a plane $M$. Let $O$ be a point in $M$ and $\mathbf{e}_{1}, \mathbf{e}_{2}$ is a basis for $M$. Then for each point $P$ in $M$ we can write

$$
\overrightarrow{O P}=x_{1} \mathbf{e}_{1}+x_{2} \mathbf{e}_{2}
$$

for unique $x_{1}, x_{2} \in \mathbf{R}$. We say that $x_{1}, x_{2}$ are the coordinates of $P$ in the coordinate system $O \mathbf{e}_{1} \mathbf{e}_{2}$ for $M$. In short: $P=\left(x_{1}, x_{2}\right)$.

Throughout the rest of this section we fix a coordinate system $O \mathbf{e}_{1} \mathbf{e}_{2} \mathbf{e}_{3}$ for threedimensional space. Each point can then be identified with its coordinates, which we denote by $(x, y, z)$ rather than $\left(x_{1}, x_{2}, x_{3}\right)$.

\section{Parametric equation of a line}

Let $\ell$ be a line in space. Suppose that $\ell$ passes through a point $Q$ and that a vector $\mathbf{u} \neq \mathbf{0}$ is parallel to $\ell$. Then a point $P$ belongs to $\ell$ if and only if

$$
\overrightarrow{Q P}=t \mathbf{u}
$$

for some $t \in \mathbf{R}$. The vector $\mathbf{u}$ is called a direction vector of $\ell$.

Denote by $(a, b, c)$ the coordinates of $\mathbf{u}$ with respect to the basis $\mathbf{e}_{1}, \mathbf{e}_{2}$, e $\mathbf{e}_{3}$. Thus

$$
\mathbf{u}=a \mathbf{e}_{1}+b \mathbf{e}_{2}+c \mathbf{e}_{3} .
$$

If $Q_{0}=\left(x_{0}, y_{0}, z_{0}\right)$ and $P=(x, y, z)$, then the vector $\overrightarrow{Q P}=\overrightarrow{O P}-\overrightarrow{O Q}$ has coordinates $\left(x-x_{0}, y-y_{0}, z-z_{0}\right)$. Hence (1) can be cast in the form

$$
\left\{\begin{array}{l}
x-x_{0}=a t \\
y-y_{0}=b t \\
z-z_{0}=c t
\end{array} \quad, \quad t \in \mathbf{R} .\right.
$$

The relation (2) is known as the parametric representation of the line $\ell$.

![](https://cdn.mathpix.com/cropped/2022_12_13_cabdc435b88729520c88g-16.jpg?height=366&width=485&top_left_y=728&top_left_x=755)

Example 1. Consider the line $\ell$ which passes through the points $Q=(3,-6,-5)$ and $R=(4,-3,-3)$. A direction vector of $\ell$ is

$$
\overrightarrow{Q R}=\overrightarrow{O R}-\overrightarrow{O Q}=(4,-3,-3)-(3,-6,-5)=(1,3,2) \text {. }
$$

Since $\ell$ passes through $Q$, we conclude that

$$
\left\{\begin{array}{l}
x-3=t \\
y+6=3 t \\
z+5=2 t
\end{array} \quad, \quad t \in \mathbf{R}\right.
$$

is a parametric representation for $\ell$.

\section{Parametric equation of a plane}

In a similar way, one can represent a plane $M$ in space. Namely, let $Q$ be a point in $M$ and $\mathbf{u}, \mathbf{v}$ a basis for $M$, i.e. two non-parallel vectors which are parallel to $M$. Then a point $P$ in space belongs to $M$ if and only if the vector $\overrightarrow{Q P}$ belongs to $M$, which is equivalent to the fact that

$$
\overrightarrow{Q P}=s \mathbf{u}+t \mathbf{v}
$$

for some $s, t \in \mathbf{R}$. The numbers $s, t$ are the coordinates for $P$ in the coordinate system $Q \mathbf{u v}$ of $M$. Let us denote

![](https://cdn.mathpix.com/cropped/2022_12_13_cabdc435b88729520c88g-17.jpg?height=553&width=1239&top_left_y=388&top_left_x=405)

With $P=(x, y, z), \overrightarrow{Q P}=\left(x-x_{0}, y-y_{0}, z-z_{0}\right), \mathbf{u}=(a, b, c)$ and $\mathbf{v}=\left(a^{\prime}, b^{\prime}, c^{\prime}\right)$, the equation (3) can be written as

$$
\left\{\begin{array}{l}
x-x_{0}=a s+a^{\prime} t \\
y-y_{0}=b s+b^{\prime} t \\
z-z_{0}=c s+c^{\prime} t
\end{array} \quad, \quad s, t \in \mathbf{R} .\right.
$$

This formula is called a parametric representation of the plane $M$.

Example 2. Consider the plane $M$ passing through the points $Q=(1,2,0), R_{1}=$ $(0,1,1)$, and $R_{2}=(2,-1,-3)$. Two non-parallel vectors in $M$ are

$$
\mathbf{u}=\overrightarrow{R_{1}}=(-1,-1,1) \quad, \quad \mathbf{v}=\overrightarrow{Q_{2}}=(1,-3,-3) .
$$

Hence

$$
\left\{\begin{aligned}
x-1 & =-s+t \\
y-2 & =-s-3 t \quad, \quad s, t \in \mathbf{R} \\
z & =s-3 t
\end{aligned}\right.
$$

is a parametric representation of $M$.

Example 3. Let us determine the point of intersection between the line $\ell$ of Example 1 and the plane $M$ of Example 2. To this end, we have to distinguish between the $t$-parameters in the representations for $\ell$ and $M$ and write

$$
\ell:\left\{\begin{array}{l}
x-3=t_{1} \\
y+6=3 t_{1} \\
z+5=2 t_{1}
\end{array} \quad, \quad M:\left\{\begin{array}{rl}
x-1 & =-s+t_{2} \\
y-2 & =-s-3 t_{2} \\
z & =s-3 t_{2}
\end{array} .\right.\right.
$$

At the point of intersection, the values of $x, y$, and $z$ must match, i.e.,

$$
\left\{\begin{array} { r } 
{ 3 + t _ { 1 } = 1 - s + t _ { 2 } } \\
{ - 6 + 3 t _ { 1 } = 2 - s - 3 t _ { 2 } } \\
{ - 5 + 2 t _ { 1 } = s - 3 t _ { 2 } }
\end{array} \Leftrightarrow \left\{\begin{array}{r}
s+t_{1}-t_{2}=-2 \\
s+3 t_{1}+3 t_{2}=8 \\
-s+2 t_{1}+3 t_{2}=5
\end{array} .\right.\right.
$$

After Gaussian elimination, this gives $s=2, t_{1}=-1$, and $t_{2}=3$. Inserting $t_{1}=-1$ into the equation for $\ell$ gives $(x, y, z)=(2,-9,-7)$.

The (point-normal) equation of a plane

We claim that planes in space correspond precisely to equations of the form

$$
A x+B y+C z=D
$$

where not all coefficients $A, B, C$ are zero. Indeed, suppose that $A \neq 0$ (the cases $B \neq 0$ and $C \neq 0$ are analogous). Then a point $(x, y, z)$ satisfies (5) if and only if

$$
\left\{\begin{array}{llc}
x-(D / A) & = & -(B / A) s-(C / A) t \\
y & = & s \\
z & = & t
\end{array}\right.
$$

for some $s, t \in \mathbf{R}$.

Thus (5) describes the plane passing through the point $(D / A, 0,0)$, which is parallel to the vectors $(-B / A, 1,0),(-C / A, 0,1)$.

Conversely, one can, by eliminating $s$ and $t$ in the parametric representation (4), prove that any plane can be described by an equation of the form (5). We omit the details, since we shall anyway find an easier method to prove this later on. Instead, we turn to some examples.

Example 4. Consider again the plane

$$
M:\left\{\begin{array}{rl}
x-1 & =-s+t \\
y-2 & =-s-3 t \\
z & =s-3 t
\end{array} \quad s, t \in \mathbf{R}\right.
$$

A point $(x, y, z)$ is in $M$ if and only if there are $s$ and $t$ satisfying these equations. To determine when this is the case, we can first eliminate $s$ from the last two equations, and then $t$ from the last equation:

$$
\begin{aligned}
& \left\{\begin{array} { r l } { x - 1 } & { = - s + t } \\{ y - 2 } & { = - s - 3 t } \\{ z } & { = s - 3 t }\end{array} \Leftrightarrow \left\{\begin{array}{cl}x & -1=-s+t \\-x+y-1= & -4 t \\x+z-1= & -2 t\end{array}\right.\right. \\
& \Leftrightarrow\left\{\begin{array}{rrr}x & -1 & =-s+t \\-x+y-1 & = & -4 t \\3 x-y+2 z-1 & = & 0\end{array} .\right.
\end{aligned}
$$

Since we can always choose $s$ and $t$ so that the first two equations are satisfied, we see that a point $(x, y, z)$ belongs to $M$ if and only if the third equation is satisfied, i.e., iff

$$
3 x-y+2 z-1=0 .
$$

Lines in space can be described as the intersection between two non-parallel planes. This is illustrated by the following example.

Example 5. The points $(x, y, z)$ which belong to both of the planes

$$
2 x+y-3 z=5 \text { and } x+2 y-z=4
$$

are precisely the solutions of the system

$$
\left\{\begin{array} { r l } 
{ 2 x + y - 3 z } & { = 5 } \\
{ x + 2 y - z } & { = 4 }
\end{array} \sim \left\{\begin{array}{r}
2 x+y-3 z=5 \\
3 y+z=3
\end{array} .\right.\right.
$$

Inserting $z=3 t$ (to obtain integer coefficients in the parametric representation) we get

$$
\left\{\begin{array}{l}
x=2+5 t \\
y=1-t \\
z=3 t
\end{array} .\right.
$$

The intersection line thus passes through the point $(2,1,0)$ and has direction vector $(5,-1,3)$.

REMark 8. To describe a line in space we need two equations of the form $A x+B y+C z=D$. On the other hand, if we only consider points in a plane $M$, and if $x, y$ denote coordinates with respect to some coordinate system in $M$, then one equation $A x+B y=C$ is sufficient to describe a line. If for example $A \neq 0$, then $(x, y)$ satisfies the equation if and only if

![](https://cdn.mathpix.com/cropped/2022_12_13_cabdc435b88729520c88g-20.jpg?height=151&width=419&top_left_y=388&top_left_x=799)

for some $t \in \mathbf{R}$. This is a parametric representation of a line in $M$ passing through the point $(C / A, 0)$, with direction vector $(-B / A, 1)$.

\section{Exercises.}

11. Give a parametric representation for the line passing through the points $(1,-1,4)$ and $(2,3,5)$.

12. Consider the lines

$$
\ell_{1}:\left\{\begin{array}{l}
x=2+t \\
y=1-t \\
z=2 t
\end{array} \quad, \quad \ell_{2}:\left\{\begin{array}{l}
x=1+2 t \\
y=\quad t \\
z=-1+t
\end{array}\right.\right.
$$

Do they intersect? Are they parallel?

13. Determine whether the following lines intersect:

$$
\left\{\begin{array} { l } 
{ x = 1 + 1 5 t } \\
{ y = - 4 - 2 1 t } \\
{ z = 5 + 3 3 t }
\end{array} \quad \left\{\begin{array}{l}
x=65 t \\
y=-11+91 t \\
z=16-143 t
\end{array}\right.\right.
$$

14. Find a parametric representation of the line $\ell$ which passes through the point $(3,2,-1)$ and intersects the lines

$$
\left\{\begin{array} { l } 
{ x = 1 + t } \\
{ y = t } \\
{ z = - 1 + t }
\end{array} \quad \text { and } \quad \left\{\begin{array}{l}
x=10+5 t \\
y=5+t \\
z=2+2 t
\end{array}\right.\right.
$$

15. Find a parametric representation of the plane $\pi$ which passes through the points $(2,3,0),(1,5,2)$, and $(-1,4,3)$.

16. Are the four points $(-1,-1,0),(0,4,1),(1,0,-1),(1,-3,-2)$ coplanar? 17. Find, in the form $A x+B y+C z=D$, the equation for the plane $\pi$ which passes through the point $(1,-1,2)$ and which contains the line

$$
\left\{\begin{array}{l}
x=3-t \\
y=2+2 t \\
z=1-3 t
\end{array} .\right.
$$

18. Prove that a line with direction-vector $(a, b, c)$ is parallel to the plane $A x+$ $B y+C z=D$ if and only if

$$
A a+B b+C c=0 .
$$

19. Find a parametric representation for the line passing through the point $(1,2,4)$ and which is parallel to the planes

$$
2 x+y-z=3 \quad \text { and } \quad 3 x-3 y+z=0 .
$$

20. Determine the equation for the plane which contains the line

$$
\left\{\begin{array}{rl}
3 x+4 y+z & =5 \\
x-y & =-6
\end{array}, \quad,\right.
$$

and which passes through the midpoint on the segment between the points $(1,1,2)$ and $(3,1,4)$.

\section{Answers to Exercises}

![](https://cdn.mathpix.com/cropped/2022_12_13_cabdc435b88729520c88g-21.jpg?height=62&width=859&top_left_y=1598&top_left_x=378)

$\begin{array}{llll}\text { 2. a) } \overrightarrow{O C} & \text { b) } \overrightarrow{A B} & \text { c) } \overrightarrow{O D} & \text { d) } \overrightarrow{A L}\end{array}$

6. $\overrightarrow{O A}=(1 / 2,0,0), \overrightarrow{O B}=(0,1 / 2,1 / 2), \overrightarrow{O C}=(1 / 4,1 / 4,1 / 4)$.

7. $\mathbf{v}=3 \mathbf{u}_{1}-4 \mathbf{u}_{2}$.

8. Yes, $(-1,-4,5)=3(1,-2,1)-2(2,-1,-1)$.

9. $(5,4,3)=23(1,1,2)-4(4,4,9)-(2,3,7)$.

The coordinates are thus $(23,-4,1)$.

10. a) $k \notin\{0,1\} \quad$ b) $k \notin\{1 / 2,1\} \quad$ c) $k \notin\{-2,4\}$.

11. $\left\{\begin{array}{l}x=1+t \\ y=-1+4 t \\ z=4+t\end{array}\right.$.

12. The lines do not intersect and they are not parallel.

13. The lines coincide. 14. $\ell: \quad\left\{\begin{array}{l}x=5+2 t \\ y=4+2 t \\ z=t\end{array}\right.$

15. $\pi: \quad\left\{\begin{array}{l}x=2-s-3 t \\ y=3+2 s+t \\ z=2 s+3 t\end{array}\right.$.

16. Yes.

17. $\pi: \quad 5 x-3 y-14 z=60$.

18. $\pi: \quad x-y-z=0$.

19. $\left\{\begin{array}{l}x=1+2 t \\ y=2+5 t \\ z=4+9 t\end{array}\right.$

20. $13 x+36 y+7 z=83$.