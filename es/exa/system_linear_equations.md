La expresión

$$2x_1+3x_2+4x_3=24$$

es una ecuación lineal, con coeficientes $a_1=2$, $a_2=3$, $a_3=4$ y término independiente $b=24$. Cuando hay pocas incógnitas, es normal llamarlas $x$, $y$, $z$, $t$... simplemente para evitar muchos subíndices

$$2x+3y+4z=24$$

Por ejemplo, $(x=1,y=2,z=4)$ es una solución de esta ecuación lineal, porque al remplazar las incógnitas por estos valores, la igualdad se cumple

$$2\cdot 1+3\cdot 2+4\cdot 4=24$$

$(x=10,y=-8,z=7)$ también es solución

$$2\cdot 10+3\cdot (-8)+4\cdot 7=24$$

pero $(x=1,y=1,z=1)$ no es solución

$$2\cdot 1+3\cdot 1+4\cdot 1= 9 \neq 24$$

es decir, algunas combinaciones son soluciones pero otras no. Nos gustaría encontrar _todas_ las soluciones

Ahora añadimos una segunda ecuación

$$
\left\{
\begin{array}{rcl}
2x+3y+4z & = & 24\\
7x+y-3z  & = & -5\\
\end{array}\right.
$$

y así tenemos un sistema de ecuaciones lineales. Para este sistema, nuestra primera combinación $(x=1,y=2,z=4)$ sigue siendo solución:

$$
\left\{
\begin{array}{rcl}
2\cdot 1+3\cdot 2+4\cdot 4 & = & 24\\
7\cdot 1+1\cdot 2-3\cdot 4 & = & -5\\
\end{array}\right.
$$

pero la segunda combinación $(x=10,y=-8,z=7)$ ya no es solución

$$
\left\{
\begin{array}{rcl}
2\cdot 10+3\cdot (-8)+4\cdot 7 & = & 24\\
7\cdot 10+1\cdot (-8)-3\cdot 7 & = & 41\neq -5\\
\end{array}\right.
$$

A ver, tiene sentido: cuantas más ecuaciones se tienen que cumplir, menos soluciones encontramos. Y como decíamos antes, queremos encontrar _todas_ las soluciones - ¿Y eso cómo lo hacemos?