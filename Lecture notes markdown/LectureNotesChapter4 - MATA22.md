\title{
Second degree curves
}

\section{Ellipse, Hyperbola, Parabola}

In this chapter we consider second-degree curves as geometrical objects whose equations can be derived by using some of the tools developed in the previous chapter.

Circle. A circle $\mathcal{C}$ in a plane $\pi$, centred at a point $F$ and of radius $a>0$ can be defined as the set of all points $P$ in $\pi$ lying at given distance $a$ to $F$. If $F$ and $P$ have coordinates $\left(x_{0}, y_{0}\right)$ and $(x, y)$ respectively, where coordinates are represented in some ON-system for $\pi$, then the equation of the circle $\mathcal{C}$ can be written

$$
\left(x-x_{0}\right)^{2}+\left(y-y_{0}\right)^{2}=a^{2} .
$$

If $F$ is the origin, the equation reduces to

$$
x^{2}+y^{2}=a^{2} .
$$

We shall now discuss the other basic types of second degree curves: ellipse, hyperbola, and parabola.

Ellipse. The definition of an ellipse generalises the definition of a circle. Let $F_{1}$ and $F_{2}$ be two points in a plane $\pi$ and let $a$ be a positive constant; we assume that $2 a$ is greater than the distance between $F_{1}$ and $F_{2}$. The set of points $P$ in $\pi$ with the property that the sum of the distances from $P$ to $F_{1}$ and from $P$ to $F_{2}$ equals to $2 a$ is called an ellipse.

