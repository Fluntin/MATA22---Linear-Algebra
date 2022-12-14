\title{
CHAPTER 7
}

\section{Determinants}

In the previous chapter we have seen that a linear system of equations

$$
\left\{\begin{array}{c}
a_{11} x_{1}+a_{12} x_{2}+\ldots+a_{1 n} x_{n}=y_{1} \\
a_{21} x_{1}+a_{22} x_{2}+\ldots+a_{2 n} x_{n}=y_{2} \\
\ldots \\
a_{n 1} x_{1}+a_{n 2} x_{2}+\ldots+a_{n n} x_{n}=y_{n}
\end{array}\right.
$$

can be written using matrix multiplication as $A X=Y$ where

$$
A=\left[\begin{array}{cccc}
a_{11} & a_{12} & \ldots & a_{1 n} \\
a_{21} & a_{22} & \ldots & a_{2 n} \\
\vdots & \vdots & \ddots & \vdots \\
a_{n 1} & a_{n 2} & \ldots & a_{n n}
\end{array}\right], \quad X=\left[\begin{array}{c}
x_{1} \\
x_{2} \\
\vdots \\
x_{n}
\end{array}\right] \quad \text { and } \quad Y=\left[\begin{array}{c}
y_{1} \\
y_{2} \\
\vdots \\
y_{n}
\end{array}\right]
$$

We also showed that a quadratic matrix $A$ is invertible if and only if the corresponding system $A X=Y$ has unique solution for every $n \times 1$ matrix $Y$. Thus, the invertibility of the matrix $A$, i.e. the existence of a matrix $A^{-1}$ such that $A A^{-1}=A^{-1} A=E$, can be directly verified by solving the system $A X=Y$ for an arbitrary $Y$. It turns out that this question is closely related to determinants. Recall that we have introduced determinants of order $n=2,3$ in connection with our previous discussion on the volume product of three vectors.

Let us first explore this connection in the case where $A$ is a $3 \times 3$ matrix. The columns $A_{1}, A_{2}, A_{3}$ of the matrix $A$ can be interpreted as vectors in $\mathbb{R}^{3}$ with respect to some orthonormal basis. Then the corresponding system $A X=Y$ can be written as:

$$
\{\begin{array}{l}
a_{11} x_{1}+a_{12} x_{2}+a_{13} x_{3}=y_{1} \\
a_{21} x_{1}+a_{22} x_{2}+a_{23} x_{3}=y_{2} \\
a_{31} x_{1}+a_{32} x_{2}+a_{33} x_{3}=y_{3}
\end{array} \Longleftrightarrow \underbrace{\left[\begin{array}{l}
a_{11} \\
a_{21} \\
a_{31}
\end{array}\right]}_{A_{1}} x_{1}+\underbrace{\left[\begin{array}{c}
a_{12} \\
a_{22} \\
a_{32}
\end{array}\right]}_{A_{2}} x_{2}+\underbrace{\left[\begin{array}{l}
a_{13} \\
a_{23} \\
a_{33}
\end{array}\right]}_{A_{3}} x_{Y}=\left[\begin{array}{l}
y_{1} \\
y_{2} \\
y_{3}
\end{array}\right] x_{3}
$$

that is, $x_{1} A_{1}+x_{2} A_{2}+x_{3} A_{3}=Y$.

Thus, the fact that $A$ is invertible and the linear system $A X=Y$ has unique solution for each $Y$ is equivalent to the linear independence of the vectors $A_{1}, A_{2}$, $A_{3}$. Recall that we have showed that three vectors in space are linearly independent if and only if their volume product is non-zero. Using the terminology introduced in the previous chapters we can state that $A$ is invertible if and only if its columns $A_{1}, A_{2}, A_{3}$ are linearly independent, that is the volume product $V\left(A_{1}, A_{2}, A_{3}\right)$ and hence the determinant $D(A)$ of the matrix $A$ is non-zero.

These observations can be summarized as follows.

Theorem 1. Let $A$ be a $3 \times 3$ matrix, $A_{1}, A_{2}, A_{3}$ denote its columns. The following are equivalent:

i. The matrix $A$ is invertible.

ii. The linear system $A X=Y$ has a unique solution $X=A^{-1} Y$ for every $3 \times 1$ matrix $Y$.

iii. The vectors $A_{1}, A_{2}, A_{3}$ are linearly independent.

iv. The volume product $V\left(A_{1}, A_{2}, A_{3}\right)$ is non-zero.

v. The determinant $D(A)$ of the matrix $A$ is non-zero.

The above theorem can be generalized to higher dimensions. If $A$ is a $n \times n$ matrix, the determinant $D(A)$ of $A$ is defined as a number that corresponds to the signed "volume" of the generalized parallelepiped spanned by the columns $A_{1}, A_{2}, \ldots, A_{n}$ of $A$ viewed as vectors in the $\mathrm{n}$-dimensional space $\mathbb{R}^{n}$.

Historically, determinants have played a crucial role in the development of linear algebra as a branch of mathematics. Determinants appear in a natural way in connection to linear systems of equations but they were introduced long before matrices were established as mathematical objects in their own right.

\section{Definition and Properties}

Let

$$
A=\left[\begin{array}{cccc}
a_{11} & a_{12} & \ldots & a_{1 n} \\
a_{21} & a_{22} & \ldots & a_{2 n} \\
\vdots & \vdots & \ddots & \vdots \\
a_{n 1} & a_{n 2} & \ldots & a_{n n}
\end{array}\right]
$$

be a quadratic matrix of order $n$. For the determinant of $A$ that will be defined in this section we use the notations

$$
D(A)=D\left(A_{1}, A_{2}, \ldots, A_{n}\right)=\operatorname{det}(A)=\left|\begin{array}{cccc}
a_{11} & a_{12} & \ldots & a_{1 n} \\
a_{21} & a_{22} & \ldots & a_{2 n} \\
\vdots & \vdots & \ddots & \vdots \\
a_{n 1} & a_{n 2} & \ldots & a_{n n}
\end{array}\right| .
$$

For $n=1, A=\left[a_{11}\right]$ we define $D(A)=a_{11}$.

For $n=2, A=\left[\begin{array}{ll}a_{11} & a_{12} \\ a_{21} & a_{22}\end{array}\right]$ we define

$$
D(A)=\left|\begin{array}{ll}
a_{11} & a_{12} \\
a_{21} & a_{22}
\end{array}\right|=a_{11} a_{22}-a_{12} a_{21} .
$$

Note that if the columns $A_{1}$ and $A_{2}$ of the matrix $A$ are viewed as the vectors with coordinates $\left(a_{11}, a_{21}\right)$ and $\left(a_{12}, a_{22}\right)$ in a plane with respect to some orthonormal basis, then $|D(A)|$ is the area of the parallelogram spanned by these vectors. The area (and hence the determinant) is non-zero precisely when the vectors $A_{1}, A_{2}$ are linearly independent.

For $n=3, A=\left[\begin{array}{lll}a_{11} & a_{12} & a_{13} \\ a_{21} & a_{22} & a_{23} \\ a_{31} & a_{32} & a_{33}\end{array}\right]$ we define

$$
D(A)=\left|\begin{array}{ccc}
a_{11} & a_{12} & a_{13} \\
a_{21} & a_{22} & a_{23} \\
a_{31} & a_{32} & a_{33}
\end{array}\right|=\begin{gathered}
a_{11} a_{22} a_{33}+a_{12} a_{23} a_{31}+a_{21} a_{32} a_{13} \\
-a_{13} a_{22} a_{31}-a_{12} a_{21} a_{33}-a_{11} a_{23} a_{32}
\end{gathered} .
$$

Before we introduce determinants of higher orders than 3, let us mention a number of fundamental properties shared by the determinants of order 2 and 3 . These properties are direct consequences of the connection between second-order determinants and area and third-order determinants and volume, and they can be easily verified by direct computations.

Property I. $D(A)$ depends linearly on each column of the matrix A.

Property II. $D(A)=0$ if two columns of the matrix A are equal.

Property III. $D(E)=1$ (where $E$ is the unit matrix).

In general, for every positive integer $n$ we can define a number $D(A)$ associated to a quadratic matrix $A$ of order $n$ such that the properties I-III are fulfilled. Moreover, the definition is uniquely determined by these properties. The proof of this statement will be carried out in detail in the next course in Linear Algebra. Using the properties above and direct computations one can show further properties shared by determinants of order 2 and 3 , and that can be generalized to higher dimensions.

Property IV. $D(A)$ changes sign if two columns are interchanged. (follows from [I] and $[\mathrm{II}])$.

Property V. $D(A)$ does not change if a multiple of a column is added to another column.

Property VI. $D(A)=D\left(A^{t}\right)$ (The Symmetry Theorem).

Property VII. $D(A)$ is unique (The Uniqueness Theorem).

Remark. By the Symmetry Theorem, the statements I, II, III-IV still hold if we replace "column/columns" with "row/rows".

Example 1. Let us illustrate how these properties can be used to compute a determinant of order 3 without using Sarrus' rule. Consider the determinant

$$
D=\left|\begin{array}{rrr}
1 & -1 & 2 \\
-2 & 2 & -2 \\
3 & -2 & 7
\end{array}\right| .
$$

We first use Property V and add the first column to the second column. Next we multiply the first column by $(-2)$ and add this multiple to the third column. This gives:

$$
D=\left|\begin{array}{rrr}
1 & 0 & 2 \\
-2 & 0 & -2 \\
3 & 1 & 7
\end{array}\right|=\left|\begin{array}{rrr}
1 & 0 & 0 \\
-2 & 0 & 2 \\
3 & 1 & 1
\end{array}\right|=-\left|\begin{array}{rrr}
1 & 0 & 0 \\
-2 & 2 & 0 \\
3 & 1 & 1
\end{array}\right| .
$$

The last equality follows by interchanging the last two columns. We can factor out 2 from the second row to obtain:

$$
D=-2\left|\begin{array}{rrr}
1 & 0 & 0 \\
-1 & 1 & 0 \\
3 & 1 & 1
\end{array}\right| \text {. }
$$

Adding the first row to the second row and $(-3)$ times the first row to the third row we obtain

$$
D=-2\left|\begin{array}{lll}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 1 & 1
\end{array}\right| .
$$

Finally, subtracting the second row from the first we get

$$
D=-2\left|\begin{array}{lll}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{array}\right|=-2 D(E)=-2 .
$$

The calculations above are unnecessarily lengthy. The process of computing determinants can be simplified by combining the properties with the recursive definition of determinants.

Definition 2. If $A$ is a $n \times n$ matrix we denote by $A^{(j k)}$ the $(n-1) \times(n-1)$ matrix obtained by removing row $j$ and column $k$ from $A$.

For each $j=1, \ldots, n$, the determinant of $A$ is given by

$$
D(A)=\sum_{k=1}^{n}(-1)^{j+k} a_{j k} D\left(A^{(j k)}\right) .
$$

The formula above is called expansion on row $j$. One can prove that $D(A)$ satisfies all the properties I-VII mentioned above. One can also show that similar expansion formulas using one of the columns of $A$ instead of a row yield $D(A)$ as well (see property VI and VII). For each $k=1, \ldots, n$, the determinant of $A$ is also given by

$$
D(A)=\sum_{j=1}^{n}(-1)^{j+k} a_{j k} D\left(A^{(j k)}\right) .
$$

Example 2. Expansion on the first row of the determinant of a quadratic matrix of order 3 gives:

$$
\begin{aligned}
\left|\begin{array}{lll}
a_{11} & a_{12} & a_{13} \\
a_{21} & a_{22} & a_{23} \\
a_{31} & a_{32} & a_{33}
\end{array}\right| & =(-1)^{1+1} a_{11}\left|\begin{array}{ll}
a_{22} & a_{23} \\
a_{32} & a_{33}
\end{array}\right|+(-1)^{1+2} a_{12}\left|\begin{array}{ll}
a_{21} & a_{23} \\
a_{31} & a_{33}
\end{array}\right|+(-1)^{1+3} a_{13}\left|\begin{array}{ll}
a_{21} & a_{22} \\
a_{31} & a_{32}
\end{array}\right|= \\
& =a_{11}\left(a_{22} a_{33}-a_{23} a_{32}\right)-a_{12}\left(a_{21} a_{33}-a_{23} a_{31}\right)+a_{13}\left(a_{21} a_{32}-a_{22} a_{31}\right) .
\end{aligned}
$$

Example 3. Using for instance expansion on the first row we can compute the following determinant:

$$
\left|\begin{array}{rrrr}
1 & 3 & 2 & 0 \\
1 & 2 & 3 & -1 \\
2 & 0 & 5 & 3 \\
0 & 6 & -3 & 6
\end{array}\right|=1\left|\begin{array}{rrr}
2 & 3 & -1 \\
0 & 5 & 3 \\
6 & -3 & 6
\end{array}\right|-3\left|\begin{array}{rrr}
1 & 3 & -1 \\
2 & 5 & 3 \\
0 & -3 & 6
\end{array}\right|+2\left|\begin{array}{rrr}
1 & 2 & -1 \\
2 & 0 & 3 \\
0 & 6 & 6
\end{array}\right| .
$$

We can of course continue by computing the determinants in the right-hand side using our favorite tools (Sarrus' rule, expansion and/or the properties of the determinants) but the computations can be simplified if we combine the expansion formula with the tools provided by the fundamental properties of the determinants. We can first add suitable multiples of one column (or row) to the other columns in order to create zero elements on a certain row. For example, we could multiply the first row by $(-3)$ and add this multiple to the second column, and by $(-2)$ and add the multiple to the third column to create zeros on the first row before we use expansion on this row:

$$
\left|\begin{array}{rrrr}
1 & 3 & 2 & 0 \\
1 & 2 & 3 & -1 \\
2 & 0 & 5 & 3 \\
0 & 6 & -3 & 6
\end{array}\right|=\left|\begin{array}{rrrr}
1 & 0 & 0 & 0 \\
1 & -1 & 1 & -1 \\
2 & -6 & 1 & 3 \\
0 & 6 & -3 & 6
\end{array}\right|=\left|\begin{array}{rrr}
-1 & 1 & -1 \\
-6 & 1 & 3 \\
6 & -3 & 6
\end{array}\right| .
$$

We can now add the first column to the second column and subtract it from the third before we use expansion again:

$$
\left|\begin{array}{rrr}
-1 & 1 & -1 \\
-6 & 1 & 3 \\
6 & -3 & 6
\end{array}\right|=\left|\begin{array}{rrr}
-1 & 0 & 0 \\
-6 & -5 & 9 \\
6 & 3 & 0
\end{array}\right|=-(1)\left|\begin{array}{rr}
-5 & 9 \\
3 & 0
\end{array}\right|=-((-5) \cdot 0-9 \cdot 3)=27 .
$$

We conclude this section with one more example.

Example 4. The determinant of a triangular matrix of the form

$$
A=\left[\begin{array}{ccccc}
a_{11} & a_{12} & a_{13} & \ldots & a_{1 n} \\
0 & a_{22} & a_{23} & \ldots & a_{2 n} \\
0 & 0 & a_{33} & \ldots & a_{3 n} \\
\vdots & \vdots & \ddots & \vdots & \\
0 & 0 & 0 & \ldots & a_{n n}
\end{array}\right]
$$

is given by the product $a_{11} a_{22} \cdot \ldots \cdot a_{n n}$ of the elements on the main diagonal. This is easily seen by repeated expansion on the first column.

\section{Exercises.}

1. Compute the following determinants:
а) $\left|\begin{array}{rrr}-1 & 1 & 3 \\ -1 & 1 & 2 \\ 4 & 5 & -1\end{array}\right|$
b) $\left|\begin{array}{rrr}0 & 1 & 7 \\ -2 & 1 & -1 \\ 3 & 2 & 1\end{array}\right|$
c) $\left|\begin{array}{lll}0 & 1 & 1 \\ 1 & 0 & 1 \\ 1 & 1 & 0\end{array}\right|$
d) $\left|\begin{array}{lll}a & b & b \\ b & a & b \\ b & b & a\end{array}\right|$. 2. Compute the following determinants:
a) $\left|\begin{array}{llll}2 & 1 & 1 & 1 \\ 1 & 2 & 1 & 1 \\ 1 & 1 & 2 & 1 \\ 1 & 1 & 1 & 2\end{array}\right|$
b) $\left|\begin{array}{llll}1 & 2 & 3 & 4 \\ 2 & 3 & 4 & 1 \\ 3 & 4 & 1 & 2 \\ 4 & 1 & 2 & 3\end{array}\right|$
$\left|\begin{array}{rrrr}-1 & 0 & 1 & 2 \\ 2 & -1 & 3 & 4 \\ 5 & -1 & 1 & 1 \\ 2 & -2 & 4 & 1\end{array}\right|$

