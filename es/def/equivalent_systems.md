Dos sistemas de ecuaciones lineales son **equivalentes** si tienen exactamente las mismas soluciones. Por ejemplo 

$$
\left\{
\begin{array}{rrrrr}
x_1 & -2x_2 & + x_3 & = & 7\\
2x_1 & -5x_2 & +2x_3 & = & 6\\
3x_1 &  2x_2 & - x_3 & = & 1\\
\end{array}\right.
\qquad\qquad
\left\{
\begin{array}{rrrrr}
2x_1 & -5x_2 & +2x_3 & = & 6\\
x_1 & -2x_2 & + x_3 & = & 7\\
3x_1 &  2x_2 & - x_3 & = & 1\\
\end{array}\right.
$$

son equivalentes, porque simplemente hemos intercambiado las dos primeras filas, y los requisitos a cumplir son los mismos. Por otro lado, 

$$
\left\{
\begin{array}{rrrrr}
x_1 & -2x_2 & + x_3 & = & 7\\
2x_1 & -5x_2 & +2x_3 & = & 6\\
3x_1 &  2x_2 & - x_3 & = & 1\\
\end{array}\right.
\qquad\qquad
\left\{
\begin{array}{rrrrr}
x &  &  & = & 2\\
& y &  & = & 8\\
&  & z & = & 21\\
\end{array}\right.
$$

también son equivalentes (y por tanto ambos sistemas tienen una sola solución $(x=2,y=8,z=21)$), pero esto no es tan obvio a simple vista

Nuestra estrategia para resolver sistemas lineales será obtener sistemas equivalentes cada vez más simples, hasta que lleguemos a un sistema cuyas soluciones se puedan encontrar directamente