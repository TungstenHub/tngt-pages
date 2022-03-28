Transform the following system of linear equations in a row echelon form, discuss and solve if having solutions

$$
\left\{
\begin{array}{rrrrr}
 x_1 & -2x_2 & + x_3 & = & 7\\
2x_1 & -5x_2 & +2x_3 & = & 6\\
3x_1 &  2x_2 & - x_3 & = & 1\\
\end{array}\right.
$$

+++
Solution
+++

The system has the following augmented matrix

$$
(A|b)=
\left(
\begin{array}{ccc|c}
 1 & -2 &  1 & 7 \\
 2 & -5 &  2 & 6 \\
 3 &  2 & -1 & 1 \\
\end{array}\right)
$$

on which we perform elementary row transformations

$$
\left(
\begin{array}{ccc|c}
 1 & -2 &  1 & 7 \\
 2 & -5 &  2 & 6 \\
 3 &  2 & -1 & 1 \\
\end{array}\right)\simeq_f
\left(
\begin{array}{ccc|c}
 1 & -2 &  1 & 7 \\
 0 & -1 &  0 & -8 \\
 0 &  8 & -4 & -20 \\
\end{array}\right)\simeq_f
\left(
\begin{array}{ccc|c}
 1 & -2 &  1 & 7 \\
 0 & -1 &  0 & -8 \\
 0 &  0 & -4 & -84 \\
\end{array}\right)\simeq_f$$
$$\simeq_f
\left(
\begin{array}{ccc|c}
 1 & -2 &  1 & 7 \\
 0 &  1 &  0 & 8 \\
 0 &  0 &  1 & 21 \\
\end{array}\right)\simeq_f
\left(
\begin{array}{ccc|c}
 1 &  0 &  1 & 23 \\
 0 &  1 &  0 & 8 \\
 0 &  0 &  1 & 21 \\
\end{array}\right)\simeq_f
\left(
\begin{array}{ccc|c}
 1 &  0 &  0 & 2 \\
 0 &  1 &  0 & 8 \\
 0 &  0 &  1 & 21 \\
\end{array}\right)
$$

So our system is equivalent to the following one

$$
\left\{
\begin{array}{rrrrr}
 x_1 &       &       & = & 2\\
     &   x_2 &       & = & 8\\
     &       &   x_3 & = & 21\\
\end{array}\right.
$$

that is **determinate compatible** with solution $x_1=2$, $x_2=8$ and $x_3=21$. Lastly, let's check that these values indeed constitute a solution

$$
\left\{
\begin{array}{rrrrrrr}
 2       & -2\cdot 8 & + 21       & = & 2-16+21 & = & 7\\
2\cdot 2 & -5\cdot 8 & +2\cdot 21 & = & 4-40+42 & = & 6\\
3\cdot 2 &  2\cdot 8 & - 21       & = & 6+16-21 & = & 1\\
\end{array}\right.
$$

+++