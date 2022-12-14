\title{
CHAPTER 5
}

\section{Cross Product and Volume Product}

In this chapter we introduce two fundamental tools in vector calculus, namely cross product (or vector product) and volume product. We start with some prerequisites.

\section{Orientation of Vectors}

Let $M$ be a plane in space and $\mathbf{u}, \mathbf{v}$ two non-parallel vectors in $M$. Consider the smallest rotation which turns $\mathbf{u}$ into a vector with the same direction as $\mathbf{v}$. If we view the rotation from one side of the plane, the rotation appears clockwise, but from the other side it will be perceived to be counterclockwise.

If $\mathbf{w}$ is a vector not in $M$, and if the rotation is counterclockwise when seen from the side of $\pi$ in the direction of $\mathbf{w}$, then the triple $\mathbf{u}, \mathbf{v}, \mathbf{w}$ is said to be positively oriented. If this is not the case, we say that the triple is negatively oriented.
![](https://cdn.mathpix.com/cropped/2022_12_13_2d4678b330ecd063230cg-01.jpg?height=220&width=744&top_left_y=1424&top_left_x=645)

A positively (negatively) oriented system is sometimes called a right handed (left handed ) system. Note that the ordering of the vectors is essential here. For example, if $\mathbf{u}, \mathbf{v}, \mathbf{w}$ is positively oriented, then $\mathbf{u}, \mathbf{w}, \mathbf{v}$ is negatively oriented.

\section{Cross Product}

Let $\mathbf{u}$ and $\mathbf{v}$ be two vectors in space and denote by $A(\mathbf{u}, \mathbf{v})$ the area of the parallelogram spanned by $\mathbf{u}$ and $\mathbf{v}$. If $\mathbf{u}$ and $\mathbf{v}$ are parallel, then of course $A(\mathbf{u}, \mathbf{v})=$ 0 ; otherwise, a simple geometric consideration shows that

$$
A(\mathbf{u}, \mathbf{v})=\|\mathbf{u}\|\|\mathbf{v}\| \sin \theta,
$$

where $\theta$ is the angle between $\mathbf{u}$ and $\mathbf{v}$ (in the interval $[0, \pi]$ ). 

![](https://cdn.mathpix.com/cropped/2022_12_13_2d4678b330ecd063230cg-02.jpg?height=276&width=442&top_left_y=404&top_left_x=814)

DEFInition 1. The cross product (or vector-product) $\mathbf{u} \times \mathbf{v}$ of $\mathbf{u}$ and $\mathbf{v}$ is the unique vector $\mathbf{w}$ with the following properties:

(i) $\mathbf{w}$ is orthogonal to $\mathbf{u}$ and to $\mathbf{v}$,

(ii) $\|\mathbf{w}\|=A(\mathbf{u}, \mathbf{v})$,

(iii) If $\mathbf{u}$ and $\mathbf{v}$ are not parallel, then $\mathbf{u}, \mathbf{v}, \mathbf{w}$ is a positively oriented triple.

REMARK 2 . Note that if the vectors $\mathbf{u}$ and $\mathbf{v}$ are parallel, then $A(\mathbf{u}, \mathbf{v})=0$ and $\mathbf{u} \times \mathbf{v}=\mathbf{0}$

Example 1. Let $\mathbf{e}_{1}, \mathbf{e}_{2}, \mathbf{e}_{3}$ be a positively oriented orthonormal basis. Then

$$
\begin{aligned}
& \mathbf{e}_{1} \times \mathbf{e}_{2}=-\mathbf{e}_{2} \times \mathbf{e}_{1}=\mathbf{e}_{3}, \\
& \mathbf{e}_{3} \times \mathbf{e}_{1}=-\mathbf{e}_{1} \times \mathbf{e}_{3}=\mathbf{e}_{2}, \\
& \mathbf{e}_{2} \times \mathbf{e}_{3}=-\mathbf{e}_{3} \times \mathbf{e}_{2}=\mathbf{e}_{1} .
\end{aligned}
$$

These formulae are geometrically obvious.

![](https://cdn.mathpix.com/cropped/2022_12_13_2d4678b330ecd063230cg-02.jpg?height=149&width=336&top_left_y=1595&top_left_x=840)

Cross Product and Projections. The cross product can (like the scalar product) be described using an orthogonal projection. Suppose that $\mathbf{v} \neq \mathbf{0}$ and that $M$ is a plane with normal vector $\mathbf{v}$. Denote by $\mathbf{u}^{\prime}$ the orthogonal projection of $\mathbf{u}$ on $M$. Then $A(\mathbf{u}, \mathbf{v})=A\left(\mathbf{u}^{\prime}, \mathbf{v}\right)$, because $\left\|\mathbf{u}^{\prime}\right\|$ is the height from $\mathbf{v}$ of the parallelogram spanned by $\mathbf{u}$ and $\mathbf{v}$. Let $\mathbf{w}=\mathbf{u} \times \mathbf{v}$.

Thus $\mathbf{w}$ is the vector orthogonal to $\mathbf{u}$ and $\mathbf{v}$, such that $\|\mathbf{w}\|=\left\|\mathbf{u}^{\prime}\right\|\|\mathbf{v}\|$ and the triple $\mathbf{u}, \mathbf{v}, \mathbf{w}$ is positively oriented. It is now easily seen that

$$
\mathbf{u} \times \mathbf{v}=\|\mathbf{v}\| \cdot T\left(\mathbf{u}^{\prime}\right)
$$



![](https://cdn.mathpix.com/cropped/2022_12_13_2d4678b330ecd063230cg-03.jpg?height=268&width=461&top_left_y=370&top_left_x=778)

where $T\left(\mathbf{u}^{\prime}\right)$ is the vector $\mathbf{u}^{\prime}$ rotated the angle $\pi / 2$ clockwise in $M$, seen from the tip of $\mathbf{v}$.

For the orthogonal projection, we know that if $\mathbf{u}_{1}$ and $\mathbf{u}_{2}$ are two vectors then the projection of their sum equals the sum of their projections, i.e. $\left(\mathbf{u}_{1}+\mathbf{u}_{2}\right)^{\prime}=\mathbf{u}_{1}^{\prime}+\mathbf{u}_{2}^{\prime}$. If the resulting vectors are rotated by $\pi / 2$ clockwise, it follows that

$$
T\left(\left(\mathbf{u}_{1}+\mathbf{u}_{2}\right)^{\prime}\right)=T\left(\mathbf{u}_{1}^{\prime}\right)+T\left(\mathbf{u}_{2}^{\prime}\right) .
$$

Using this together with (2) we obtain that

$$
\left(\mathbf{u}_{1}+\mathbf{u}_{2}\right) \times \mathbf{v}=\mathbf{u}_{1} \times \mathbf{v}+\mathbf{u}_{2} \times \mathbf{v} .
$$

We have thus proved the distributive law for the cross product.

It is also clear from the definition of the cross product that the following holds:

$$
(t \mathbf{u}) \times \mathbf{v}=t(\mathbf{u} \times \mathbf{v}), \quad t \in \mathbb{R},
$$

which together with (3) implies that the cross product obeys linearity in the first argument.

Another direct consequence of the definition is the following rule:

$$
\mathbf{v} \times \mathbf{u}=-\mathbf{u} \times \mathbf{v} .
$$

This rule is known as the anti-commutativity of the cross product.

Combining (5) with (3) and (4) we obtain the following rules for the second component:

$$
\mathbf{u} \times\left(\mathbf{v}_{1}+\mathbf{v}_{2}\right)=\mathbf{u} \times \mathbf{v}_{1}+\mathbf{u} \times \mathbf{v}_{2} \quad, \quad \mathbf{u} \times(t \mathbf{v})=t(\mathbf{u} \times \mathbf{v}),
$$

thus the cross product is linear in the second component. If $\mathbf{e}_{1}, \mathbf{e}_{2}, \mathbf{e}_{3}$ is a basis for three-dimensional space and

$$
\mathbf{u}=x_{1} \mathbf{e}_{1}+x_{2} \mathbf{e}_{2}+x_{3} \mathbf{e}_{3} \quad, \quad \mathbf{v}=y_{1} \mathbf{e}_{1}+y_{2} \mathbf{e}_{2}+y_{3} \mathbf{e}_{3}
$$

we use linearity to infer

$$
\mathbf{u} \times \mathbf{v}=x_{1} y_{1} \mathbf{e}_{1} \times \mathbf{e}_{1}+x_{1} y_{2} \mathbf{e}_{1} \times \mathbf{e}_{2}+\cdots+x_{3} y_{3} \mathbf{e}_{3} \times \mathbf{e}_{3} .
$$

Since $\mathbf{e}_{j} \times \mathbf{e}_{j}=\mathbf{0}$ and $\mathbf{e}_{j} \times \mathbf{e}_{k}=-\mathbf{e}_{k} \times \mathbf{e}_{j}$, this simplifies to

$$
\left(x_{1} y_{2}-x_{2} y_{1}\right) \mathbf{e}_{1} \times \mathbf{e}_{2}+\left(x_{1} y_{3}-x_{3} y_{1}\right) \mathbf{e}_{1} \times \mathbf{e}_{3}+\left(x_{2} y_{3}-x_{3} y_{2}\right) \mathbf{e}_{2} \times \mathbf{e}_{3} .
$$

In the important case when the basis $\mathbf{e}_{1}, \mathbf{e}_{2}, \mathbf{e}_{3}$ is orthonormal and positively oriented, we get (using Example 1) the following result.

THEOREM 3. Suppose that $\mathbf{e}_{1}, \mathbf{e}_{2}, \mathbf{e}_{3}$ is a positively oriented orthonormal basis and let $\mathbf{u}=x_{1} \mathbf{e}_{1}+x_{2} \mathbf{e}_{2}+x_{3} \mathbf{e}_{3}$ and $\mathbf{v}=y_{1} \mathbf{e}_{1}+y_{2} \mathbf{e}_{2}+y_{3} \mathbf{e}_{3}$. Then

$$
\mathbf{u} \times \mathbf{v}=\left(x_{2} y_{3}-x_{3} y_{2}\right) \mathbf{e}_{1}-\left(x_{1} y_{3}-x_{3} y_{1}\right) \mathbf{e}_{2}+\left(x_{1} y_{2}-x_{2} y_{1}\right) \mathbf{e}_{3} .
$$

REMARK 4. There is a well-known mnemonic trick to remember the above formula. This uses the concept of "determinants", which will be discussed in detail later in the course.

By definition a $2 \times 2$-determinant is given by

$$
\left|\begin{array}{ll}
a & b \\
c & d
\end{array}\right|=a d-b c .
$$

A $3 \times 3$-determinant is then defined by

$$
\left|\begin{array}{lll}
a_{1} & a_{2} & a_{3} \\
b_{1} & b_{2} & b_{3} \\
c_{1} & c_{2} & c_{3}
\end{array}\right|=a_{1}\left|\begin{array}{ll}
b_{2} & b_{3} \\
c_{2} & c_{3}
\end{array}\right|-a_{2}\left|\begin{array}{cc}
b_{1} & b_{3} \\
c_{1} & c_{3}
\end{array}\right|+a_{3}\left|\begin{array}{ll}
b_{1} & b_{2} \\
c_{1} & c_{2}
\end{array}\right| .
$$

This rule is called "expansion along the first row". We can now write

$$
\mathbf{u} \times \mathbf{v}=\left|\begin{array}{lll}
\mathbf{e}_{1} & \mathbf{e}_{2} & \mathbf{e}_{3} \\
x_{1} & x_{2} & x_{3} \\
y_{1} & y_{2} & y_{3}
\end{array}\right| .
$$

REMARK 5. We saw above that the cross product is non-commutative (it is in fact anti-commutative). The cross product does not obey the associatve law either. For example, if $\mathbf{e}_{1}, \mathbf{e}_{2}, \mathbf{e}_{3}$ is an orthonormal basis, then by Example 1,

$$
\mathbf{e}_{1} \times\left(\mathbf{e}_{1} \times \mathbf{e}_{2}\right)=-\mathbf{e}_{2} \quad \text { and } \quad\left(\mathbf{e}_{1} \times \mathbf{e}_{1}\right) \times \mathbf{e}_{2}=\mathbf{0} \times \mathbf{e}_{2}=\mathbf{0} .
$$

Thus it can happen that $\mathbf{u} \times(\mathbf{v} \times \mathbf{w}) \neq(\mathbf{u} \times \mathbf{v}) \times \mathbf{w}$. Example 2. Consider three points $P_{0}, P_{1}, P_{2}$, which in a positively oriented orthonormal system have coordinates $(2,3,-2),(4,1,1)$, and $(2,1,-1)$, respectively. We shall compute the area of the triangle $P_{0} P_{1} P_{2}$. This area equals to half the area of the parallelogram spanned by the vectors $\vec{P}_{0} P_{1}$ and $\overrightarrow{P_{0} P_{2}}$. The area of that parallelogram is the length of the cross product

$$
\overrightarrow{P_{0} P_{1}} \times \overrightarrow{P_{0} P_{2}}=(2,-2,3) \times(0,-2,1)=(4,-2,-4) .
$$

Thus the triangle $P_{0} P_{1} P_{2}$ has area

$$
\frac{1}{2} \sqrt{4^{2}+2^{2}+4^{2}}=3 .
$$

Example 3. If $\mathbf{e}_{1}, \mathbf{e}_{2}$ is an orthonormal basis in a plane $\pi$, we can choose a unit normal vector $\mathbf{e}_{3}$ to $\pi$ such that $\mathbf{e}_{1}, \mathbf{e}_{2}, \mathbf{e}_{3}$ becomes an orthonormal basis for space. Two vectors

$$
\mathbf{u}=x_{1} \mathbf{e}_{1}+x_{2} \mathbf{e}_{2} \quad, \quad \mathbf{v}=y_{1} \mathbf{e}_{1}+y_{2} \mathbf{e}_{2}
$$

in $\pi$ will then have coordinates $\left(x_{1}, x_{2}, 0\right)$ and $\left(y_{1}, y_{2}, 0\right)$, respectively, in the basis $\mathbf{e}_{1}, \mathbf{e}_{2}, \mathbf{e}_{3}$. The area of the parallelogram spanned by $\mathbf{u}$ and $\mathbf{v}$ therefore equals to the length of the cross product

$$
\left(x_{1}, x_{2}, 0\right) \times\left(y_{1}, y_{2}, 0\right)=\left(0,0, x_{1} y_{2}-x_{2} y_{1}\right),
$$

i.e. we have the formula

$$
A(\mathbf{u}, \mathbf{v})=\left|x_{1} y_{2}-x_{2} y_{1}\right| .
$$

Example 4. The cross product can be used to calculate the distance between lines. Assume a positively oriented orthonormal system, and let $\ell_{1}$ be the line through the points $(1,1,1)$ and $(4,5,3)$ while $\ell_{2}$ is the line passing through the points $(-1,-10,-1)$ and $(8,2,2)$. Thus $\ell_{1}$ has direction vector $(3,4,2)$ and $\ell_{2}$ has direction vector $(3,4,1)$. Since

$$
(3,4,2) \times(3,4,1)=(-4,3,0)
$$

we see that $\mathbf{e}=\frac{1}{5}(-4,3,0)$ is a unit vector orthogonal to both $\ell_{1}$ and $\ell_{2}$. If $P$ is a poin on $\ell_{1}$ and $Q$ a point on $\ell_{2}$, we infer that the absolute value of the scalar product $(\overrightarrow{P Q} \mid \mathbf{e})$ must equal to the distance between $\ell_{1}$ and $\ell_{2}$. Choosing, for example, $P=(1,1,1)$ and $Q=(8,2,2)$, we find that

$$
(\overrightarrow{P Q} \mid \mathbf{e})=-5 \text {. }
$$

The distance between $\ell_{1}$ and $\ell_{2}$ is thus 5 . Example 5. Determine a positively oriented orthonormal basis $e_{1}, e_{2}$ and $e_{3}$ such that $e_{1}$ and $e_{3}$ are parallel to the plane $3 x-5 y+4 z=7$.

Solution: Since $e_{1}$ and $e_{3}$ are parallel to the plane $3 x-5 y+4 z=7$, we may choose $e_{2}$ to be a normal vector of unit length to this plane, that is

$$
e_{2}=\frac{(3,-5,4)}{\|(3,-5,4)\|}=\frac{1}{\sqrt{50}}(3,-5,4)=\frac{1}{5 \sqrt{2}}(3,-5,4) .
$$

We may then choose $e_{1}$ as an arbitrary unit vector that is orthogonal to $e_{2}$, for instance

$$
e_{1}=\frac{(4,0,-3)}{\|(4,0,-3)\|}=\frac{1}{5}(4,0,-3) .
$$

Finally, for the chosen $e_{1}$ and $e_{2}$, we set $e_{3}=e_{1} \times e_{2}$ to ensure that these vectors form a positively oriented orthonormal basis. We have that

$e_{3}=e_{1} \times e_{2}=\frac{1}{5}(4,0,-3) \times \frac{1}{5 \sqrt{2}}(3,-5,4)=\frac{1}{25 \sqrt{2}}(-15,-25,-20)=-\frac{1}{5 \sqrt{2}}(3,5,4)$.

\section{Exercises.}

1. Prove that if $\mathbf{u}+\mathbf{v}+\mathbf{w}=\mathbf{0}$, then

$$
2 \mathbf{u} \times \mathbf{v}=\mathbf{v} \times \mathbf{w}+\mathbf{w} \times \mathbf{u} .
$$

2. Find the area of the triangle which in a positively oriented ON-system has its vertices at the points

a) $(1,2,3),(3,4,1),(2,0,2)$.

b) $(5,1,1),(2,3,2),(3,2,3)$.

c) $(1,0,0),(0,1,0),(0,0,1)$.

3. In a positively oriented ON-system, the points $(1,1,1)$ and $(0,3,3)$ are on the line $\ell_{1}$, and $(2,2,-4)$ and $(4,4,4)$ are on $\ell_{2}$. Find the distance between $\ell_{1}$ and $\ell_{2}$.

4. Prove that

$$
(\mathbf{u} \times \mathbf{v}) \times \mathbf{w}=(\mathbf{u} \mid \mathbf{w}) \mathbf{v}-(\mathbf{v} \mid \mathbf{w}) \mathbf{u} .
$$

HINT: To simplify the computations, one can choose an ON-basis $\mathbf{e}_{1}, \mathbf{e}_{2}$, $\mathbf{e}_{3}$ such that $\mathbf{u}=x_{1} \mathbf{e}_{1}$ and $\mathbf{v}=y_{1} \mathbf{e}_{1}+y_{2} \mathbf{e}_{2}$. 5. Prove that

$$
(\mathbf{u} \times \mathbf{v}) \times \mathbf{w}=\mathbf{u} \times(\mathbf{v} \times \mathbf{w})
$$

if and only if $\mathbf{u}$ is parallel to $\mathbf{w}$, or $\mathbf{u}$ and $\mathbf{w}$ are both orthogonal to $\mathbf{v}$.

Hint: Use the preceding exercise.

\section{Volume Product}

Cross product and scalar product can be combined to define the so-called volume product $V(\mathbf{u}, \mathbf{v}, \mathbf{w})$ of three vectors in space:

$$
V(\mathbf{u}, \mathbf{v}, \mathbf{w})=(\mathbf{u} \times \mathbf{v} \mid \mathbf{w}) .
$$

The motivation for the name is that the absolute value of $V(\mathbf{u}, \mathbf{v}, \mathbf{w})$ equals to the volume of the parallelepiped spanned by the vectors $\mathbf{u}, \mathbf{v}, \mathbf{w}$, if they are set from the same point.

![](https://cdn.mathpix.com/cropped/2022_12_13_2d4678b330ecd063230cg-07.jpg?height=301&width=412&top_left_y=1069&top_left_x=802)

To show this, note that the vector

$$
\mathbf{e}=\frac{\mathbf{u} \times \mathbf{v}}{\|\mathbf{u} \times \mathbf{v}\|}
$$

is a unit normal to the plane spanned by $\mathbf{u}$ and $\mathbf{v}$. Denote by $P$ the parallelepiped spanned by $\mathbf{u}, \mathbf{v}, \mathbf{w}$. From elementary geometry we know that the volume of $P$ equals the area of the "base parallelogram" spanned by $\mathbf{u}, \mathbf{v}$, times the height $h$ of $P$ above the plane spanned by $\mathbf{u}$ and $\mathbf{v}$. Then $h$ is the length of the orthogonal projection of $\mathbf{w}$ on the normal of the plane, i.e., $h=|(\mathbf{e} \mid \mathbf{w})|$. Since the base parallelogram has area $A(\mathbf{u}, \mathbf{v})=\|\mathbf{u} \times \mathbf{v}\|$, we infer that the volume of $P$ equals

$$
A(\mathbf{u}, \mathbf{v}) h=\|\mathbf{u} \times \mathbf{v}\| \cdot|(\mathbf{e} \mid \mathbf{w})|=|(\mathbf{u} \times \mathbf{v} \mid \mathbf{w})| .
$$

The asserted property of the volume product is proved.

When two vectors $\mathbf{u}$ and $\mathbf{v}$ are parallel we have $\mathbf{u} \times \mathbf{v}=\mathbf{0}$, so $V(\mathbf{u}, \mathbf{v}, \mathbf{w})=0$ in this case. More generally, the volume product is zero when the parallelepiped is degenerate, i.e., when the vectors $\mathbf{u}, \mathbf{v}, \mathbf{w}$ are linearly dependent. On the other hand, if $\mathbf{u}, \mathbf{v}, \mathbf{w}$ are linearly independent, the sign of $(\mathbf{u} \times \mathbf{v} \mid \mathbf{w})$ depends on whether or not the two vectors $\mathbf{u} \times \mathbf{v}$ and $\mathbf{w}$ lie on the same side of the plane spanned by $\mathbf{u}$ and $\mathbf{v}$. The volume product $V(\mathbf{u}, \mathbf{v}, \mathbf{w})$ is positive when the triple $\mathbf{u}, \mathbf{v}, \mathbf{w}$ is positively oriented and negative otherwise. Since the volume of the parallelepiped is the same regardless of how we choose to permute the vectors $\mathbf{u}, \mathbf{v}, \mathbf{w}$, only the sign can change under such a permutation:

$$
\begin{aligned}
V(\mathbf{u}, \mathbf{v}, \mathbf{w}) & =V(\mathbf{w}, \mathbf{u}, \mathbf{v})=V(\mathbf{v}, \mathbf{w}, \mathbf{u})=-V(\mathbf{u}, \mathbf{w}, \mathbf{v}) \\
& =-V(\mathbf{v}, \mathbf{u}, \mathbf{w})=-V(\mathbf{w}, \mathbf{v}, \mathbf{u}) .
\end{aligned}
$$

Combining the computational rules for the cross- and scalar- products, we find that

$$
V\left(s \mathbf{u}_{1}+t \mathbf{u}_{2}, \mathbf{v}, \mathbf{w}\right)=s V\left(\mathbf{u}_{1}, \mathbf{v}, \mathbf{w}\right)+t V\left(\mathbf{u}_{2}, \mathbf{v}, \mathbf{w}\right)
$$

for all real numbers $s$ and $t$. Thus we have linearity in the first argument for the volume product. We similarly have linearity in the second and in the third argument. In short: the volume product is tri-linear, i.e., linear in each of its three arguments.

Now let $\mathbf{e}_{1}, \mathbf{e}_{2}$, $\mathbf{e}_{3}$ be a basis for space, and take three vectors $\mathbf{u}=\left(x_{1}, x_{2}, x_{3}\right)$, $\mathbf{v}=\left(y_{1}, y_{2}, y_{3}\right), \mathbf{w}=\left(z_{1}, z_{2}, z_{3}\right)$, where coordinates are given according to the chosen basis. Then by linearity in the different arguments,

$$
\begin{aligned}
V(\mathbf{u}, \mathbf{v}, \mathbf{w}) & =V\left(x_{1} \mathbf{e}_{1}+x_{2} \mathbf{e}_{2}+x_{3} \mathbf{e}_{3}, \mathbf{v}, \mathbf{w}\right) \\
& =x_{1} V\left(\mathbf{e}_{1}, \mathbf{v}, \mathbf{w}\right)+x_{2} V\left(\mathbf{e}_{2}, \mathbf{v}, \mathbf{w}\right)+x_{3} V\left(\mathbf{e}_{3}, \mathbf{v}, \mathbf{w}\right) \\
& =\cdots=\sum x_{i} y_{j} z_{k} V\left(\mathbf{e}_{i}, \mathbf{e}_{j}, \mathbf{e}_{k}\right)
\end{aligned}
$$

Here the sum is taken over all possible choices of of $i, j, k \in\{1,2,3\}$, but since $V\left(\mathbf{e}_{i}, \mathbf{e}_{j}, \mathbf{e}_{k}\right)=0$ if two of them coincide, only six terms can be non-zero. Furthermore

$$
\begin{aligned}
V\left(\mathbf{e}_{1}, \mathbf{e}_{2}, \mathbf{e}_{3}\right) & =V\left(\mathbf{e}_{3}, \mathbf{e}_{1}, \mathbf{e}_{2}\right)=V\left(\mathbf{e}_{2}, \mathbf{e}_{3}, \mathbf{e}_{1}\right)=-V\left(\mathbf{e}_{1}, \mathbf{e}_{3}, \mathbf{e}_{2}\right) \\
& =-V\left(\mathbf{e}_{2}, \mathbf{e}_{1}, \mathbf{e}_{3}\right)=-V\left(\mathbf{e}_{3}, \mathbf{e}_{2}, \mathbf{e}_{1}\right) .
\end{aligned}
$$

This gives that $V(\mathbf{u}, \mathbf{v}, \mathbf{w})$ is equal to

$$
\left(x_{1} y_{2} z_{3}+x_{3} y_{1} z_{2}+x_{2} y_{3} z_{1}-x_{1} y_{3} z_{2}-x_{2} y_{1} z_{3}-x_{3} y_{2} z_{1}\right) V\left(\mathbf{e}_{1}, \mathbf{e}_{2}, \mathbf{e}_{3}\right) \text {. }
$$

The number in front of $V\left(\mathbf{e}_{1}, \mathbf{e}_{2}, \mathbf{e}_{3}\right)$ can now be recognised as the $3 \times 3$-determinant (see Remark 4 in the previous section)

$$
\left|\begin{array}{lll}
x_{1} & y_{1} & z_{1} \\
x_{2} & y_{2} & z_{2} \\
x_{3} & y_{3} & z_{3}
\end{array}\right| .
$$

We then have the formula

$$
V(\mathbf{u}, \mathbf{v}, \mathbf{w})=\left|\begin{array}{lll}
x_{1} & y_{1} & z_{1} \\
x_{2} & y_{2} & z_{2} \\
x_{3} & y_{3} & z_{3}
\end{array}\right| V\left(\mathbf{e}_{1}, \mathbf{e}_{2}, \mathbf{e}_{3}\right)
$$

This formula is particularly simple when the basis $\mathbf{e}_{1}, \mathbf{e}_{2}, \mathbf{e}_{3}$ is orthonormal. Then $V\left(\mathbf{e}_{1}, \mathbf{e}_{2}, \mathbf{e}_{3}\right)=1$, so we simply have:

$$
V(\mathbf{u}, \mathbf{v}, \mathbf{w})=\left|\begin{array}{lll}
x_{1} & y_{1} & z_{1} \\
x_{2} & y_{2} & z_{2} \\
x_{3} & y_{3} & z_{3}
\end{array}\right| .
$$

Example 1. Suppose that the coordinates of the vectors $\mathbf{u}, \mathbf{v}, \mathbf{w}$ are $(2,-1,3)$, $(0,3,2)$, and $(3,5,1)$, respectively, with respect to a positively oriented orthonormal basis. We get

$$
V(\mathbf{u}, \mathbf{v}, \mathbf{w})=\left|\begin{array}{ccc}
2 & -1 & 3 \\
0 & 3 & 2 \\
3 & 5 & 1
\end{array}\right|=-47 .
$$

The volume of the parallelepiped spanned by $\mathbf{u}, \mathbf{v}, \mathbf{w}$ is thus 47 .

As we mentioned above, three vectors are linearly dependent if and only if they are coplanar, i.e., if the corresponding parallelepiped has volume zero. According to (10) this is equivalent to the fact that the determinant of the coordinates of the vectors is zero.

Example 2. To decide when the vectors $(1, a, 2),(-1,7,1+a)$, and $(1,-1,1)$ are linearly dependent, we form the determinant

$$
\left|\begin{array}{ccc}
1 & a & 2 \\
-1 & 7 & 1+a \\
1 & -1 & 1
\end{array}\right|=a^{2}+3 a-4=(a-1)(a+4) .
$$

The vectors are thus linearly dependent if $a=1$ or $a=-4$.

\section{Exercises.}

6. Motivate the identity

$$
(\mathbf{u} \times \mathbf{v} \mid \mathbf{w})=(\mathbf{u} \mid \mathbf{v} \times \mathbf{w}) .
$$

7. The volume of a tetrahedron spanned by three vectors $\mathbf{u}, \mathbf{v}, \mathbf{w}$, rooted at the same point, equals to $1 / 6$ of the volume of the parallelepiped spanned by $\mathbf{u}, \mathbf{v}$, and $\mathbf{w}$. Find the volume of the tetrahedron with vertices at

a) $(2,1,0),(3,5,2),(4,1,2),(6,1,5)$.

b) $(-2,2,-3),(2,1,3),(1,4,-2),(0,5,1)$. 8. A tetrahedron with volume 5 has three of its vertices at the points $(2,1,-1)$, $(3,0,1),(2,-1,3)$. The fourth vertex is on the positive $y$-axis. Determine its $y$-coordinate.

