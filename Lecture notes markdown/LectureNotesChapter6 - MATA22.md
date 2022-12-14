\title{
CHAPTER 6
}

\section{Matrices}

\section{Basic Properties}

\section{Definitions}

By a $p \times n$-matrix we mean an array of numbers, arranged in the form

$$
A=\left[\begin{array}{rrrr}
a_{11} & a_{12} & \ldots & a_{1 n} \\
a_{21} & a_{22} & \ldots & a_{2 n} \\
\vdots & \vdots & & \vdots \\
a_{p 1} & a_{p 2} & \ldots & a_{p n}
\end{array}\right]
$$

with $p$ rows and $n$ columns. The numbers $a_{j k}$ are called matrix elements. Notice that $a_{j k}$ is in the $j$ :th row and $k$ :th column. A more brief notation, meaning the same matrix $A$ is:

$$
A=\left(a_{j k}\right)_{j, k=1}^{p, n} .
$$

In the special case when $p=n$ we say that $A$ is a square matrix of order $n$.

\section{Arithmetic Operations}

The most basic arithmetic operations that can be performed with matrices are addition and multiplication by scalars. First of all, we should mention that two matrices are equal if they have the same dimensions and their corresponding entries agree.

Addition. Let $A=\left(a_{j k}\right)_{j, k=1}^{p, n}$ and $B=\left(b_{j k}\right)_{j, k=1}^{p, n}$ be two $p \times n$ matrices. We define $A+B$ to be the $p \times n$ matrix with entries $a_{j k}+b_{j k}$, i.e.,

$$
A+B=\left(a_{j k}+b_{j k}\right)_{j, k=1}^{p, n} \text {. }
$$

Example 1.

$$
\left[\begin{array}{rrr}
2 & 3 & -1 \\
4 & 2 & 1
\end{array}\right]+\left[\begin{array}{rrr}
3 & -2 & 1 \\
2 & 1 & 2
\end{array}\right]=\left[\begin{array}{lll}
5 & 1 & 0 \\
6 & 3 & 3
\end{array}\right]
$$

Scalar Multiplication. For a scalar $t$ we define $t A$ as the matrix with entries $t a_{j k}$.

Example 2.

$$
2 \cdot\left[\begin{array}{rrr}
2 & 3 & -1 \\
4 & 2 & 1
\end{array}\right]=\left[\begin{array}{rrr}
4 & 6 & -2 \\
8 & 4 & 2
\end{array}\right] .
$$

Matrix subtraction is defined in the following way: if $A$ and $B$ are $p \times n$ matrices we define $-A=(-1) \cdot A$ and then the difference $A-B$ is given by $A-B=A+(-1) \cdot B$. Clearly $A+(-A)=O$ where $O$ is the $p \times n$ matrix whose elements are all 0 . $(O$ is called the zero matrix.)

Matrix Multiplication. The definition of the product of two matrices is less obvious. In order to find a reasonable definition, let us consider a linear relation