![](https://cdn.mathpix.com/cropped/2022_12_13_d79b7efdae9e82f8066bg-01.jpg?height=421&width=526&top_left_y=1882&top_left_x=759)

If we choose an ON-system in $\pi$ such that the origin is the mid-point on the segment $F_{1} F_{2}$, and the $x$-axis passes through the points $F_{1}$ and $F_{2}$, then $F_{1}$ and $F_{2}$ have coordinates $(-c, 0)$ and $(c, 0)$ for some real $c$. We can assume that $c>0$.

The fact that the sum of distances from $P=(x, y)$ to $F_{1}$ and $F_{2}$ equals $2 a$ can be written as

$$
\sqrt{(x+c)^{2}+y^{2}}+\sqrt{(x-c)^{2}+y^{2}}=2 a .
$$

Squaring the equation (1) leads to

$$
(x+c)^{2}+(x-c)^{2}+2 y^{2}+2 \sqrt{\left((x+c)^{2}+y^{2}\right)\left((x-c)^{2}+y^{2}\right)}=4 a^{2} .
$$

Dividing by 2 and rearranging, this becomes

$$
x^{2}+y^{2}+c^{2}-2 a^{2}=-\sqrt{\left(x^{2}+y^{2}+c^{2}+2 c x\right)\left(x^{2}+y^{2}+c^{2}-2 c x\right)} .
$$

Squaring again, we obtain that

$$
\left(x^{2}+y^{2}+c^{2}\right)^{2}-4 a^{2}\left(x^{2}+y^{2}+c^{2}\right)+4 a^{4}=\left(x^{2}+y^{2}+c^{2}\right)^{2}-4 c^{2} x^{2},
$$

i.e.,

$$
\left(a^{2}-c^{2}\right) x^{2}+a^{2} y^{2}=a^{2}\left(a^{2}-c^{2}\right) .
$$

If we put $b^{2}=a^{2}-c^{2}$ and divide with $a^{2} b^{2}$, this becomes

$$
\frac{x^{2}}{a^{2}}+\frac{y^{2}}{b^{2}}=1 .
$$

We have shown that each point $(x, y)$ satisfying the root-equation (1) also satisfies (2). By tracing back in the calculations, one can also verify that all solutions of (2) satisfy (1). (Since we have squared several times, this is not immediate!) We have shown that the ellipse is completely determined by the equation (2).

Notice that the ellipse (2) intersects the coordinate axes at the points $(\pm a, 0)$ and $(0, \pm b)$. The segments from the origin to these points are called the semi-axes of the ellipse. The points $F_{1}=(-c, 0)$ and $F_{2}=(c, 0)$ are the foci of the ellipse.

Hyperbola. If we instead consider the set of points $P$ in a plane $\pi$ such that the difference between the distances to two given points ("foci") $F_{1}$ and $F_{2}$ is constant $=2 a$, we get a curve known as a hyperbola. In a similar way to the case of the ellipse, we can introduce an ON-system in $\pi$ such that $F_{1}=(-c, 0)$ and $F_{2}=(c, 0)$ for a number $c>a$. Hence the equation of the hyperbola becomes

$$
\sqrt{(x+c)^{2}+y^{2}}-\sqrt{(x-c)^{2}+y^{2}}=\pm 2 a \text {. }
$$

Here the plus-sign shall be chosen if $P=(x, y)$ is closer to $F_{2}$, and the minus-sign if $P$ is closer to $F_{1}$. The hyperbola is not connected, it has two branches. 

![](https://cdn.mathpix.com/cropped/2022_12_13_d79b7efdae9e82f8066bg-03.jpg?height=420&width=529&top_left_y=310&top_left_x=760)

Calculations analogous to the case for the ellipse show that the equation of the hyperbola can be written

$$
\frac{x^{2}}{a^{2}}-\frac{y^{2}}{b^{2}}=1,
$$

where this time $b^{2}=c^{2}-a^{2}$.

Parabola. Let $\ell$ be a line in a plane $\pi$, and $F$ a point in $\pi$, which is not on $\ell$. The set of points $P$ in $\pi$ whose distance to $\ell$ equals the distance to $F$ is called a parabola. The point $F$ is the focus and the line $\ell$ is called the directrix of the parabola. Choose an ON-system in $\pi$ such that the $y$-axis is parallel to $\ell$, the $x$-axis

![](https://cdn.mathpix.com/cropped/2022_12_13_d79b7efdae9e82f8066bg-03.jpg?height=423&width=526&top_left_y=1282&top_left_x=759)

passes through $F$, and the origin has equal distance $a$ to $F$ and to $\ell$. We shall prove that the equation of the parabola in this ON-system becomes

$$
y^{2}=4 a x \text {. }
$$

To show this, note that the distance from a point $P=(x, y)$ to $\ell$ is $x+a$, while the distance to $F$ is $\sqrt{(x-a)^{2}+y^{2}}$. Squaring these distances leads to (5).

REMARK 1 . The parabola has an interesting optical property with many practical applications. Each light-ray parallel to the positive $x$-axis will, after reflection in the parabola, pass through the same point $F$. A set of parallel light-rays are thus focused to the point $F$. Conversely, if we place a source of light at $F$, this will after reflection give rise to light-rays which are parallel to the $x$-axis. In the case of the ellipse, one has instead that if a light source is placed at $F_{1}$, then all light-rays will pass through $F_{2}$.

Remark 2. The ellipse, the hyperbola, and the parabola are all cases of socalled conic sections. This name stems from the fact that all such curves can be obtained as the intersection of a double cone with a suitable plane.

REMARK 3. A natural generalisation of second-degree curves in a plane are second-degree surfaces in the three-dimensional space, such as spheres, ellipsoids, hyperboloids, cones and paraboloids. Second-degree surfaces will be studied in your next course in Linear Algebra using quadratic forms. However, the equation of a sphere can be derived using the same tools used above to express equations of second-degree curves and we shall introduce it below.

Sphere. A sphere $\mathcal{S}$ centered at a given point $F$ and of radius $a$ is the set of all points $P$ in the 3-dimensional space, whose distance to $F$ equals $a \in \mathbb{R}^{+}$, i.e.,

$$
\mathcal{S}=\left\{P \in \mathbb{R}^{3},\|\overline{F P}\|=a\right\} .
$$

If $F=\left(x_{0}, y_{0}, z_{0}\right)$ and $P=(x, y, z)$ in a given $\mathrm{ON}$-system for the 3-dimensional space, then we can write $\|\overline{F P}\|=a$ as

$$
\left(x-x_{0}\right)^{2}+\left(y-y_{0}\right)^{2}+\left(z-z_{0}\right)^{2}=a^{2} .
$$

We conclude this section with a couple of examples.

\section{Example 1.}

The plane $\pi: 2 x-2 y+z=-1$ intersects the sphere $(x+3)^{2}+(y-1)^{2}+(z+2)^{2}=25$ along a circle $C$. Suppose that we want to determine the centre $P$ and the radius $r$ of the intersection circle.

Note that the given sphere is centred at the point $(-3,1,-2)$, call it $Q$, and has radius 5. Then the centre $P$ of the intersection circle is the orthogonal projection of the centre of the sphere onto the plane $\pi$. Consider the line $\ell$ through $Q$ and orthogonal to the plane $\pi$, that is

$$
\ell:\left\{\begin{array}{l}
x=-3+2 t \\
y=1-2 t \\
z=-2+t
\end{array} \quad t \in \mathbb{R} .\right.
$$

Then $P$ is the intersection point between $\ell$ and the plane $\pi$ and it is given by

$$
2(-3+2 t)-2(1-2 t)+(-2+t)=-1 \Longleftrightarrow 9 t=9 \Longleftrightarrow t=1 .
$$

For this value of $t$ we get $P=(-1,-1,-1)$.

![](https://cdn.mathpix.com/cropped/2022_12_13_d79b7efdae9e82f8066bg-05.jpg?height=699&width=716&top_left_y=393&top_left_x=672)

To determine the radius $r$ of the circle let $R$ be an arbitrary point on the circle. Then the triangle $\triangle P Q R$ has a right angle at $P$ and by Pythagora's theorem we have that

$$
\|\overline{Q P}\|^{2}+\|\overline{P R}\|^{2}=\|\overline{Q R}\|^{2} \Longleftrightarrow r^{2}+\|\overline{Q P}\|^{2}=25 .
$$

We have that

$$
\|\overline{Q P}\|=\|(2,-2,1)\|=\sqrt{9}=3 .
$$

Thus $r^{2}=25-3^{2}=16$ and hence $r=4$.

\section{Example 2.}

A ray of light emerging from the point $A=(1,0,1)$ in the direction of the vector $(-1,-1,-1)$ hits a spherical mirror centred at the origin and of radius 1 at the point $P$. Suppose that we are interested to determine a parametric equation of the reflected ray as well as the coordinates of the point $P$. (Positive ON-system)

Let $\ell$ be the line through $A=(1,0,1)$ with direction of the vector $(-1,-1,-1)$, that is $\ell:(x, y, z)=(1-t,-t, 1-t), t \in \mathbb{R}$. The point $P$ where the ray of light hits the given sphere $x^{2}+y^{2}+z^{2}=1$ is one of the two intersection points between $\ell$ and the sphere, that lies closest to the point $A$. The intersection points are given by:

$$
(1-t)^{2}+(-t)^{2}+(1-t)^{2}=1 \Longleftrightarrow 3 t^{3}-4 t-1=0 \Longleftrightarrow t=\frac{1}{3} \text { or } t=1 .
$$

Clearly, $t=\frac{1}{3}$ gives the coordinates of the intersection point $P$ closest to $A$, that 

![](https://cdn.mathpix.com/cropped/2022_12_13_d79b7efdae9e82f8066bg-06.jpg?height=710&width=922&top_left_y=309&top_left_x=561)

is, $P=\frac{1}{3}(2,-1,2)$.

To determine a parametric equation of the reflected ray, we need to determine another point on this line. Note that the reflected line $\ell_{r}$ is symmetric to $\ell$ with respect to the normal line of the plane $\pi$ tangent to the sphere at the point $P$. The point $A^{\prime \prime}$ that is the reflection of $A$ with respect to the plane $\pi$ lies on $\ell_{r}$. To determine its coordinates, we determine first the orthogonal projection $A^{\prime}$ of the point $A$ on the plane $\pi$. The point $A^{\prime}$ is the intersection between $\pi$ and the line $\ell_{n}$ through $A$ orthogonal to $\pi$.

Using that the directed segment $\overline{O P}=\frac{1}{3}(2,-1,2)$ is orthogonal to $\pi$ and $P \in \pi$, we write the corresponding point-normal equation of $\pi$ :

$$
2 x-y+2 z=3 .
$$

A parametric equation of the line $\ell_{n}$ is given by $(x, y, z)=(1,0,1)+(2,-1,2) t, t \in \mathbb{R}$ and the intersection point $A^{\prime}=\ell_{n} \cap \pi$ is obtained from:

$$
2(1+2 t)-(-t)+2(1+2 t)=3 \Longleftrightarrow 9 t=-1 \Longleftrightarrow t=-\frac{1}{9} .
$$

The point $A^{\prime \prime} \in \ell_{n}$ corresponds to $t=-\frac{2}{9}$, that is $A^{\prime \prime}=\frac{1}{9}(5,2,5)$. Then, the vector associated to the directed segment

$$
\overline{A^{\prime \prime} P}=\frac{1}{3}(2,-1,2)-\frac{1}{9}(5,2,5)=\frac{1}{9}(1,-5,1)
$$

is a direction vector of $\ell_{r}$. We can now write a parametric equation of $\ell_{r}$ :

$$
(x, y, z)=\frac{1}{3}(2,-1,2)+t(1,-5,1), t \in \mathbb{R} .
$$

$(x, y, z)=\frac{1}{3}(2,-1,2)+t(1,-5,1), t \in \mathbb{R}$.

\section{Exercises.}

1. Determine the centres of circles which are tangent to the $x$-axis and which pass through the points $(0,1)$ and $(0,9)$.

2. Determine the foci of the ellipses
a) $9 x^{2}+25 y^{2}=225$.
b) $25 x^{2}+169 y^{2}=4225$.

3. Determine the equation of the ellipse which intersects the $y$-axis at the points $(0, \pm 2)$ and has foci at the points $(\pm 2,0)$.

4. Let $\left(x_{0}, y_{0}\right)$ be a point on the ellipse $x^{2} / a^{2}+y^{2} / b^{2}=1$.

a) Show that the line $x=x_{0}+\alpha t, y=y_{0}+\beta t$ is tangent to the ellipse if and only if $\alpha x_{0} / a^{2}+\beta y_{0} / b^{2}=0$.

b) Show that the point $(x, y)$ is on the tangent of the ellipse at $\left(x_{0}, y_{0}\right)$ if and only if $x x_{0} / a^{2}+y y_{0} / b^{2}=1$.

5. Find the foci of the hyperbolae
a) $16 x^{2}-9 y^{2}=144$.
b) $3 x^{2}-5 y^{2}=75$.