9. For which values of $a$ and $b$ are the three vectors

$$
(a, b, b) \quad, \quad(b, a, b) \quad, \quad(b, b, a)
$$

linearly dependent?

10. For which values of $a$ are the four points

$$
(0,2,1) \quad, \quad(-a, 1,0) \quad, \quad(-3,3,-a) \quad, \quad(3,-3,1+a)
$$

in the same plane? 

\section{Quaternions}

We have seen that neither the commutative, nor the associative laws hold for the cross product. One can ask whether there is some other way of defining multiplication between vectors, so that all the usual computational laws are satisfied. For vectors in a plane, this is true, since plane vectors can be identified with complex numbers. In the definition of multiplication of complex numbers, one starts with the familiar identity $i^{2}=-1$; if the usual laws of calculation shall hold, the product of complex numbers must be

$$
\left(x_{1}+i x_{2}\right)\left(y_{1}+i y_{2}\right)=\left(x_{1} y_{1}-x_{2} y_{2}\right)+i\left(x_{1} y_{2}+x_{2} y_{1}\right) .
$$

As we know, this definition does indeed satisfy all the usual computational rules. Vectors in three-dimensional space can formally be written

$$
x_{1}+x_{2} i+x_{3} j
$$

and if we still insist that $i^{2}=-1$, so that the multiplication when $x_{3}=0$ corresponds to multiplication of complex numbers, we just need to establish the rules for multiplication with $j$. In particular, the product $i j$ must be a new vector