3. Let $a \in \mathbb{R}$. Solve the equation

$$
\left|\begin{array}{llll}
x & a & a & a \\
a & x & a & a \\
a & a & x & a \\
a & a & a & x
\end{array}\right|=0 .
$$

4. Consider the matrices $A=\left[\begin{array}{rrr}2 & 0 & 1 \\ 0 & 3 & 1 \\ -2 & 2 & 1\end{array}\right]$ and $B=\left[\begin{array}{rrr}-2 & 5 & -1 \\ 3 & -1 & 5 \\ 2 & 6 & 1\end{array}\right]$.

Compute the determinants $D(A), D(B), D(A \cdot B)$ and $D(A+B)$.

\section{Determinants and the Inverse of a Matrix}

In the introductory part of this chapter we have proved that a quadratic matrix of order less than or equal to 3 is invertible if and only if its determinant is non-zero. This is true in general for a $n \times n$ matrix $A$ and we also have that

$$
D\left(A^{-1}\right)=\frac{1}{D(A)} .
$$

This statement can be proved using another fundamental property of determinants namely the product rule:

If $A$ and $B$ are two $n \times n$ matrices, then $D(A B)=D(A) \cdot D(B)$.

The proofs of these statements will be carried out in detail in the course Linear Algebra 2.

In what follows let $A$ be an invertible matrix of order $n$. There is a formula, called Cramer's rule after the mathematician Gabriel Cramer (1704-1752) that expresses the solution $X$ of the system $A X=Y$ using determinants. The formula reads as follows:

