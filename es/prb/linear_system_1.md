Transformar el siguiente sistema de ecuaciones lineales en un sistema escalonado, discutirlo y resolverlo si tiene solución

$$
\left\{
\begin{array}{rrrrr}
 x_1 & -2x_2 & + x_3 & = & 7\\
2x_1 & -5x_2 & +2x_3 & = & 6\\
3x_1 &  2x_2 & - x_3 & = & 1\\
\end{array}\right.
$$

+++
Solución
+++

El sistema tiene matriz ampliada

$$
(A|b)=
\left(
\begin{array}{ccc|c}
 1 & -2 &  1 & 7 \\
 2 & -5 &  2 & 6 \\
 3 &  2 & -1 & 1 \\
\end{array}\right)
$$

en la que hacemos transformaciones elementales por filas

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

Así pues el sistema de partida es equivalente al sistema

$$
\left\{
\begin{array}{rrrrr}
 x_1 &       &       & = & 2\\
     &   x_2 &       & = & 8\\
     &       &   x_3 & = & 21\\
\end{array}\right.
$$

que es **compatible determinado** con solución $x_1=2$, $x_2=8$ and $x_3=21$. Por último, comprobemos que la solución efectivamente resuelve el sistema

$$
\left\{
\begin{array}{rrrrrrr}
 2       & -2\cdot 8 & + 21       & = & 2-16+21 & = & 7\\
2\cdot 2 & -5\cdot 8 & +2\cdot 21 & = & 4-40+42 & = & 6\\
3\cdot 2 &  2\cdot 8 & - 21       & = & 6+16-21 & = & 1\\
\end{array}\right.
$$

+++