Por comodidad, de ahora en adelante cada sistema lineal tendrá una **matriz asociada**. Por ahora, podemos pensar en una matriz como si fuera un cajón de números; por supuesto, tiene un significado más profundo que estudiaremos más tarde

$$
\left\{
\begin{array}{rrrrrrrcl}
a_{11}x_1 & + & a_{12}x_2 & + & \cdots & + & a_{1n}x_n & = & b_1\\
a_{21}x_1 & + & a_{22}x_2 & + & \cdots & + & a_{2n}x_n & = & b_2\\
	&  &  &  &  &  &  & \vdots & \\
a_{m1}x_1 & + & a_{m2}x_2 & + & \cdots & + & a_{mn}x_n & = & b_m\\
\end{array}\right.
\qquad\longleftrightarrow\qquad
\left(\begin{array}{cccc|c}
a_{11} & a_{12} & \cdots  & a_{1n} & b_1 \\
a_{21} & a_{22} & \cdots  & a_{2n} & b_2 \\
\vdots  & \vdots  & \ddots  & \vdots  & \vdots \\
a_{m1} & a_{m2} & \cdots  & a_{mn} & b_m \\
\end{array}\right)
$$ 

y se denota $(A|b)$. Por ejemplo,

$$
\left\{
\begin{array}{rrrrr}
	x_1 & -2x_2 & + x_3 & = & 7\\
2x_1 & -5x_2 & +2x_3 & = & 6\\
3x_1 &  2x_2 & - x_3 & = & 1\\
\end{array}\right.
\qquad\longleftrightarrow\qquad
\left(
\begin{array}{ccc|c}
1 & -2 &  1 & 7 \\
2 & -5 &  2 & 6 \\
3 &  2 & -1 & 1 \\
\end{array}\right)=(A|b)
$$
$$A=\left(
\begin{array}{ccc}
1 & -2 &  1 \\
2 & -5 &  2 \\
3 &  2 & -1 \\
\end{array}\right)\qquad\qquad\qquad
b=\left(
\begin{array}{c}
7 \\
6 \\
1 \\
\end{array}\right)$$