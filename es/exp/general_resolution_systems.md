Nuestro estudio de la [eliminación gaussiana]( thm | gaussian_elimination ) y la [forma canónica por filas]( thm | row_canonical_form ) nos da un método para resolver sistemas de ecuaciones lineales

En primer lugar, es más cómodo trabajar con la matriz asociada al sistema

$$
\left\{
\begin{array}{rrrrrrrcl}
a_{11}x_1 & + & a_{12}x_2 & + & \cdots & + & a_{1n}x_n & = & b_1\\
a_{21}x_1 & + & a_{22}x_2 & + & \cdots & + & a_{2n}x_n & = & b_2\\
  &  &  &  &  &  &  & \vdots & \\
a_{m1}x_1 & + & a_{m2}x_2 & + & \cdots & + & a_{mn}x_n & = & b_m\\
\end{array}\right.
\qquad\leadsto\qquad
\left(\begin{array}{cccc|c}
a_{11} & a_{12} & \cdots  & a_{1n} & b_1 \\
a_{21} & a_{22} & \cdots  & a_{2n} & b_2 \\
\vdots  & \vdots  & \ddots  & \vdots  & \vdots \\
a_{m1} & a_{m2} & \cdots  & a_{mn} & b_m \\
\end{array}\right)
$$

En esta matriz efectuamos operaciones elementales hasta que llegamos a su forma reducida por filas. Sabemos que las operaciones elementales no modifican el conjunto de soluciones, ¡esto es lo importante!

$$
\left(
\begin{array}{cccccccc|c}
 1      & \times & \cdot  & \cdot  & \times & \times & \cdot  & \cdot  & \times \\
 \cdot  & \cdot  & 1      & \cdot  & \times & \times & \cdot  & \cdot  & \times \\
 \cdot  & \cdot  & \cdot  & 1      & \times & \times & \cdot  & \cdot  & \times \\
 \cdot  & \cdot  & \cdot  & \cdot  & \cdot  & \cdot  & 1      & \cdot  & \times \\
 \cdot  & \cdot  & \cdot  & \cdot  & \cdot  & \cdot  & \cdot  & 1      & \times \\
 \cdot  & \cdot  & \cdot  & \cdot  & \cdot  & \cdot  & \cdot  & \cdot  & \cdot  \\
\end{array}
\right)
$$

Las últimas filas son las más simples: por eso tenemos que analizar el sistema desde las últimas filas hacia arriba

<ol>
  <li>
  Una fila llena de ceros

  $$
  \left(
  \begin{array}{cccccccc|c}
  0  & 0  & 0  & 0  & 0  & 0  & 0  & 0  & 0  \\
  \end{array}
  \right)
  $$

  representa la ecuación

  $$0\cdot x_1 + 0\cdot x_2 + \cdots + 0\cdot x_n = 0$$

  que esencialmente no dice nada. Ignoramos tales filas
  </li>
  <li>
  Una fila con un pivote justo al final

  $$
  \left(
  \begin{array}{cccccccc|c}
  0  & 0  & 0  & 0  & 0  & 0  & 0  & 0  & 1  \\
  \end{array}
  \right)
  $$

  representa la ecuación

  $$0\cdot x_1 + 0\cdot x_2 + \cdots + 0\cdot x_n = 1$$

  que ¡es imposible! Si nos encontramos con una fila así, nuestro sistema es **incompatible**
  </li>
  <li>
  Si no nos encontramos estas filas imposibles, nuestro sistema será **compatible**. Para entender por qué, ten en cuenta que cada una de las otras filas encima tiene un pivote. Si hay tantos pivotes como incógnitas, entonces la forma canónica reducida (después de quitar filas de ceros) será algo como

  $$
  \left(\begin{array}{cccc|c}
  1      & \cdot  & \cdots  & \cdot  & b_1' \\
  \cdot  & 1      & \cdots  & \cdot  & b_2' \\
  \vdots & \vdots & \ddots  & \vdots & \vdots \\
  \cdot  & \cdot  & \cdots  & 1      & b_n' \\
  \end{array}\right)
  $$

  para algunos coeficientes alterados $b_i'$, que representa el sistema

  $$
  \left\{
  \begin{array}{rrrrrrrcl}
  x_1 & + & 0\cdot x_2 & + & \cdots & + & 0\cdot x_n & = & b_1'\\
  0\cdot x_1 & + & x_2 & + & \cdots & + & 0\cdot x_n & = & b_2'\\
    &  &  &  &  &  &  & \vdots & \\
  0\cdot x_1 & + & 0\cdot x_2 & + & \cdots & + & x_n & = & b_n'\\
  \end{array}\right.
  $$

  que obviamente sólo tiene una solución

  $$
  \begin{array}{rcl}
  x_1 & = & b_1'\\
  x_2 & = & b_2'\\
    & \vdots & \\
  x_n & = & b_n'\\
  \end{array}
  $$

  y que por ello es **determinado**

  Si hay más incógnitas que pivotes, las incógnitas cuya columna no tiene pivote serán _libres_: podemos elegir para ellas el valor que queramos. Una vez que estos valores están fijos, las incógnitas asociadas a un pivote se pueden resolver en términos de las libres. Puesto que podemos _elegir_, hay muchas soluciones, y el sistema es **indeterminado**. Por ejemplo, la matriz

  $$
  \left(
  \begin{array}{cccccccc|c}
  1      & 8      & \cdot  & \cdot  & -6     & 1      & \cdot  & \cdot  & 7 \\
  \cdot  & \cdot  & 1      & \cdot  & 0      & -4     & \cdot  & \cdot  & 3 \\
  \cdot  & \cdot  & \cdot  & 1      & 5      & 2      & \cdot  & \cdot  & 9 \\
  \cdot  & \cdot  & \cdot  & \cdot  & \cdot  & \cdot  & 1      & \cdot  & -4 \\
  \cdot  & \cdot  & \cdot  & \cdot  & \cdot  & \cdot  & \cdot  & 1      & 2 \\
  \end{array}
  \right)
  $$

  representaría el sistema

  $$
  \left\{
  \begin{array}{rrrrrrrrcl}
  x_1 & +8x_2 & & & -6x_5 & +x_6 & & & = & 7\\
  & & x_3 & & +0x_5 & -4x_6 & & & = & 3\\
  & & & x_4 & +5x_5 & +2x_6 & & & = & 9\\
  & & & & & & x_7 & & = & -4\\
  & & & & & & & x_8 & = & 2\\
  \end{array}\right.
  $$

  $x_2$, $x_5$ y $x_6$ son libres y se les puede dar cualquier valor de $\K$; las otras variables se resuelven en términos de las primeras

  $$
  \begin{array}{rcl}
  x_2 & \in & \K\\
  x_5 & \in & \K\\
  x_6 & \in & \K\\
  x_1 & =   & 7-8x_2+6x_5-x_6\\
  x_3 & =   & 3+4x_6\\
  x_4 & =   & 9-5x_5-2x_6\\
  x_7 & =   & -4\\
  x_8 & =   & 2\\
  \end{array}
  $$
  </li>
</ol>

La compatibilidad y determinación del sistema $(A|b)$ se encuentra según el número de filas no nulas de la forma canónica por filas de $A$ y $(A|b)$ - este número tiene un nombre especial, el _rango_, y esta discusión también tiene un nombre especial, el _Teorema de Rouché-Frobenius_