6. Find the equation of the hyperbola which intersects the $x$-axis at the points $(\pm 2,0)$ and has foci at $(\pm 3,0)$.

7. Find the equation of the parabola which is symmetric with respect to the $x$ axis and which passes through the points $(0,0)$ and $(27,18)$. Also determine the focus.

8. The sphere of radius 5 centred at the point $(-3,1,-2)$ intersects the plane $\pi: 2 x-2 y+z=-1$ along a circle $C$. Does the intersection point between the plane $\pi$ and the line $\ell(x, y, z)=(2+t, 2+2 t, 2+4 t), t \in \mathbb{R}$ lie inside this circle? (ON-system assumed.)

9. Let $M$ be the plane $2 x+y+2 z=27, S$ the sphere of radius 15 centred at the origin and let $C$ be the circle of intersection between $M$ and $S$. Determine the points in $M, S$ and $C$ that lie closest to the point $(33,30,6)$. (ON-system assumed.) 

\section{General Second-Degree Equations}

A second-degree equation in the variables $x$ and $y$ is an equation of the form

$$
A x^{2}+B x y+C y^{2}+D x+E y=F .
$$

Now suppose that $x$ and $y$ are coordinates with respect to an $\mathrm{ON}$-system $O \mathbf{e}_{1} \mathbf{e}_{2}$ in the plane. We shall investigate the geometric meaning of the equation (1). In the preceding section, we saw that ellipses, hyperbolae, and parabolae are all described by second-degree equations. We shall here show that, except for certain "pathological" cases, these three basic types of curves can be used to describe all second-degree curves.

