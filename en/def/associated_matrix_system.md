For the sake of commodity, from now on each linear system will have an **associated matrix**. For now, we may think a matrix as a box of numbers; it has of course a deep meaning that will be studied later

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

and it is denoted $(A|b)$. For instance,

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