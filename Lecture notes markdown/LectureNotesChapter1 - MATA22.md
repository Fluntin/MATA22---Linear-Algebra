\title{
Lecture Notes for Linear Algebra 1
}

8 September 2019 

\section{CHAPTER 1}

\section{Linear Systems of Equations}

\section{Introduction}

A linear equation in the variables (or unknowns) $x_{1}, \ldots, x_{n}$ is a statement of the form

$$
a_{1} x_{1}+a_{2} x_{2}+\cdots+a_{n} x_{n}=b .
$$

Here $a_{1}, \ldots, a_{n}$ and $b$ are constants which are usually known. By a solution of (1) we mean a set of values of $x_{1}, x_{2}, \ldots, x_{n}$ which makes the statement true.

The linear equation (1) is called homogeneous if $b=0$; otherwise it is nonhomogeneous.

A linear system of equations consists of a number of linear equations that are simultaneously fulfilled by the variables $x_{1}, x_{2}, \ldots, x_{n}$ :

$$
\left\{\begin{array}{c}
a_{11} x_{1}+a_{12} x_{2}+\ldots+a_{1 n} x_{n}=y_{1} \\
a_{21} x_{1}+a_{22} x_{2}+\ldots+a_{2 n} x_{n}=y_{2} \\
\ldots \\
a_{p 1} x_{1}+a_{p 2} x_{2}+\ldots+a_{p n} x_{n}=y_{p}
\end{array}\right.
$$

This system has $p$ equations and $n$ variables. By a solution of such a system we mean a set of values of the variables such that each of the equations in the system are fulfilled. The double indexed constants $a_{i j}, 1 \leq i \leq p, 1 \leq j \leq n$ are called the coefficients of the linear system. In the above notation, the first index indicates the number of the coefficient's corresponding equation in the system, while the second index indicates its corresponding variable. A system is called quadratic if the number of equations is equal to the number of variables. A system is called homogeneous if all its equations are homogeneous.

Example. (a) The system

$$
\left\{\begin{array}{r}
x+2 y=5 \\
-2 x+3 y=4
\end{array}\right.
$$

has a solution $(x, y)=(1,2)$. (b) The system

$$
\left\{\begin{array}{r}
x+y+z=1 \\
2 x-y+z=3 \\
3 x+2 z=4
\end{array}\right.
$$

has, for example, the solutions $(x, y, z)=(2,0,-1)$ and $(x, y, z)=(4,1,-4)$. Note that these are not the only solutions of this system.

(c) The system

$$
\left\{\begin{array}{l}
x+y=2 \\
x+y=3
\end{array}\right.
$$

has no solutions, for if there were a solution $(x, y)$, we would have $2=x+y=3$, which is false.

\section{The Gauss-Jordan Elimination Method}

We shall now introduce a general method for solving linear systems of equations. In this method, we shall successively replace a given system of equations by simpler, equivalent systems. Here, by definition, two systems are equivalent if and only if they have precisely the same solutions. We begin with some examples.

Example 1. Solve the linear system $\left\{\begin{array}{r}x+2 y=5 \\ -2 x+3 y=4\end{array}(*)\right.$.

Solution. The first equation in the system is equivalent to that $x=5-2 y$. We can then eliminate $x$ from the second equation by replacing it with $5-2 y$. The system $(*)$ is thus equivalent to

$$
\begin{array}{r}
\left\{\begin{array}{r}
x+2 y=5 \\
-2(5-2 y)+3 y=4
\end{array}\right. \\
\Leftrightarrow \quad\left\{\begin{array}{r}
x+2 y=5 \\
7 y=14
\end{array}\right. \\
\Leftrightarrow \quad\left\{\begin{array}{r}
x+2 y=5 \\
y=2
\end{array}\right.
\end{array}
$$

The second equation in the last system says that $y=2$. We can then eliminate $y$ from the first equation by substituting this value for $y$, so that (3) is equivalent to

$$
\left\{\begin{array} { r } 
{ x + 2 \cdot 2 = 5 } \\
{ y = 2 }
\end{array} \Leftrightarrow \left\{\begin{array}{l}
x=1 \\
y=2
\end{array}\right.\right.
$$

It follows that the system has the unique solution $(x, y)=(1,2)$. The elimination we performed to obtain $(2)$ from $(*)$ can be recognised as the following operation: the first equation in $\left(^{*}\right)$ is multiplied by 2 , and is then added to the second equation. The coefficient of $x$ in the resulting sum of equations is then zero, i.e. the variable $x$ is eliminated there:

$$
\begin{aligned}
& \left\{\begin{array}{c}
x+2 y=5 \quad \times 2, \text { add to second eq. } \\
-2 x+3 y=4
\end{array}\right. \\
& \Leftrightarrow\left\{\begin{array}{cc}
x+ & 2 y=5 \\
0 \cdot x+(2 \cdot 2+3) y=2 \cdot 5+4
\end{array}\right. \\
& \Leftrightarrow\left\{\begin{array}{c}
x+2 y=5 \\
7 y=14
\end{array}\right.
\end{aligned}
$$

The elimination of $y$ from the first equation has a similar interpretation: the second equation in (3) is multiplied by $-2$ and added to the first,

$$
\begin{aligned}
& \left\{\begin{array}{c}
x+2 y=5 \\
y=2 \quad \times(-2), \text { add to first eq. }
\end{array}\right. \\
& \left\{\begin{array}{c}
x+0 \cdot y=5-2 \cdot 2 \\
y=2
\end{array}\right.
\end{aligned}
$$

The indicated operation is the main ingredient in the Gauss-Jordan elimination method. We shall execute this operation repeatedly, in a systematic way.

Example 2. Solve the linear system

$$
\left\{\begin{array}{r}
x+4 y-2 z=8 \\
2 x+9 y+z=7 . \\
3 x-2 y-4 z=6
\end{array}\right.
$$

Solution. We first use the first equation to eliminate $x$ from the other equations. From the second equation we subtract 2.(first eq.) and from the third we subtract 3.(first eq.). The system becomes

$$
\left\{\begin{array}{rl}
x+4 y-2 z & =8 \\
y+5 z & =-9 \\
-14 y+2 z & =-18
\end{array} .\right.
$$

To simplify, we here divide the third equation by 2 ,

$$
\left\{\begin{aligned}
x+4 y-2 z & =8 \\
y+5 z & =-9 . \\
-7 y+z & =-9
\end{aligned}\right.
$$

We now eliminate $y$ from the third equation by adding $7 \cdot($ second eq.):

$$
\left\{\begin{array} { r l } 
{ x + 4 y - 2 z } & { = 8 } \\
{ y + 5 z } & { = - 9 } \\
{ 3 6 z } & { = - 7 2 }
\end{array} \Leftrightarrow \quad \left\{\begin{array}{rl}
x+4 y-2 z & =8 \\
y+5 z & =-9 . \\
z & =-2
\end{array}\right.\right.
$$

Using the third equation, we eliminate $z$ from the first two ones:

$$
\left\{\begin{array}{rl}
x+4 y & =4 \\
y & =1 \\
z & =-2
\end{array} .\right.
$$

Finally, $y$ is eliminated from the first equation using the second one:

$$
\left\{\begin{array}{rl}
x & =0 \\
y & =1 \\
z & =-2
\end{array} .\right.
$$

The system has the unique solution $(x, y, z)=(0,1,-2)$.

Here is the main principle. The first equation is used to eliminate the first unknown from the other equations. Then the (new) second equation is used to eliminate the second unknown from the subsequent equations, etc. The last equation will only contain the last unknown, which has thus been calculated. After that we make a backwards substitution to eliminate the variables "upwards", one at a time, until the system is completely solved.

The simple rule above can not always be carried out. We illustrate with a couple of simple examples.

Example 3. In the system

$$
\left\{\begin{aligned}
y-2 z & =3 \\
x+2 y-z & =2 \\
2 x+3 y+z & =-1
\end{aligned}\right.
$$

we can't as earlier use the first equation to eliminate $x$ from the other ones. On the other hand, the second equation can be used. To obtain a system of the same form as earlier, we switch places of the first two equations:

$$
\left\{\begin{aligned}
x+2 y-z & =2 \\
y-2 z & =3 \\
2 x+3 y+z & =-1
\end{aligned}\right.
$$

After this we can proceed as before. Do this! (The system has the unique solution $(x, y, z)=(2,-1,-2)$. Example 4. Solve the system $\left\{\begin{array}{l}3 x+2 y=4 \\ 6 x+4 y=1\end{array}\right.$.

Solution. We eliminate $x$ from the second equation by subtracting 2.(first eq.) and get

$$
\left\{\begin{aligned}
3 x+2 y & =4 \\
0 & =-7
\end{aligned}\right.
$$

The second equation is a false statement for all values of the variables $x$ and $y$. This means that the system has no solutions.

Example 5. Solve the system $\left\{\begin{array}{l}3 x+2 y=4 \\ 6 x+4 y=8\end{array}\right.$.

Solution. Eliminating $x$ from the second equation, we now get

$$
\left\{\begin{aligned}
3 x+2 y & =4 \\
0 & =0
\end{aligned}\right.
$$

The second equation is always satisfied, so the system is equivalent to the single equation $3 x+2 y=4$. This means that we can let $y$ have an arbitrary value, say $y=t$, and then $x$ is uniquely determined by $y$. Hence the system has infinitely many solutions

$$
\left\{\begin{array}{l}
x=\frac{4}{3}-\frac{2}{3} t \\
y=t
\end{array}, \quad t \in \mathbb{R} .\right.
$$

\section{Exercises.}

1. Solve the following linear systems of equations:
a) $\left\{\begin{array}{r}x+y=2 \\ -x+y=4\end{array}\right.$
b) $\left\{\begin{array}{l}2 x-3 y=1 \\ 6 x+y=7\end{array}\right.$
c) $\left\{\begin{array}{l}4 x+3 y=2 \\ 3 x-5 y=6\end{array}\right.$.

2. Solve the following systems:
a) $\left\{\begin{array}{r}x-y+z=4 \\ 3 x+5 y-z=0 \\ 2 x-y-3 z=2\end{array}\right.$
b) $\left\{\begin{array}{l}2 x-y+3 z=9 \\ 3 x+2 y-2 z=1 \\ 4 x+5 y-4 z=2\end{array}\right.$
c) $\left\{\begin{aligned} y+z & =-2 \\ x-2 y+z & =-2 \\ 2 x-5 y+3 z & =-2\end{aligned}\right.$
d) $\left\{\begin{aligned} x+y & =8 \\ x+z & =6 \\ y+z & =4\end{aligned}\right.$. 3. Solve the following systems:
a) $\left\{\begin{array}{l}2 x-\frac{1}{3} y=2 \\ 6 x-y=4\end{array}\right.$
b) $\left\{\begin{array}{c}4 x-3 y=4 \\ -3 x+\frac{9}{4} y=-3\end{array}\right.$
c) $\left\{\begin{array}{l}6 x+9 y=5 \\ 9 x+3 y=\frac{15}{2}\end{array}\right.$.

\section{The Augmented Matrix of a Linear System of Equations}

The numerical operations used when solving a linear system involve solely the coefficients of the unknowns and the constants in the right hand sides. To simplify the notation, one can omit the unknown and represent the system by a scheme called the augmented matrix of the system. For example, the system

$$
\left\{\begin{aligned}
x+2 y+3 z & =10 \\
x+y-z & =4 \\
2 x-y+z & =5
\end{aligned} \quad \text { is represented by } \quad\left[\begin{array}{ccc|c}
1 & 2 & 3 & 10 \\
1 & 1 & -1 & 4 \\
2 & -1 & 1 & 5
\end{array}\right]\right. \text {. }
$$

Example 6 . We solve the system $(*)$ in two ways: by writing down complete equations as before, and, in parallel, by just manipulating the augmented matrix.

Eliminate $x$ from eq.'s 2 and $3 / /$ Row 2 - row 1, row 3 - 2.row 1 .

$$
\left\{\begin{aligned}
x+2 y+3 z & =10 \\
-y-4 z & =-6 \\
-5 y-5 z & =-15
\end{aligned} \quad \sim\left[\begin{array}{ccc|c}
1 & 2 & 3 & 10 \\
0 & -1 & -4 & -6 \\
0 & -5 & -5 & -15
\end{array}\right]\right.
$$

Multiply eq. 2 by ( $-1$ ), eq. 3 by $-\frac{1}{5} / /$ Multiply row 2 by $(-1)$, row 3 by $-\frac{1}{5}$.

$$
\left\{\begin{aligned}
x+2 y+3 z & =10 \\
y+4 z & =6 \\
y+z & =3
\end{aligned} \sim\left[\begin{array}{ccc|c}
1 & 2 & 3 & 10 \\
0 & 1 & 4 & 6 \\
0 & 1 & 1 & 3
\end{array}\right]\right.
$$

Eliminate $y$ from eq. $3 / /$ Row 3 - row 2 .

$$
\left\{\begin{aligned}
x+2 y+3 z & =10 \\
y+4 z & =6 \\
-3 z & =-3
\end{aligned} \sim\left[\begin{array}{ccc|c}
1 & 2 & 3 & 10 \\
0 & 1 & 4 & 6 \\
0 & 0 & -3 & -3
\end{array}\right]\right.
$$

Divide eq. 3 by $-3 / /$ Divide row 3 by $-3$.

$$
\left\{\begin{aligned}
x+2 y+3 z & =10 \\
y+4 z & =6 \\
z & =1
\end{aligned} \sim\left[\begin{array}{lll|r}
1 & 2 & 3 & 10 \\
0 & 1 & 4 & 6 \\
0 & 0 & 1 & 1
\end{array}\right]\right.
$$

Eliminate $z$ in eq.'s 1 and $2 / /$ Row $1-3 \cdot$ row 3 , row $2-4$.row 3.

$$
\left\{\begin{aligned}
& x+2 y=7 \\
& y=2 \\
& z=1
\end{aligned} \quad \sim\left[\begin{array}{lll|r}
1 & 2 & 0 & 7 \\
0 & 1 & 0 & 2 \\
0 & 0 & 1 & 1
\end{array}\right]\right.
$$

Eliminate $y$ in eq. $1 / /$ Row $1-2$.row 2 .

![](https://cdn.mathpix.com/cropped/2022_12_13_d5177f55811f50cd70abg-09.jpg?height=186&width=700&top_left_y=1105&top_left_x=669)

The system thus has the unique solution $(x, y, z)=(3,2,1)$.

The admissible operations on the augmented matrix, i.e. those giving rise to an equivalent augmented matrix, are the following:

(i) A row is multiplied by a constant $\neq 0$.

(ii) A constant multiple of a row is added to another row.

(iii) Two rows are interchanged.

(iv) Two columns can be interchanged if one observes that this means that two unknowns are interchanged. This must be taken into account when interpreting the answer.

The operation (iv) is not really needed - one can always circumvent it by other means. Here is an example of this.

Example 7. Solve the system

$$
\left\{\begin{aligned}
x+2 y-3 z+w & =-2 \\
3 x+6 y+3 z-w & =-2 \\
2 x+4 y+3 z+w & =9 \\
2 x+4 y-3 z-w & =-13
\end{aligned}\right.
$$

Solution. The augmented matrix is

$$
\begin{aligned}
& \left[\begin{array}{cccc|c}1 & 2 & -3 & 1 & -2 \\3 & 6 & 3 & -1 & -2 \\2 & 4 & 3 & 1 & 9 \\2 & 4 & -3 & -1 & -13\end{array}\right] \\
& \text { row } 2-3 \cdot \text { row } 1 \\
& \text { row } 3-2 \text {.row } 1 \\
& \text { row } 4-2 \text {.row } 1 \\
& \sim\left[\begin{array}{cccc|c}41 & 2 & -3 & 1 & -2 \\0 & 0 & 12 & -4 & 4 \\0 & 0 & 9 & -1 & 13 \\0 & 0 & 3 & -3 & -9\end{array}\right] \\
& \text { divide row } 2 \text { by } 4 \\
& \text { divide row } 4 \text { by } 3 \\
& \sim\left[\begin{array}{cccc|c}41 & 2 & -3 & 1 & -2 \\0 & 0 & 3 & -1 & 1 \\0 & 0 & 9 & -1 & 13 \\0 & 0 & 1 & -1 & -3\end{array}\right]
\end{aligned}
$$

Here we realise that we can not eliminate the variable in the second column. We therefore skip that column and continue with the third one. Interchange rows 2 and 4 :

$$
\begin{aligned}
& \left[\begin{array}{cccc|c}41 & 2 & -3 & 1 & -2 \\0 & 0 & 1 & -1 & -3 \\0 & 0 & 9 & -1 & 13 \\0 & 0 & 3 & -1 & 1\end{array}\right] \\
& \text { row } 3-9 \text {.row } 2 \\
& \text { row } 4-3 \text {.row } 2 \\
& \sim\left[\begin{array}{cccc|c}41 & 2 & -3 & 1 & -2 \\0 & 0 & 1 & -1 & -3 \\0 & 0 & 0 & 8 & 40 \\0 & 0 & 0 & 2 & 10\end{array}\right] \\
& \text { divide row } 3 \text { by } 8 \\
& \text { divide row } 4 \text { by } 2 \\
& \sim\left[\begin{array}{cccc|c}41 & 2 & -3 & 1 & -2 \\0 & 0 & 1 & -1 & -3 \\0 & 0 & 0 & 1 & 5 \\0 & 0 & 0 & 1 & 5\end{array}\right] \\
& \text { row 1- row } 3 \\
& \text { row } 2+\text { row } 3 \\
& \text { row } 4 \text { is unnecessary - strike it! } \\
& \sim\left[\begin{array}{cccc|c}41 & 2 & -3 & 0 & -7 \\0 & 0 & 1 & 0 & 2 \\0 & 0 & 0 & 1 & 5\end{array}\right] \\
& \text { row } 1+3 \text {.row } 2 \\
& \sim\left[\begin{array}{cccc|c}41 & 2 & 0 & 0 & -1 \\0 & 0 & 1 & 0 & 2 \\0 & 0 & 0 & 1 & 5\end{array}\right] \quad \text { i.e. } \quad\left\{\begin{array}{rl}x+2 y & =-1 \\z & =2 \\w & =5\end{array} .\right. 
\end{aligned}
$$

Here $y$ can have an arbitrary value (say $t$ ), and then the solution is fixed. The solutions are thus

$$
(x, y, z, w)=(-1-2 t, t, 2,5), \quad t \in \mathbb{R} .
$$

We finish this section by discussing the application of the Gauss-Jordan method in a few other slightly complicated cases.

Example 8. Solve the system

$$
\left\{\begin{array}{l}
x-2 y=1 \\
2 x-3 y=4 \\
4 x-7 y=5
\end{array} .\right.
$$

Solution. The augmented matrix is

$$
\begin{aligned}
& {\left[\begin{array}{cc|c}
1 & -2 & 1 \\
2 & -3 & 4 \\
4 & -7 & 5
\end{array}\right] \quad \text { row } 2-2 \cdot \text { row } 1} \\
& \sim\left[\begin{array}{cc|c}
1 & -2 & 1 \\
0 & 1 & 2 \\
0 & 0 & -1
\end{array}\right]
\end{aligned}
$$

The last line represents the equation $0=-1$, which is not satisfied for any values of $x$ and $y$. The given system thus lacks solutions.

Example 9. Solve the system

$$
\left\{\begin{array}{rl}
x-2 y+z & =3 \\
-2 x+4 y-2 z & =-6
\end{array} .\right.
$$

Solution.

$$
\begin{array}{rr} 
& {\left[\begin{array}{ccc|c}
1 & -2 & 1 & 3 \\
-2 & 4 & -2 & -6
\end{array}\right] \quad \text { row } 2+2 \cdot \text { row } 1} \\
\sim\left[\begin{array}{ccc|c}
31 & -2 & 1 & 3 \\
0 & 0 & 0 & 0
\end{array}\right] \quad \text { i.e. } \quad\left\{\begin{array}{r}
x-2 y+z=3 \\
0=0
\end{array}\right.
\end{array}
$$

The last equation is always satisfied - it does not mean any condition on the unknowns $x, y$, and $z$. The given system of equations is therefore equivalent to the single equation $x-2 y+z=3$. Here we can prescribe values for $y$ and $z$ arbitrarily; the variable $x$ is uniquely determined by these values. The general solution can be written

$$
(x, y, z)=(3+2 s-t, s, t), \quad s, t \in \mathbf{R} .
$$

Example 10. Solve the following system for all values of $a$ :

$$
\left\{\begin{array}{l}
x+y-a z=\quad 3 \\
x-a y-z=2 \\
x-3 y-z=2-a
\end{array}\right.
$$

Solution.

$$
\begin{aligned}
& \left[\begin{array}{ccc|c}1 & 1 & -a & 3 \\1 & -a & -1 & 2 \\1 & -3 & -1 & 2-a\end{array}\right] \\
& \text { row } 2 \text { - row } 1 \\
& \text { row } 3 \text { - row } 1 \\
& \sim\left[\begin{array}{ccc|c}1 & 1 & -a & 3 \\0 & -a-1 & a-1 & -1 \\0 & -4 & a-1 & -1-a\end{array}\right] \\
& \text { Divide row } 3 \text { by }-4 \text {, } \\
& \text { then interchange } \\
& \text { row } 2 \text { with row } 3 \text {. } \\
& \sim\left[\begin{array}{ccc|c}1 & 1 & -a & 3 \\0 & 1 & \frac{1}{4}(1-a) & \frac{1}{4}(1+a) \\0 & -a-1 & a-1 & -1\end{array}\right] \\
& \text { row } 3+(a+1) \cdot \text { row } 2 \\
& \sim\left[\begin{array}{ccc|c}1 & 1 & -a & 3 \\0 & 1 & \frac{1}{4}(1-a) & \frac{1}{4}(1+a) \\0 & 0 & \frac{1}{4}(a-1)(3-a) & \frac{1}{4}(a-1)(a+3)\end{array}\right] .
\end{aligned}
$$

The last row is equivalent to the equation

$$
(a-1)(3-a) z=(a-1)(a+3) .
$$

Here we need to divide into cases.

Case 1: $a=1$. Then the equation $\left(^{*}\right)$ reduces to $0=0$, which is always satisfied. The given system is then equivalent to the first two rows in (4), i.e.,

$$
\begin{array}{r}
{\left[\begin{array}{ccc|c}
1 & 1 & -1 & 3 \\
0 & 1 & 0 & \frac{1}{2}
\end{array}\right] \quad \text { row } 1 \text { - row } 2} \\
\sim\left[\begin{array}{ccc|c}
1 & 0 & -1 & \frac{5}{2} \\
0 & 1 & 0 & \frac{1}{2}
\end{array}\right] \quad \text { i.e. } \quad\left\{\begin{array}{c}
x-z=\frac{5}{2} \\
y=\frac{1}{2}
\end{array}\right.
\end{array}
$$

One can e.g. prescribe $z$ arbitrarily and then get $x, y, z$ from the value of $z$,

$$
(x, y, z)=\left(\frac{5}{2}+t, \frac{1}{2}, t\right), \quad t \in \mathbb{R} .
$$

Case 2: $a=3$. In this case, $\left({ }^{*}\right)$ says that $0 \cdot z=2 \cdot 6 \Leftrightarrow 0=12$. This is false, so the system lacks solutions for $a=3$. Case 3: $a \neq 1 \wedge a \neq 3$. In this case, the third row in (4) can be multiplied by $\frac{4}{(a-1)(3-a)}$, which leads to

$$
\begin{aligned}
& {\left[\begin{array}{ccc|c}
1 & 1 & -a & 3 \\
0 & 1 & \frac{1}{4}(1-a) & \frac{1}{4}(1+a) \\
0 & 0 & 1 & \frac{3+a}{3-a}
\end{array}\right] \quad \begin{array}{l}
\text { row } 1+a \cdot \text { row } 3 \\
\text { row } 2+\frac{1}{4}(a-1) \cdot \operatorname{row} 3
\end{array}} \\
& \sim\left[\begin{array}{lll|l}
1 & 1 & 0 & \frac{9+a^{2}}{3-a} \\
0 & 1 & 0 & \frac{a}{3-a} \\
0 & 0 & 1 & \frac{3+a}{3-a}
\end{array}\right] \\
& \sim\left[\begin{array}{lll|l}
1 & 0 & 0 & \frac{a^{2}-a+9}{3-a} \\
0 & 1 & 0 & \frac{a}{3-a} \\
0 & 0 & 1 & \frac{3+a}{3-a}
\end{array}\right]
\end{aligned}
$$

In conclusion, we have arrived at the following result concerning the solutions of the system:

(a) For $a=3$ the system has no solutions.

(b) For $a=1$ it has the solutions $(x, y, z)=\left(\frac{5}{2}+t, \frac{1}{2}, t\right), t \in \mathbb{R}$.

(c) For $a \notin\{1,3\}$ it has the unique solution

$$
(x, y, z)=\left(\frac{a^{2}-a+9}{3-a}, \frac{1}{3-a}, \frac{3+a}{3-a}\right) .
$$

\section{Exercises.}

4. Solve the following systems:
a) $\left\{\begin{array}{l}x-9 y-3 z=4 \\ 3 x-2 y+z=2 \\ 2 x+7 y+4 z=-2\end{array}\right.$
b) $\left\{\begin{array}{l}x-y+z=0 \\ 3 x+5 y-z=0 \\ 6 x+2 y+2 x=5\end{array}\right.$
c) $\left\{\begin{array}{r}2 x+3 y=2 \\ x+3 y-z=5 \\ 3 x+y+z=3\end{array}\right.$
d) $\left\{\begin{aligned} x+2 y & =-3 \\ 2 x-3 y & =8 \\ 10 x-y & =2\end{aligned}\right.$
e) $\left\{\begin{array}{c}x-2 y=6 \\ 3 x+y=2 \\ 5 x-3 y=14\end{array}\right.$
f) $\left\{\begin{array}{l}2 x+y-3 z=4 \\ 4 x+3 y-z=2\end{array}\right.$
g) $\left\{\begin{array}{l}x+y-4 z=7 \\ x+y+2 z=1\end{array}\right.$
h) $\left\{\begin{array}{r}2 x-3 y+4 z=1 \\ 3 x+y-z=7 \\ x-y+5 z=1 \\ 4 x-6 y+8 z=3\end{array}\right.$ i) $\left\{\begin{array}{r}2 x-3 y+4 z=1 \\ 3 x+y-z=7 \\ x-y+5 z=1 \\ 4 x-6 y+8 z=2\end{array} \quad\right.$ j) $\left\{\begin{array}{l}2 x-y+z=3 \\ 4 x-2 y+5 z=0 \\ 2 x-y-2 z=9\end{array}\right.$

k) $\left\{\begin{array}{c}x+3 y+z-w=2 \\ 3 x+5 y-z-w=2 \\ 5 x-y-5 z+3 w=0 \\ 2 x+3 y-3 z-2 w=2\end{array}\right.$

5. Solve the system $\left\{\begin{array}{r}2 x-3 y+z=a \\ x-3 y+2 z=b \\ 3 x+y-4 z=c\end{array}\right.$ when
a) $a=2, b=-3, c=0$;
b) $a=b=c=0$.

Hint: Several linear systems with the same coefficient matrices but different right hand sides can be solved simultaneously with the same augmented matrix: one just writes the different right hand sides next to each other.

6. Determine $a$ and $b$ so that the lines $y-3 x=2$ and $2 y+a x=b$ a) intersect at a point, b) are parallel and different, c) coincide.

7. Determine $a$ and $b$ so that $\frac{2 x+13}{(x-1)(x+2)}=\frac{a}{x-1}+\frac{b}{x+2}$.

(This is an example of a decomposition in partial fractions of a rational function. Such decompositions are frequently used in the calculation of integrals, for example.)

8. Determine for all values of $a$ the number of solutions of the system
a) $\left\{\begin{array}{c}x+2 y=2 \\ 2 x+a y=a\end{array}\right.$
b) $\left\{\begin{array}{c}x+2 y=1 \\ 2 x+a y=a\end{array}\right.$
c) $\left\{\begin{array}{c}x+2 y=1 \\ 2 x+a^{2} y=a\end{array}\right.$.

9. Determine all solutions of the following systems for all values of the constant $a$ :
a) $\left\{\begin{array}{c}x+3 y=4 \\ 2 x+a y=a\end{array}\right.$
b) $\left\{\begin{array}{c}x+3 y=3 \\ 2 x+a y=a\end{array}\right.$
c) $\left\{\begin{aligned} x-3 a y & =2 \\ a x-12 y & =a+2\end{aligned}\right.$ 

$$
\begin{aligned}
& \text { d) }\left\{\begin{array} { c } { x + y = 3 } \\{ 2 x - a y = 2 }\end{array} \text { e) } \left\{\begin{array} { c } { x - 2 a y = 3 } \\{ a x + 3 y = 3 a - 1 }\end{array} \text { f) } \left\{\begin{array}{c}x+y+3 z=1 \\2 x+y+z=2 \\3 x+3 y+a z=0\end{array}\right.\right.\right. \\
& \text { g) }\left\{\begin{array} { r l } { x + y + z } & { = 1 } \\{ 2 x + a y - \quad z } & { = 1 } \\{ a x + 2 y + ( a + 3 ) z } & { = 2 }\end{array} \quad \text { h) } \left\{\begin{array}{rl}x+y+a z & =1 \\x+a y+z & =a \\a x+y+z & =a^{2}\end{array}\right.\right. \text {. }
\end{aligned}
$$

10. Examine, for different values of $a$ and $b$, the number of solutions of the following linear systems of equations:
a) $\left\{\begin{array}{l}a x+2 y=b \\ 3 x+2 y=5\end{array}\right.$
b) $\left\{\begin{aligned} a x+b y & =2 \\ x+y & =1\end{aligned}\right.$.

11. Determine $a, b$, and $c$ so that

$$
\frac{3 x^{2}+6 x-16}{x^{3}-4 x}=\frac{a}{x}+\frac{b}{x+2}+\frac{c}{x-2} .
$$

12. Determine the constants $a, b, c$ so that the function $f(x)=a x^{2}+b x+c$ satisfies $f(1)=-3, f(2)=1$ and $f(-1)=7$.

13. Determine the equation of a third degree polynomial whose graph passes through the points $(0,1),(1,1),(2,1)$, and $(-1,7)$.

\section{Answers to Exercises}

![](https://cdn.mathpix.com/cropped/2022_12_13_d5177f55811f50cd70abg-15.jpg?height=68&width=1196&top_left_y=1533&top_left_x=367)
2. $(x, y, z)=$ a) $(2,-1,1)$
b) $(1,2,3)$
c) $(-6,-2,0)$

d) $(5,3,1)$.

3. a) Has no solution. b) $x=1+\frac{3}{4} y, y \in \mathbb{R}$. c) $(x, y)=\left(\frac{5}{6}, 0\right)$.

4. a) $(x, y, z)=\left(1+\frac{3}{2} t, t,-1-\frac{5}{2} t\right), t \in \mathbb{R}$.

b) No solution.

c) $(x, y, z)=(4,-2,-7)$.

d) No solution exists.

![](https://cdn.mathpix.com/cropped/2022_12_13_d5177f55811f50cd70abg-15.jpg?height=69&width=1109&top_left_y=1841&top_left_x=478)

g) $(x, y, z)=(3-t, t,-1), t \in \mathbb{R} \quad$ h) Has no solution.

![](https://cdn.mathpix.com/cropped/2022_12_13_d5177f55811f50cd70abg-15.jpg?height=63&width=1158&top_left_y=1947&top_left_x=489)

k) $(x, y, z, w)=(2,-1,1,-2)$.

5. a) There is no solution. $\quad$ b) $x=y=z=t, t \in \mathbb{R}$.

$\begin{array}{lll}\text { 6. a) } a \neq-6 & \text { b) } a=-6, b \neq 4 & \text { c) } a=-6, b=4 \text {. }\end{array}$

d) The system of equations has respectively: exactly one solution, no solutions, infinitely many solutions.

7. $a=5, b=-3$. 8. a) If $a=4$ there are infinitely many, otherwise unique.

b) If $a=4$ there is no solution, otherwise unique.

c) If $a=2$ there are infinitely many, if $a=-2$ none, otherwise a unique solution.

9. a) For $a=6$ no solution. For $a \neq 6,(x, y)=\left(\frac{a}{a-6}, \frac{a-8}{a-6}\right)$.

b) For $a=6:(x, y)=(3-3 t, t), t \in \mathbb{R}$. For $a \neq 6:(x, y)=(0,1)$.

c) For $a=-2$, no solution. For $a=2:(x, y)=(2+6 t, t), t \in \mathbb{R}$.

For $a \neq \pm 2:(x, y)=\left(\frac{a+4}{a+2},-\frac{1}{3(a+2)}\right)$.

d) For $a=-2$ : insoluble. For $a \neq-2:(x, y)=\left(\frac{3 a+2}{a+2}, \frac{4}{a+2}\right)$.

e) $(x, y)=\left(\frac{6 a^{2}-2 a+9}{2 a^{2}+3},-\frac{1}{2 a^{2}+3}\right)$.

f) $a=9$ : insoluble. $a \neq 9:(x, y, z)=\left(\frac{a-15}{a-9}, \frac{15}{a-9}, \frac{-3}{a-9}\right)$.

g) $a \neq 1$ : insoluble. $a=1:(x, y, z)=(2 t, 1-3 t, t), t \in \mathbb{R}$.

h) $a=1:(x, y, z)=(1-t-u, t, u), t, u \in \mathbb{R}$. $a=-2$ : insoluble.

$a \notin\{1,-2\}:(x, y, z)=\left(\frac{a^{2}+2 a+1}{a+2}, \frac{1}{a+2},-\frac{a+1}{a+2}\right)$.

10. a) If $a \neq 3$ unique solution; if $a=3$ and $b=5$ infinitely many solutions; if $a=3$ and $b \neq 5$ no solutions.

b) If $a=b=2$ infinitely many solutions; if $a=b \neq 2$ none; if $a \neq b$ a unique solution.

11. $a=4, b=-2, c=1$.

12. $a=3, b=-5, c=-1$.

13. The polynomial $-x^{3}+3 x^{2}-2 x+1$.