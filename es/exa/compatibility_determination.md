El sistema (de una sola ecuación)

$$
\left\{
\begin{array}{rcl}
2x+3y+4z & = & 24\\
\end{array}\right.
$$

es compatible e indeterminado, porque tiene montones de soluciones. De hecho, dale a $x$ e $y$ los valores que quieras, y resuelve $z$. Si elegimos $x=3$ e $y=1$, entonces

$$2x+3y+4z = 2\cdot 3+3\cdot 1 +4z = 24\Longrightarrow 4z=15\Longrightarrow z=\dfrac{15}{4}$$

y $\left(x=3,y=1,z=\frac{15}{4}\right)$ es una solución. Si en cambio elegimos $x=0$ e $y=0$, entonces

$$2x+3y+4z = 2\cdot 0+3\cdot 0 +4z = 24\Longrightarrow 4z=24\Longrightarrow z=6$$

y $(x=0,y=0,z=6)$ es una solución. ¿Ves? Mogollón de soluciones

---

El sistema

$$
\left\{
\begin{array}{rcl}
2x+3y+4z & = & 24\\
7x+4y+4z & = & 11\\
\end{array}\right.
$$

también es compatible e indeterminado. Pero ya no es tan holgado. Podemos elegir el valor que queramos para $x$, pero una vez que hemos elegido aquí, ya no podemos seguir eligiendo. ¿Por qué? Bueno, cuando el valor de $x$ está fijo, se nos queda algo como

$$
\left\{
\begin{array}{rcl}
3y+4z & = & a\\
4y+4z & = & b\\
\end{array}\right.
$$

para algunos valores $a$ y $b$. ¡Pero la segunda fila es exactamente una $y$ mayor que la primera fila! Con lo que $y$ es necesariamente $b-a$. Y $z$ se determinaría acto seguido. De nuevo muchas soluciones, pero _menos_ que en el ejemplo anterior

---

El sistema

$$
\left\{
\begin{array}{rcl}
2x+3y+4z & = & 24\\
2x+3y+4z & = & 27\\
\end{array}\right.
$$

es incompatible: ¡no puede ser que $2x+3y+4z = 24$ y $2x+3y+4z = 27$ a la vez! Sin embargo, el prototipo ("ejemplo mínimo") de ecuación incompatible es

$$
\left\{
\begin{array}{rcl}
0x+0y+0z & = & 1\\
\end{array}\right.
$$

Qué triste, ¿no?

---

El sistema

$$
\left\{
\begin{array}{rrrrr}
x & -2y & + z & = & 7\\
2x & -5y & +2z & = & 6\\
3x &  2y & - z & = & 1\\
\end{array}\right.
$$

tiene exactamente una solución, $(x=2,y=8,z=21)$, y por tanto es compatible y determinado. ¿Pero cómo sabemos esto? Lo vamos a estudiar en más detalle. Por otra parte, un sistema que sería súper fácil de clasificar como compatible y determinado es

$$
\left\{
\begin{array}{rrrrr}
x &  &  & = & 2\\
 & y &  & = & 8\\
 &  & z & = & 21\\
\end{array}\right.
$$

Puede parecer una estupidez prestar atención a este tipo de sistemas... ¡pero no lo es! Y la razón es que para resolver el primer sistema, vamos a tener que transformarlo de alguna manera en el segundo

$$
\left\{
\begin{array}{rrrrr}
x & -2y & + z & = & 7\\
2x & -5y & +2z & = & 6\\
3x &  2y & - z & = & 1\\
\end{array}\right.
\qquad\leadsto\qquad
\left\{
\begin{array}{rrrrr}
x &  &  & = & 2\\
 & y &  & = & 8\\
 &  & z & = & 21\\
\end{array}\right.
$$

que ya se resuelve directamente. Así que... ¿preparado para saber más?