$$
\left\{\begin{array}{c}
a_{11} x_{1}+a_{12} x_{2}+\cdots+a_{1 n} x_{n}=y_{1} \\
a_{21} x_{1}+a_{22} x_{2}+\cdots+a_{2 n} x_{n}=y_{2} \\
\vdots \\
a_{p 1} x_{1}+a_{p 2} x_{2}+\cdots+a_{p n} x_{n}=y_{p}
\end{array} .\right.
$$

If the numbers $y_{1}, \ldots, y_{p}$ are given, then (1) is a linear system for the unknowns $x_{1}, \ldots, x_{n}$. On the other hand, if $x_{1}, \ldots, x_{n}$ are given, then (1) gives us the values of $y_{1}, \ldots, y_{p}$. That is, the quantities $y_{1}, \ldots, y_{p}$ can via (1) be regarded as functions of $x_{1}, \ldots, x_{n}$. In order to define matrix multiplication, we shall adapt this latter point of view: we regard (1) as a recipe for a function.

Now suppose that we have another set of variables $z_{1}, \ldots, z_{q}$ which depend on $y_{1}, \ldots, y_{p}$ in a similar way,

$$
\left\{\begin{array}{c}
b_{11} y_{1}+b_{12} y_{2}+\cdots+b_{1 p} y_{p}=z_{1} \\
b_{21} y_{1}+b_{22} y_{2}+\cdots+b_{2 p} y_{p}=z_{2} \\
\vdots \\
b_{q 1} y_{1}+b_{q 2} y_{2}+\cdots+a_{q p} y_{p}=z_{q}
\end{array}\right.
$$

If we here substitute $y_{1}, \ldots, y_{p}$ by the corresponding left hand side in (1), we get a relation of the form

$$
\left\{\begin{array}{c}
c_{11} x_{1}+c_{12} x_{2}+\cdots+c_{1 n} x_{n}=z_{1} \\
c_{21} x_{1}+c_{22} x_{2}+\cdots+c_{2 n} x_{n}=z_{2} \\
\vdots \\
c_{q 1} x_{1}+c_{q 2} x_{2}+\cdots+c_{q n} x_{n}=z_{q}
\end{array}\right.
$$

where

$$
c_{j k}=b_{j 1} a_{1 k}+b_{j 2} a_{j 2}+\cdots+b_{j p} a_{p k} .
$$

Now define two matrices by

$$
A=\left[\begin{array}{rrrr}
a_{11} & a_{12} & \ldots & a_{1 n} \\
a_{21} & a_{22} & \ldots & a_{2 n} \\
\vdots & \vdots & & \vdots \\
a_{p 1} & a_{p 2} & \ldots & a_{p n}
\end{array}\right] \text { and } B=\left[\begin{array}{rrrr}
b_{11} & b_{12} & \ldots & b_{1 p} \\
b_{21} & b_{22} & \ldots & b_{2 p} \\
\vdots & \vdots & & \vdots \\
b_{q 1} & b_{p 2} & \ldots & b_{q p}
\end{array}\right] \text {. }
$$

We call these matrices the coefficient matrices of the linear equation systems (1) and (2), respectively. We define the product $B A$ to be the matrix $C=\left(c_{j k}\right)_{j, k=1}^{q, n}$ where the $c_{j k}$ are given by (4). Thus the element in position $(j, k)$ in $B A$ is obtained by pairwise multiplication of the elements of row $j$ in $B$ with the elements in column $k$ in $A$, followed by summation.

Observe that the matrix product $B A$ is defined only if the number of columns of $B$ equals to the number of rows of $A$.

Example 1.

$$
\begin{aligned}
{\left[\begin{array}{ll}
1 & 2 \\
3 & 4
\end{array}\right]\left[\begin{array}{lll}
1 & 0 & 5 \\
3 & 6 & 7
\end{array}\right] } & =\left[\begin{array}{lll}
1 \cdot 1+2 \cdot 3 & 1 \cdot 0+2 \cdot 6 & 1 \cdot 5+2 \cdot 7 \\
3 \cdot 1+4 \cdot 3 & 3 \cdot 0+4 \cdot 6 & 3 \cdot 5+4 \cdot 7
\end{array}\right] \\
& =\left[\begin{array}{rrr}
7 & 12 & 19 \\
15 & 24 & 43
\end{array}\right] .
\end{aligned}
$$

Example 2.

$$
\left[\begin{array}{lll}
1 & 2 & 3
\end{array}\right]\left[\begin{array}{l}
3 \\
2 \\
1
\end{array}\right]=\left[\begin{array}{l}
10
\end{array}\right]
$$

Example 3.

$$
\left[\begin{array}{l}
3 \\
2 \\
1
\end{array}\right]\left[\begin{array}{lll}
1 & 2 & 3
\end{array}\right]=\left[\begin{array}{lll}
3 & 6 & 9 \\
2 & 4 & 6 \\
1 & 2 & 3
\end{array}\right]
$$

Example 4.

$$
\begin{aligned}
& {\left[\begin{array}{lr}
4 & -2 \\
2 & -1
\end{array}\right]\left[\begin{array}{rr}
1 & -2 \\
-2 & 4
\end{array}\right]=\left[\begin{array}{rr}
8 & -16 \\
4 & -8
\end{array}\right],} \\
& {\left[\begin{array}{rr}
1 & -2 \\
-2 & 4
\end{array}\right]\left[\begin{array}{ll}
4 & -2 \\
2 & -1
\end{array}\right]=\left[\begin{array}{ll}
0 & 0 \\
0 & 0
\end{array}\right] .}
\end{aligned}
$$

The last example shows that the order between the factors is essential for matrix multiplication. In other words, matrix multiplication is non-commutative: it is possible (and very common) to have $A B \neq B A$.

In Example 1, $B$ is a $2 \times 2$ matrix and $A$ is a $2 \times 3$ matrix. The product $B A$ is therefore a $2 \times 3$ matrix. The product $A B$ is not defined in this case. In order to have both $A B$ and $B A$ well defined, it is necessary and sufficient that $A$ is a $n \times p$ and $B$ a $p \times n$ matrix (with the same $n$ and $p$ ). Then $B A$ is an $n \times n$ matrix and $A B$ is $p \times p$. This is illustrated by examples 2 and 3 .

Definition 1 . The square $n \times n$-matrix

$$
E=E_{n}=\left[\begin{array}{cccc}
1 & 0 & \ldots & 0 \\
0 & 1 & \ldots & 0 \\
\vdots & \vdots & & \vdots \\
0 & 0 & \ldots & 1
\end{array}\right]
$$

is called the identity matrix of order $n$.

Notice that $E$ is the neutral element for matrix multiplication, i.e. we have

$$
E A=A E=A
$$

for all $n \times n$ matrices $A$.

While matrix multiplication fails to be commutative, it obeys the other arithmetic rules.

THEOREM 2. Matrix multiplication obeys the associative law

$$
C(B A)=(C B) A
$$

and the distributive laws

$$
B\left(A+A^{\prime}\right)=B A+B A^{\prime} \quad, \quad\left(B+B^{\prime}\right) A=B A+B A^{\prime} .
$$

(We here assume that the dimensions of the matrices are such that the sums and products make sense.) Proof. The formulae can easily be verified by direct evaluation. Nevertheless, we shall give an alternative argument for the associative law (5).

Consider the relation (1) as a function $F: \mathbf{R}^{n} \rightarrow \mathbf{R}^{p}$, which to each $n$-tuple $\left(x_{1}, \ldots, x_{n}\right) \in \mathbf{R}^{n}$ associates a $p$-tuple $\left(y_{1}, \ldots, y_{p}\right) \in \mathbf{R}^{p}$. Likewise (2) can be regarded as a function $G$ from $\mathbf{R}^{p}$ to $\mathbf{R}^{q}$, which to $\left(y_{1}, \ldots, y_{p}\right)$ associates $\left(z_{1}, \ldots, z_{q}\right)$. The matrix product $B A$ will then correspond to the composite function $G \circ F$, and (5) follows from the associate law from composition of functions:

$$
H \circ(G \circ F)=(H \circ G) \circ F .
$$

We shall in this course only be concerned with matrices whose entries are real numbers. However, we mention that matrices with complex entries can be handled in the same way, as in the following example.

Example 5. Consider the three matrices

$$
I=\left[\begin{array}{rr}
i & 0 \\
0 & -i
\end{array}\right] \quad, \quad J=\left[\begin{array}{rr}
0 & 1 \\
-1 & 0
\end{array}\right] \quad, \quad K=\left[\begin{array}{ll}
0 & i \\
i & 0
\end{array}\right],
$$

where $i$ is the imaginary unit. If these are multiplied by $-i$, one obtains the famous Pauli matrices; these were used by Paul Dirac in 1928, to formulate an equation for the electron.

It is easy to check that

$$
I^{2}=J^{2}=K^{2}=-E,
$$

where $E$ is the identity matrix of order 2 , and that

$$
I J=-J I=K \quad, \quad J K=-K J=I \quad, \quad K I=-I K=J .
$$

If this is compared with the formulae for multiplication of quaternions in the preceding chapter, one realises that Hamilton's quaternions $x_{0}+x_{1} i+x_{2} j+x_{3} k$ can be identified with the set of complex $2 \times 2$ matrices of the form

$$
x_{0} E+x_{1} I+x_{2} J+x_{3} K=\left[\begin{array}{rr}
x_{0}+i x_{2} & x_{2}+i x_{3} \\
-x_{2}+i x_{3} & x_{0}-i x_{1}
\end{array}\right] .
$$

The computational rules for quaternions can then be seen as special cases of the rules for matrix multiplication.

Before we close this section, we define a new matrix operation called transposition. If $A$ is a $p \times n$ matrix, then the transpose of $A A^{t}$ is defined as the $n \times p$ matrix whose rows are the columns of $A$ :

$$
\text { If } A=\left[\begin{array}{rrrr}
a_{11} & a_{12} & \ldots & a_{1 n} \\
a_{21} & a_{22} & \ldots & a_{2 n} \\
\vdots & \vdots & & \vdots \\
a_{p 1} & a_{p 2} & \ldots & a_{p n}
\end{array}\right] \text { then } A^{t}=\left[\begin{array}{rrrr}
a_{11} & a_{21} & \ldots & a_{p 1} \\
a_{12} & a_{22} & \ldots & a_{p 2} \\
\vdots & \vdots & & \vdots \\
a_{1 n} & a_{2 n} & \ldots & a_{p n}
\end{array}\right] \text {. }
$$

Transposition satisfies the following computational rules (proofs are left as exercises for the reader)

$$
(A+B)^{t}=A^{t}+B^{t} \quad, \quad(A B)^{t}=B^{t} A^{t} .
$$

Notice that the last rule says that transposition reverses the order of a matrix product.

\section{Exercises.}

1. Let

$$
A=\left[\begin{array}{rrr}
1 & 0 & 2 \\
0 & 3 & 1 \\
2 & 2 & -1
\end{array}\right] \quad, \quad B=\left[\begin{array}{rrr}
0 & 1 & 1 \\
2 & -2 & 0 \\
1 & 2 & 3
\end{array}\right] \quad, \quad C=\left[\begin{array}{rr}
2 & 1 \\
-1 & 1 \\
1 & 2
\end{array}\right]
$$
Compute a) $A B$
b) $B A$
c) $A^{t} B^{t}$
d) $(A+3 B) C$
e) $C C^{t}$
f) $C^{t} C$.

