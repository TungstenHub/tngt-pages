¿Qué podemos hacer para obtener sistemas equivalentes? Hay pequeños trucos. Obviamente intercambiar dos filas siempre da pie a un sistema equivalente. También hay otro truco que es bastante simple. Si tenemos una ecuación, digamos

$$2x-y+5z=8$$

la podemos multiplicar por otro número, por ejemplo $3$, y nos queda una ecuación equivalente

$$6x-3y+15z=24$$

Cualquier combinación de $x$, $y$ y $z$ que cumpla la primera ecuación (es decir, una solución) también cumplirá la segunda ecuación. ¡Pero cuidado! _No podemos multiplicar por $0$_. Si lo hiciéramos, tendríamos

$$0x+0y+0z=0$$

y _todas_ las combinaciones de $x$, $y$ y $z$ lo cumplirían. La nueva ecuación tiene muchas más soluciones que la original, por lo que no son equivalentes. En cierto sentido, la equivalencia tiene que ver con la reversibilidad: multiplicar por un número mantiene la implicación válida

$$2x-y+5z=8\Longrightarrow 6x-3y+15z=24$$
$$2x-y+5z=8\Longrightarrow 0x+0y+0z=0$$

pero mientras que la primera implicación se puede revertir al multiplicar por $\frac{1}{3}$, la segunda no se puede revertir

$$6x-3y+15z=24\Longrightarrow 2x-y+5z=8$$
$$0x+0y+0z=0\kern.4em\not\kern -.4em \Longrightarrow 2x-y+5z=8$$

así que

$$2x-y+5z=8\Longleftrightarrow 6x-3y+15z=24$$
$$2x-y+5z=8\kern.6em\not\kern -.6em \Longleftrightarrow 0x+0y+0z=0$$

Un último truco es combinar dos ecuaciones de modo adecuado... Supongamos que uno tiene un par de ecuaciones (entre otras cuantas):

$$
\left\{
\begin{array}{rcl}
2x+3y+4z & = & 24\\
7x+4y+4z & = & 11\\
\end{array}\right.
$$

Si las dos ecuaciones se tienen que cumplir... ¡la ecuación generada al sumar ambas también se tiene que satisfacer!

$$(2x+3y+4z)+(7x+4y+4z)=24+11$$
$$9x+7y+8z=35$$

Esta ecuación sola no es tan restrictiva como las dos iniciales juntas... pero basta con incluir al menos alguna de las ecuaciones originales

$$
\left\{
\begin{array}{rcl}
2x+3y+4z & = & 24\\
7x+4y+4z & = & 11\\
\end{array}\right.
\qquad \Longleftrightarrow \qquad
\left\{
\begin{array}{rcl}
2x+3y+4z & = & 24\\
9x+7y+8z & = & 35\\
\end{array}\right.
$$

justo porque uno puede volver atrás con el mismo truco, pero restando en vez de sumando. Y esto funciona si añadimos cualquier múltiplo de la primera ecuación a la segunda ecuación

$$
\left\{
\begin{array}{rcl}
2x+3y+4z & = & 24\\
7x+4y+4z & = & 11\\
\end{array}\right.
\qquad \Longleftrightarrow \qquad
\left\{
\begin{array}{rcl}
2x+3y+4z & = & 24\\
7x+4y+4z + k(2x+3y+4z) & = & 11+24k\\
\end{array}\right.
$$

Aquí $k$ puede ser cualquier número, ¡incluso cero! Sólo que para  $k=0$ en realidad no estamos haciendo nada

Estos trucos son tan habituales que tienen un nombre especial: **operaciones elementales (por filas)**