$$
x_{j}=\frac{D\left(A_{1}, \ldots, Y, \ldots, A_{n}\right)}{D\left(A_{1}, \ldots, A_{j}, \ldots, A_{n}\right)}, \quad j=1, \ldots, n .
$$

The determinant in the denominator is $D(A)$ while $D\left(A_{1}, \ldots, Y, \ldots, A_{n}\right)$ is the determinant of a matrix obtained from $A$ by replacing its j'th column by $Y$. We will prove this formula and the fact that the inverse of $A$ is given by

$$
A^{-1}=\frac{1}{D(A)}\left[\begin{array}{ccc}
(-1)^{1+1} D\left(A^{(11)}\right) & \ldots & (-1)^{1+n} D\left(A^{(1 n)}\right) \\
(-1)^{2+1} D\left(A^{(21)}\right) & \ldots & (-1)^{2+n} D\left(A^{(2 n)}\right) \\
\ldots & \ldots & \ldots \\
(-1)^{n+1} D\left(A^{(n 1)}\right) & \ldots & (-1)^{n+n} D\left(A^{(n n)}\right)
\end{array}\right]^{t} .
$$

Proof. Recall that $A X=Y$ can be written as $x_{1} A_{1}+x_{2} A_{2}+\cdots+x_{n} A_{n}=Y$.