2. Let

$$
A=\left[\begin{array}{rr}
1 & 1 \\
-1 & 1
\end{array}\right] \quad \text { and } \quad B=\left[\begin{array}{rr}
1 & -2 \\
3 & 4
\end{array}\right]
$$

Determine: a) $A^{2}-B^{2}$, b) $(A+B)(A-B)$.

Why are the answers different in a) and b)?

3. Let

$$
A=\left[\begin{array}{rr}
1 & -3 \\
-3 & 9
\end{array}\right]
$$

Find all $2 \times 2$ matrices $B$ such that

$$
A B=B A=0 .
$$

Here 0 denotes the $2 \times 2$ zero-matrix, i.e. the matrix all of whose entries equal zero.

4. Denote by $A^{k}$ the product of a matrix $A$ by itself $k$ times.

a) Prove that if $A B=B A$, then we have the binomial expansion

$$
(A+B)^{k}=A^{k}+k A^{k-1} B+\left(\begin{array}{c}
k \\
2
\end{array}\right) A^{k-2} B^{2}+\cdots+A^{k}
$$

b) Compute $(I+A)^{10}$ where $I$ is the identity matrix and

$$
A=\left[\begin{array}{lll}
0 & 5 & 3 \\
0 & 0 & 3 \\
0 & 0 & 0
\end{array}\right] .
$$