If $A=B=C=0$, then (1) is a first-degree equation

$$
D x+E y=F .
$$

This is (unless $D=E=0$ ) the equation for a line. In the sequel, we can hence assume that at least one of the coefficients $A, B, C$ are non-zero.

The main idea for our solution of (1) involves changing coordinates to a new ONsystem, where the equation has a simpler form. We start by showing that, by a suitable rotation of the basis vectors, we can get rid of the coefficient $B$ for $x y$. Thus we introduce new basis vectors $\mathbf{e}_{1}^{\prime}, \mathbf{e}_{2}^{\prime}$ by

$$
\begin{aligned}
& \mathbf{e}_{1}^{\prime}=\cos \theta \mathbf{e}_{1}+\sin \theta \mathbf{e}_{2}, \\
& \mathbf{e}_{2}^{\prime}=-\sin \theta \mathbf{e}_{1}+\cos \theta \mathbf{e}_{2} .
\end{aligned}
$$

It is easy to see that $\mathbf{e}_{1}^{\prime}$, $\mathbf{e}_{2}^{\prime}$ is an orthonormal basis (since $\mathbf{e}_{1}, \mathbf{e}_{2}$ is so).

Let $\left(x^{\prime}, y^{\prime}\right)$ be the coordinates for a point $P$ relative to the system $O \mathbf{e}_{1}^{\prime} \mathbf{e}_{2}^{\prime}$. Then