$$
i j=a+b i+c j .
$$

If this is multiplied by $i$, using that $i^{2}=-1$, we obtain

$$
-j=-b+i a+i j c .
$$

If we here substitute $i j$ for the right hand side of (12), we get after simplification that

$$
0=(a c-b)+(b c+a) i+\left(c^{2}+1\right) j .
$$

This does not make sense, for we can not have $c^{2}+1=0$ for a real number $c$.

The above argument shows that it is impossible to extend the multiplication of complex numbers to multiplication of triples of numbers in a way such that the usual laws of calculation are preserved. Annoyed by this type of inconveniences, the Irish mathematician Hamilton tried to instead define multiplication between 4-tuples

$$
\mathbf{x}=x_{0}+x_{1} i+x_{2} j+x_{3} k .
$$

For reasons soon to be made clear, the coefficients are enumerated from 0 to 3 , rather than from 1 to 4 . In 1843, Hamilton discovered that if one abandons the commutative law $\mathbf{x y}=\mathbf{y} \mathbf{x}$ and defines

$$
\begin{aligned}
& i^{2}=j^{2}=k^{2}=-1 \\
& i j=-j i=k \quad, \quad j k=-k j=i \quad, \quad k i=-i k=j
\end{aligned}
$$

then multiplication of 4-tuples will satisfy all other rules of calculation. Hamilton coined the term quaternions for the set of 4-tuples with this multiplication. He also showed how to define division by a non-zero quaternion.