5. Show that, in order to verify all statements in Example 5, it suffices to prove that

$$
I^{2}=J^{2}=K^{2}=I J K=-E .
$$

\section{Matrix Inverse}

Let

$$
A=\left[\begin{array}{rrrr}
a_{11} & a_{12} & \ldots & a_{1 n} \\
a_{21} & a_{22} & \ldots & a_{2 n} \\
\vdots & \vdots & & \vdots \\
a_{p 1} & a_{p 2} & \ldots & a_{p n}
\end{array}\right] \quad, \quad \mathbf{x}=\left[\begin{array}{r}
x_{1} \\
x_{2} \\
\vdots \\
x_{n}
\end{array}\right] \quad, \quad \mathbf{y}=\left[\begin{array}{r}
y_{1} \\
y_{2} \\
\vdots \\
y_{p}
\end{array}\right]
$$

The linear equation system (1) can then be written in the matrix form:

$$
A \mathrm{x}=\mathrm{y} \text {. }
$$

We shall here discuss (7) in the important case when $n=p$, i.e., when $A$ is a square matrix of order $n$.

If $n=1$, the system (7) reduces to a single equation

$$
a x=y .
$$

If $a \neq 0$ this equation can be solved by multiplication with $a^{-1}=1 / a$ :

$$
x=a^{-1} y .
$$