Using this we can write

$$
\begin{aligned}
D(A_{1}, \ldots, \underbrace{Y}_{j^{\prime} \text { th column }} & \left., \ldots, A_{n}\right)=D\left(A_{1}, \ldots, \sum_{k=1}^{n} x_{k} A_{k}, \ldots, A_{n}\right)= \\
& =\sum_{k=1}^{n} x_{k} D(A_{1}, \ldots, \underbrace{A_{k}}_{j^{\prime} \text { th column }}, \ldots, A_{n})=x_{j} D\left(A_{1}, \ldots, A_{j}, \ldots, A_{n}\right) .
\end{aligned}
$$

Thus,

$$
x_{j}=\frac{D\left(A_{1}, \ldots, Y, \ldots, A_{n}\right)}{D(A)}, \quad j=1, \ldots, n .
$$

On the other hand, expansion of $D\left(A_{1}, \ldots, Y, \ldots, A_{n}\right)$ on the $j$ 'th column $Y$ gives

$$
\begin{aligned}
& D\left(A_{1}, \ldots, Y, \ldots, A_{n}\right)= \\
& \quad=(-1)^{1+j} y_{1} D\left(A^{(1 j)}\right)+(-1)^{2+j} y_{2} D\left(A^{(2 j)}\right)+\ldots+(-1)^{n+j} y_{n} D\left(A^{(n j)}\right) \\
& \quad=\left[\begin{array}{llll}
(-1)^{1+j} D\left(A^{(1 j)}\right) & (-1)^{2+j} D\left(A^{(2 j)}\right) & \ldots & (-1)^{n+j} D\left(A^{(n j)}\right.
\end{array}\right]\left[\begin{array}{c}
y_{1} \\
y_{2} \\
\vdots \\
y_{n}
\end{array}\right]
\end{aligned}
$$

Putting these together we obtain

$$
\underbrace{\left[\begin{array}{c}
x_{1} \\
x_{2} \\
\vdots \\
x_{n}
\end{array}\right]}_{X}=\underbrace{\frac{1}{D(A)}\left[\begin{array}{ccc}
(-1)^{1+1} D\left(A^{(11)}\right) & \ldots & (-1)^{n+1} D\left(A^{(n 1)}\right) \\
(-1)^{1+2} D\left(A^{(12)}\right) & \ldots & (-1)^{n+2} D\left(A^{(n 2)}\right) \\
\ldots & \ldots & \ldots \\
(-1)^{1+n} D\left(A^{(1 n)}\right) & \ldots & (-1)^{n+n} D\left(A^{(n n)}\right)
\end{array}\right]}_{A^{-1}} \underbrace{\left[\begin{array}{c}
y_{1} \\
y_{2} \\
\vdots \\
y_{n}
\end{array}\right]}_{Y} .
$$

Note the reversal of the indices. The equality above can be written as: 

$$
A^{-1}=\frac{1}{D(A)}\left[\begin{array}{ccc}
(-1)^{1+1} D\left(A^{(11)}\right) & \ldots & (-1)^{1+n} D\left(A^{(1 n)}\right) \\
(-1)^{2+1} D\left(A^{(21)}\right) & \ldots & (-1)^{2+n} D\left(A^{(2 n)}\right) \\
\ldots & \ldots & \cdots \\
(-1)^{n+1} D\left(A^{(n 1)}\right) & \ldots & (-1)^{n+n} D\left(A^{(n n)}\right)
\end{array}\right]^{t}
$$

which completes the proof.

The methods described earlier for solving systems of equations and finding inverses usually involve shorter calculations than the methods of the last two theorems. One exception to this is the following formula for the inverse of an invertible $2 \times 2$ matrix:

$$
\left[\begin{array}{ll}
a_{11} & a_{12} \\
a_{21} & a_{22}
\end{array}\right]^{-1}=\frac{1}{a_{11} a_{22}-a_{12} a_{21}}\left[\begin{array}{cc}
a_{22} & -a_{12} \\
-a_{21} & a_{11}
\end{array}\right]
$$

We conclude this section by computing the inverse of the matrix $A=\left[\begin{array}{lll}1 & 0 & 2 \\ 0 & 3 & 1 \\ 1 & 2 & 0\end{array}\right]$. We have that $D(A)=-8$ and by Cramer's rule we get

$$
\begin{aligned}
& A^{-1}=-\frac{1}{8}\left[-\left|\begin{array}{ll}\left|\begin{array}{ll}3 & 1 \\2 & 0\end{array}\right|-\left|\begin{array}{ll}0 & 1 \\1 & 0\end{array}\right| \\0 & 2 \\2 & 0\end{array}\right|\left|\begin{array}{ll}0 & 3 \\1 & 2\end{array}\right|\right]^{t} \\
& =-\frac{1}{8}\left[\begin{array}{rrr}-2 & 1 & -3 \\4 & -2 & -2 \\-6 & -1 & 3\end{array}\right]^{t}=\frac{1}{8}\left[\begin{array}{rrr}2 & -4 & 6 \\-1 & 2 & 1 \\3 & 2 & -3\end{array}\right]
\end{aligned}
$$

\section{Exercises.}

5. Use Cramer's rule to compute the inverse of the following matrices:

$$
A=\left[\begin{array}{ll}
3 & 4 \\
2 & 3
\end{array}\right] \quad, \quad B=\left[\begin{array}{rrr}
2 & 2 & 3 \\
1 & -1 & 1 \\
-1 & 2 & 1
\end{array}\right] \quad, \quad C=\left[\begin{array}{rrrr}
1 & 2 & 3 & 4 \\
0 & -1 & 2 & 1 \\
0 & 0 & 1 & 2 \\
0 & 0 & 0 & -1
\end{array}\right]
$$