$$\begin{cases}
x_{1}+3x_{2}+4x_{3}=15 \\
2x_{1}+9x_{2}+14x_{3}=48 \\
x_{1}+5x_{2}+11x_{3}=33
\end{cases}$$
$$\begin{bmatrix}
1 & 3 & 4 \\
2 & 9 & 14 \\
1 & 5 & 11
\end{bmatrix}=
\begin{bmatrix}
\ell_{11} & 0 & 0 \\
\ell_{21} & \ell_{22} & 0 \\
\ell_{31} & \ell_{32} & \ell_{33}
\end{bmatrix}\cdot
\begin{bmatrix}
1 & u_{12} & u_{13} \\
0 & 1 & u_{23} \\
0 & 0 & 1
\end{bmatrix}$$
$\ell_{11}=1$
$\ell_{11}u_{12}=3\Rightarrow u_{12}=3$
$\ell_{11}u_{13}=4\Rightarrow u_{13}=4$

$\ell_{21}=2$
$\ell_{21}u_{12}+\ell_{22}=9\Rightarrow \ell_{22}=3$
$\ell_{21}u_{13}+\ell_{22}u_{23}=14\Rightarrow u_{23}=2$

$\ell_{31}=1$
$\ell_{31}u_{12}+\ell_{32}=5\Rightarrow \ell_{32}=2$
$\ell_{31}u_{13}+\ell_{32}u_{23}+\ell_{33}=11\Rightarrow \ell_{33}=3$

Therefore,
$$\begin{bmatrix}
1 & 3 & 4 \\
2 & 9 & 14 \\
1 & 5 & 11
\end{bmatrix}=
\begin{bmatrix}
1 & 0 & 0 \\
2 & 3 & 0 \\
1 & 2 & 3
\end{bmatrix}\cdot
\begin{bmatrix}
1 & 3 & 4 \\
0 & 1 & 2 \\
0 & 0 & 1
\end{bmatrix}$$