There is a counterpart to this procedure also when $n>1$.

Definition 3 . Let $A$ be a $n \times n$-matrix. We say that $A$ is invertible if there is an $n \times n$-matrix $B$ such that

$$
A B=E \quad \text { and } \quad B A=E .
$$

In this case, $B$ is called an inverse to $A$. REmarK 4. If $A$ is invertible, then the inverse is unique. We can thus speak of the inverse and write $B=A^{-1}$. To see this, assume that there are two matrices $B$ and $C$ which are inverse to $A$. Then $B A=E$ and $A C=E$, so

$$
B=B E=B(A C)=(B A) C=E C=C .
$$

The uniqueness is proved.

Example 1. If

$$
A=\left[\begin{array}{ll}
1 & 2 \\
2 & 3
\end{array}\right] \quad, \quad B=\left[\begin{array}{rr}
-3 & 2 \\
2 & -1
\end{array}\right]
$$

then by direct calculation, $A B=B A=E$. Thus $A$ is invertible and $B=A^{-1}$. For the same reason, $B$ is invertible and $A=B^{-1}$.

Now suppose that $A$ is an invertible matrix. The linear system

$$
A \mathrm{x}=\mathrm{y}
$$

can then be multiplied by $A^{-1}$ from the left, giving

$$
\mathbf{x}=E \mathbf{x}=\left(A^{-1} A\right) \mathbf{x}=A^{-1}(A \mathbf{x})=A^{-1} \mathbf{y} .
$$

If the system has a solution $\mathbf{x}$ we must thus have $\mathbf{x}=A^{-1} \mathbf{y}$. That this really is a solution follows from that

$$
A\left(A^{-1} \mathbf{y}\right)=\left(A A^{-1}\right) \mathbf{y}=E \mathbf{y}=\mathbf{y} .
$$

We have proved one direction of the following theorem.

ThEOREM 5. A square matrix $A$ is invertible if and only if the linear equation system $A \mathbf{x}=\mathbf{y}$ has a unique solution $\mathbf{x}$ for all right hand sides $\mathbf{y}$. If this is the case, the solution is given by $\mathbf{x}=A^{-1} \mathbf{y}$.

REMARK 6 . In the proof we shall make use of the following property of matrix multiplication: If $C$ is a square matrix with columns $C_{1}, C_{2}, \ldots, C_{n}$, then the matrix $A C$ has columns $A C_{1}, A C_{2}, \ldots, A C_{n}$. The (simple) verification of this fact is left as an exercise for the interested reader.

Proof of Theorem 5. It remains to prove that if the system $A \mathbf{x}=\mathbf{y}$ has a unique solution for all possible right hand sides $\mathbf{y}$, then $A$ is invertible.

