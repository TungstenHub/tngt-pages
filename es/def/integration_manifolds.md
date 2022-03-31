Supongamos que tenemos una variedad orientada $M$. Entonces deberíamos ser capaces de definir la integración de formas de modo riguroso...

{{ image | integration_manifolds_sum width = 480 }}

Empecemos con $\R^n$

Una forma de orden maximal en $\R^n$ es del tipo $\alpha=f(x_1,x_2,...,x_n)\d x_1\wedge\d x_2\wedge...\wedge\d x_n$. Como $\d x_1\wedge\d x_2\wedge...\wedge\d x_n$ es el volumen estándar al evaluarse en una base positiva, parece natural definir

$$
\int_{\R ^n}\alpha=\int_{\R ^n}f(x_1,x_2,...,x_n)\d x_1\wedge\d x_2\wedge...\wedge\d x_n=\int_{\R ^n}f(x_1,x_2,...,x_n)\d x_1\d x_2...\d x_n,
$$

donde la última integral es la estándar de $\R^n$. Para evitar problemas de convergencia, requeriremos que $f$ tenga soporte compacto, es decir, $\alpha\in\Omega^n_c(\R ^n)$.

Por otra parte, supongamos que tenemos una forma de orden maximal $\alpha$ en una variedad orientada $M$ y que $\varphi:U\longrightarrow M$ es una carta positiva. En $U\subset \R^n$ tenemos la $n$-forma $\varphi^*\alpha$; ésta última se define como para mantener la valoración de $\alpha$, por lo que es razonable que $\int_U \varphi^*\alpha=\int_{\varphi(U)}\alpha$. Esto debería ser suficiente para integrar sobre $M$, puesto que sabemos cómo hacerlo localmente

{{ image | integration_manifolds_euclidean_chart }}

>>>
Sea $M$ una variedad orientada de dimensión $n$. Existe una única aplicación lineal

$$\int_M:\Omega^n_c(M)\longrightarrow \R$$

satisfaciendo la siguiente propiedad: si $\varphi:U\longrightarrow M$ es una carta positivamente orientada y el soporte de $\alpha\in\Omega^n_c(M)$ está contenido en $\varphi(U)$, entonces $\int_M\alpha=\int_U \varphi^*\alpha$.

Si $\{\varphi_i:U_i\longrightarrow M\}$ es una colección de cartas cubriendo $M$ y $\{\rho_i\}$ es una partición de la unidad asociada a los abiertos $\{\varphi_i(U_i)\}$, entonces se cumple que $\int_M\alpha=\sum_i \int_{U_i}\varphi_i^*(\rho_i\alpha)$.
<<<

La validez de estas afirmaciones previas reside en última instancia en probar que la última expresión es independiente de las cartas y la partición de la unidad elegidas. Por ahora, nos limitaremos a comprobar el hecho clave: que $\int_M\alpha=\int_U \varphi^*\alpha$ se cumple al considerar difeomorfismos entre abiertos de $\R^n$, teniendo en mente que aquí aplica la integral usual

Sea $\varphi:U\longrightarrow V$ un difeomorfismo positivamente orientado entre abiertos de $\R^n$ y $\alpha=f(y)\d y_1\wedge...\wedge\d y_n$ una $n$-forma en $V$. Entonces

$$
\begin{array}{rcl}
\varphi^*(f(y)\d y_1\wedge...\wedge\d y_n) & = & (f\circ \varphi)\d(\varphi_1)\wedge...\wedge \d(\varphi_n)\\\\
& = & (f\circ \varphi)\left(\sum \dfrac{\partial \varphi_1}{\partial x_j}\d x_j\right)\wedge...\wedge\left(\sum \dfrac{\partial \varphi_n}{\partial x_j}\d x_j\right)\\\\
& = & (f\circ \varphi)\text{Det}\left(\dfrac{\partial \varphi_i}{\partial x_j}\right)\d x_1\wedge...\wedge\d x_n,
\end{array}
$$

apareciendo el determinante debido a la antisimetría del producto wedge. El Teorema de Cambio de Variables asegura que

$$
\int_V\alpha=\int_V f\d y=\int_U (f\circ \varphi)\left|\text{Det}\left(\dfrac{\partial \varphi_i}{\partial x_j}\right)\right|\d x=\int_U (f\circ \varphi)\text{Det}\left(\dfrac{\partial \varphi_i}{\partial x_j}\right)\d x=\int_U\varphi^*\alpha,
$$

porque $\varphi$ es un difeomorfismo positivamente orientado y por tanto el determinante de la matriz jacobiana es positivo

Dos apuntes más:

<ol>
<li>Si cambiamos la orientación de $M$ (las bases positivas se vuelven negativas y viceversa), todas las integrales quedan multiplicadas por $-1$</li>
<li>Si $f:M\longrightarrow N$ es un difeomorfismo positivamente orientado, entonces $ \int_N\alpha=\int_M f^*\alpha$ para toda $\alpha\in\Omega^n_c(N)$</li>
</ol>