$$
\overrightarrow{O P}=\left(x^{\prime} \cos \theta-y^{\prime} \sin \theta\right) \mathbf{e}_{1}+\left(x^{\prime} \sin \theta+y^{\prime} \cos \theta\right) \mathbf{e}_{2}
$$

If $(x, y)$ are the coordinates of $P$ in the "old" system $O \mathbf{e}_{1} \mathbf{e}_{2}$, we hence have

$$
\begin{aligned}
& x=x^{\prime} \cos \theta-y^{\prime} \sin \theta . \\
& y=x^{\prime} \sin \theta+y^{\prime} \cos \theta .
\end{aligned}
$$

Substituting these expressions into (1), we get an equation of the form

$$
A^{\prime}\left(x^{\prime}\right)^{2}+B^{\prime} x^{\prime} y^{\prime}+C^{\prime}\left(y^{\prime}\right)^{2}+D^{\prime} x^{\prime}+E^{\prime} y^{\prime}=F,
$$

where the coefficient $B^{\prime}$ for $x^{\prime} y^{\prime}$ is given by

$$
\begin{aligned}
B^{\prime} & =-2 A \cos \theta \sin \theta+B\left(\cos ^{2} \theta-\sin ^{2} \theta\right)+2 C \cos \theta \sin \theta \\
& =B \cos 2 \theta-(A-C) \sin 2 \theta,
\end{aligned}
$$

where we have used the familiar "double angle" formulae for cos and sin. If $B=0$ no rotation is necessary, and we can take $\theta=0$. If $B \neq 0$ we choose $\theta$ such that

$$
\cot 2 \theta=\frac{A-C}{B} .
$$

The relation (2) then shows that $B^{\prime}=0$. In all cases, our new coordinate system turns our equation into the type

$$
A^{\prime}\left(x^{\prime}\right)^{2}+C^{\prime}\left(y^{\prime}\right)^{2}+D^{\prime} x^{\prime}+E^{\prime} y^{\prime}=F,
$$

for suitable constants $A^{\prime}, C^{\prime}, D^{\prime}, E^{\prime}$. Since we have assumed that at least one of the numbers $A, B, C$ are not zero, it is easy to see that at least one of $A^{\prime}, C^{\prime}$ are not zero.

Case 1. We first consider the case when both $A^{\prime}$ and $C^{\prime}$ are non-zero. We can then complete squares in (3) to obtain

$$
A^{\prime}\left(x^{\prime}+\frac{D^{\prime}}{2 A^{\prime}}\right)^{2}+C^{\prime}\left(y^{\prime}+\frac{E^{\prime}}{2 C^{\prime}}\right)^{2}=\frac{\left(D^{\prime}\right)^{2}}{4 A^{\prime}}+\frac{\left(E^{\prime}\right)^{2}}{4 C^{\prime}}+F .
$$

We then make a new change of coordinates by

$$
x^{\prime \prime}=x^{\prime}+\frac{D^{\prime}}{2 A^{\prime}} \quad, \quad y^{\prime \prime}=y^{\prime}+\frac{E^{\prime}}{2 C^{\prime}} .
$$

This means that the origin in the old system is moved to the point which has $x^{\prime} y^{\prime}$-coordinates $\left(-D^{\prime} / 2 A^{\prime},-E^{\prime} / 2 C^{\prime}\right)$. If

$$
F^{\prime}=\frac{\left(D^{\prime}\right)^{2}}{4 A^{\prime}}+\frac{\left(E^{\prime}\right)^{2}}{4 C^{\prime}}+F,
$$

then (4) becomes

$$
A^{\prime}\left(x^{\prime \prime}\right)^{2}+C^{\prime}\left(y^{\prime \prime}\right)^{2}=F^{\prime} .
$$