Let $C$ and $D$ be two square matrices with columns $C_{1}, C_{2}, \ldots, C_{n}$ and $D_{1}, D_{2}, \ldots, D_{n}$, respectively. By Remark 6 , the matrix identity

$$
A C=D
$$

is equivalent to the $n$ vector identities

$$
A C_{k}=D_{k}, \quad k=1, \ldots, n .
$$

Hence if the system $A \mathbf{x}=\mathbf{y}$ has a unique solution for all $\mathbf{y}$, there is precisely one $n \times n$ matrix $D$ satisfying (8). In particular there is a unique $n \times n$ matrix $B$ such that

$$
A B=E .
$$

In order to show that $A$ is invertible, we shall show that also $B A=E$. But by (9) we have

$$
A(B A)=(A B) A=E A=A .
$$

The matrix $C=B A$ thus satisfies the equation

$$
A C=A .
$$

This last equation is also satisfied by $C=E$. Since (8) has precisely one solution $C$ for every right hand side $D$, we must then have $B A=E$.

The following example shows how one can calculate inverse matrices in practice.

Example 2. To determine whether the matrix

$$
A=\left[\begin{array}{lll}
1 & 1 & 1 \\
1 & 2 & 3 \\
1 & 3 & 2
\end{array}\right]
$$

is invertible, we try to solve the system $A \mathbf{x}=\mathbf{y}$ for an arbitrary right hand side $\mathbf{y}$ :

$$
\begin{gathered}
\left\{\begin{array}{l}
x_{1}+x_{2}+x_{3}=y_{1} \\
x_{1}+2 x_{2}+3 x_{3}=y_{2} \\
x_{1}+3 x_{2}+2 x_{3}=y_{3}
\end{array}\right. \\
\sim\left\{\begin{aligned}
& x_{1}+x_{2}+x_{3}=y_{1} \\
& x_{2}+2 x_{3}=-y_{1}+y_{2} \\
& x_{2}-x_{3}=-y_{2}+y_{3}
\end{aligned}\right. \\
\sim \quad \cdots \quad \sim \quad=5 y_{1}-y_{2}-y_{3} \\
\cdots\left\{\begin{array}{rl}
3 x_{1} \quad 3 x_{2} \quad=-y_{1}-y_{2}+2 y_{3} \\
3 x_{3} & =-y_{1}+2 y_{2}-y_{3}
\end{array} .\right.
\end{gathered}
$$

We see that the system has a unique solution $\mathbf{x}$ for each right hand side $\mathbf{y}$, so the matrix $A$ is invertible. The last system also shows that

$$
A^{-1}=\frac{1}{3}\left[\begin{array}{rrr}
5 & -1 & -1 \\
-1 & -1 & 2 \\
-1 & 2 & -1
\end{array}\right] \text {. }
$$

Computational Rules for the Inverse. If both of the matrices $A$ and $B$ are invertible, then the product $A B$ is also invertible, and

$$
(A B)^{-1}=B^{-1} A^{-1} .
$$

The order between factors is thus reversed after inversion. This is realised by observing that if $A$ and $B$ are invertible then the matrix $D=B^{-1} A^{-1}$ satisfies

$$
D(A B)=B^{-1}\left(A^{-1} A\right) B=B^{-1} E B=B^{-1} B=E \text {, }
$$

and similarly

$$
(A B) D=E .
$$

Thus $A B$ is invertible with inverse $D$.

Finally, we leave it to the reader to check that if $A$ is invertible, then $A^{t}$ is invertible and

$$
\left(A^{t}\right)^{-1}=\left(A^{-1}\right)^{t} .
$$

\section{Exercises.}

6. Determine which of the matrices below are invertible. Also determine the inverse matrix when it exists.
a) $\left[\begin{array}{lll}1 & 2 & 3 \\ 0 & 1 & 2 \\ 0 & 0 & 1\end{array}\right]$
b) $\left[\begin{array}{rrr}1 & 1 & 2 \\ 2 & 1 & 1 \\ -1 & 1 & 4\end{array}\right]$
c) $\left[\begin{array}{lll}1 & 0 & 1 \\ 0 & 1 & 1 \\ 1 & 1 & 0\end{array}\right]$.