In 1878 , the German mathematician Frobenius proved that if we want to define multiplication of $n$-tuples such that division by non-zero elements is always possible, and if we only are prepared to abandon the commutative law for multiplication, then $n$ must be either 1, 2, or 4. Except for the real and complex fields, Hamilton's quaternions are the only possibility.

Hamilton called the number $x_{0}$ the scalar part of the quaternion (13) and $x_{1} i+$ $x_{2} j+x_{3} k$ is the vector part. If one multiplies two quaternions with scalar parts zero and uses the identities in (14), one finds after a little calculation that

$$
\begin{aligned}
& \left(x_{1} i+x_{2} j+x_{3} k\right)\left(y_{1} i+y_{2} j+y_{3} k\right)=-\left(x_{1} y_{1}+x_{2} y_{2}+x_{3} y_{3}\right)+ \\
& +\left(x_{2} y_{3}-x_{3} y_{2}\right) i+\left(x_{3} y_{1}-x_{1} y_{3}\right) j+\left(x_{1} y_{2}-x_{2} y_{1}\right) k .
\end{aligned}
$$

The scalar part of the right hand sign equals the negative of the scalar product of the vectors in the left hand side, and the vector part of the right hand side equals the cross product of the vectors in the left hand side. The scalar product is older, even though the name was invented by Hamilton, but the cross product was discovered in this way, as a by-product of multiplication of quaternions. Hamilton also interpreted the quaternions geometrically and defined the scalar- and cross products in a basis-independent way, as we have done in this chapter.

\section{Exercises.}

11. Prove that the formula (14) implies that

$$
\left(x_{0}+x_{1} i+x_{2} j+x_{3} k\right)\left(x_{0}-x_{1} i-x_{2} j-x_{3} k\right)=x_{0}^{2}+x_{1}^{2}+x_{2}^{2}+x_{3}^{2},
$$

and that one therefore can define division by non-zero quaternions.

\section{Answers to Exercises}

2. a) $3 \sqrt{2}$. b) $\sqrt{26} / 2$. c) $\sqrt{3} / 2$.

3. 3 .

7. a) $4 / 3$. b) 10 .

8. $y=8$.

9. $a=b$ or $a=-2 b$.

10. $a=1$ and $a=-9 / 4$.