If $A^{\prime}$ and $C^{\prime}$ are both positive, then (5) describes an ellipse, a point, or the empty set, depending on whether $F^{\prime}>0, F^{\prime}=0$, or $F^{\prime}<0$. The case then $A^{\prime}$ and $C^{\prime}$ are both negative can be reduced to the positive case by multiplying both sides of the equation by $-1$. If $A^{\prime}$ and $C^{\prime}$ have opposite signs, we can after multiplication with a suitable constant assume that $A^{\prime}>0$ and $C^{\prime}=-1$. The equation (5) is then

$$
A^{\prime}\left(x^{\prime \prime}\right)^{2}-\left(y^{\prime \prime}\right)^{2}=F^{\prime} .
$$

If $F^{\prime \prime} \neq 0$ this means a hyperbola. If $F^{\prime}=0$ we get

$$
y^{\prime \prime}=\pm \sqrt{A^{\prime}} \cdot x^{\prime \prime},
$$

which means a "degenerate hyperbola", or rather: two intersecting straight lines. Case 2. Now suppose that one of the numbers $A^{\prime}, C^{\prime}$ in (3) are zero. We can w.l.o.g. assume that $A^{\prime}=0$ and $C^{\prime} \neq 0$. Then (3) says that

$$
C^{\prime}\left(y^{\prime}\right)^{2}+D^{\prime} x^{\prime}+E^{\prime} y^{\prime}=F .
$$

If $D^{\prime}=0$, then the equation (6) becomes independent of $x^{\prime}$. The equation then means two lines parallel to the $x^{\prime}$-axis, or one line parallel to the $x^{\prime}$-axis, or the empty set, depending on the number of different real solutions of the second-degree equation $C^{\prime}\left(y^{\prime}\right)^{2}+E^{\prime} y^{\prime}=F$. If $D^{\prime} \neq 0$, the equation (6) can be written

$$
C^{\prime}\left(y^{\prime}+\frac{E^{\prime}}{2 C^{\prime}}\right)^{2}+D^{\prime}\left(x^{\prime}-\frac{F}{D^{\prime}}-\frac{\left(E^{\prime}\right)^{2}}{4 C^{\prime} D^{\prime}}\right)=0 .
$$

If we now put

$$
x^{\prime \prime}=x^{\prime}-\frac{F}{D^{\prime}}-\frac{\left(E^{\prime}\right)^{2}}{4 C^{\prime} D^{\prime}} \quad, \quad y^{\prime \prime}=y^{\prime}+\frac{E^{\prime}}{2 C^{\prime}} 4 C^{\prime} D^{\prime},
$$

we see that (6) transforms into the equation

$$
C^{\prime}\left(y^{\prime \prime}\right)^{2}+D^{\prime} x^{\prime \prime}=0 .
$$

This last equation means a parabola: if $C^{\prime}$ and $D^{\prime}$ have equal signs, it surrounds the negative $x^{\prime \prime}$-axis, otherwise it surrounds the positive $x^{\prime \prime}$-axis.

The above discussion characterises all possible second-degree curves. Except for ellipse, hyperbola, and parabola, there are the following "pathological" cases: two intersecting straight lines, one or two parallel straight lines, a point, the whole plane (when $A=B=C=D=E=F=0$ ), and the empty set.

\section{Exercises.}

8. Prove that each of the following equations describes an ellipse. Also determine the lengths of the semi-axes.

a) $17 x^{2}-16 x y+17 y^{2}=225$.

b) $3 x^{2}+2 x y+3 y^{2}=8$

c) $9 x^{2}+y^{2}-18 x+4 y+4=0$

d) $2 x^{2}+3 y^{2}+12 x+12=0$.

\section{Answers to exercises}

1. $(\pm 3,5)$.

2. a) $(\pm 4,0)$. b) $(\pm 12,0)$.

3. $x^{2}+2 y^{2}=8$.

5. a) $(\pm 5,0)$. b) $(\pm \sqrt{40}, 0)$.

6. $5 x^{2}-4 y^{2}=20$.

7. $y^{2}=12 x$; focus $(3,0)$. 8. Yes.

9. $(15,21,-12),(11,10,2)$ and $(10,11,-2)$.

10. a) 5 and 3. b) 2 and $\sqrt{2}$. c) 3 and 1. d) $\sqrt{3}$ and $\sqrt{2}$.