7. Let

$$
A=\left[\begin{array}{rrr}
1 & 0 & a \\
0 & -1 & 1 \\
1 & 1 & 0
\end{array}\right] .
$$

Calculate $A^{-1}$ for those values of $a$ for which $A$ is invertible.

8. Find the inverse matrices of $A$ and of $A^{2}$ where

$$
A=\left[\begin{array}{lll}
1 & 2 & 3 \\
2 & 3 & 1 \\
1 & 1 & 1
\end{array}\right] .
$$

9. Find a matrix $X$ which solves the matrix equation $A X B=C$ where

$$
A=\left[\begin{array}{ll}
1 & 1 \\
1 & 2
\end{array}\right] \quad, \quad B=\left[\begin{array}{lll}
1 & 2 & 3 \\
0 & 1 & 2 \\
0 & 0 & 1
\end{array}\right] \quad, \quad C=\left[\begin{array}{lll}
1 & 2 & 1 \\
2 & 1 & 2
\end{array}\right] .
$$

10. Let $A$ and $B$ be two $n \times n$-matrices such that $E-A B$ is invertible. Prove that $E-B A$ is invertible and that

$$
(E-B A)^{-1}=E+B(E-A B)^{-1} A .
$$

\section{Answers to Exercises}

1. a) $\left[\begin{array}{rrr}2 & 5 & 7 \\ 7 & -4 & 3 \\ 3 & -4 & -1\end{array}\right] \quad$ b) $\left[\begin{array}{rrr}2 & 5 & 0 \\ 0 & -6 & 2 \\ 7 & 12 & 1\end{array}\right] \quad$ c) $\left[\begin{array}{rrr}2 & 2 & 7 \\ 5 & -6 & 12 \\ 0 & 2 & 1\end{array}\right]$ d) $\left[\begin{array}{rr}4 & 14 \\ 16 & 5 \\ 10 & 29\end{array}\right]$

e) $\left[\begin{array}{rrr}5 & -1 & 4 \\ -1 & 2 & 1 \\ 4 & 1 & 5\end{array}\right]$ f) $\left[\begin{array}{ll}6 & 3 \\ 3 & 6\end{array}\right]$

2. a) $\left[\begin{array}{rr}5 & 12 \\ -17 & -10\end{array}\right] \quad$ b) $\left[\begin{array}{rr}4 & 9 \\ -20 & -9\end{array}\right]$.

3. $\left[\begin{array}{cc}9 t & 3 t \\ 3 t & t\end{array}\right], t \in \mathbb{R}$

4. b) $(E+A)^{10}=\left[\begin{array}{rrr}1 & 50 & 705 \\ 0 & 1 & 30 \\ 0 & 0 & 1\end{array}\right]$.

6. a) $\left[\begin{array}{rrr}1 & -2 & 1 \\ 0 & 1 & -2 \\ 0 & 0 & 1\end{array}\right]$. b) Not invertible. c) $\frac{1}{2}\left[\begin{array}{rrr}1 & -1 & 1 \\ -1 & 1 & 1 \\ 1 & 1 & -1\end{array}\right]$.

7. $A^{-1}=\frac{1}{1-a}\left[\begin{array}{rrr}1 & -a & -a \\ -1 & a & 1 \\ -1 & 1 & 1\end{array}\right]$ for $a \neq 1$. 8. $A^{-1}=\frac{1}{3}\left[\begin{array}{rrr}-2 & -1 & 7 \\ 1 & 2 & -5 \\ 1 & -1 & 1\end{array}\right], \quad\left(A^{2}\right)^{-1}=\frac{1}{9}\left[\begin{array}{rrr}10 & -7 & -2 \\ -5 & 8 & -8 \\ -2 & -4 & 13\end{array}\right]$.

9. $X=A^{-1} C B^{-1}=\left[\begin{array}{rrr}0 & 3 & -6 \\ 1 & -3 & 4\end{array}\right]$.