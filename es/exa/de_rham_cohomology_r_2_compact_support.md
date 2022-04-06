Las formas diferenciales con soporte compacto en $\R ^2$ y la actuación de $\d$ son como antes, solo que $f$, $g$, $h$ y $k$ son ahora funciones de soporte compacto

---

$\text{ker }\d_0$ vuelve a estar formado por funciones $f$ constantes, pero como ahora se requiere que $f$ sea de soporte compacto, resulta que $\text{ker }\d_0=\{f\equiv 0\}$ y

$$H^0_c(\R ^2)=\dfrac{\{f\equiv 0\}}{0}=0$$

---

Para el siguiente grupo, en un primer momento se propuso la función

$$ f(x,y)=\int_0^x f_x(t,0)\d t+\int_0^y f_y(x,t)\d t=\int_0^x g(t,0)\d t+\int_0^y h(x,t)\d t$$

que cumple $\d f=g\d x+h\d y$, y así todas las 1-formas cerradas son exactas. El problema es que ahora $f$ puede no tener soporte compacto aun cuando $g$ y $h$ sí. Pero esto no es gran dificultad: si $g$ y $h$ se anulan fuera de un conjunto $[-M,M] \times[-M,M]$, entonces ahí también es cierto que

$$\dfrac{\partial f}{\partial x}=g=0$$ 
$$\dfrac{\partial f}{\partial y}=h=0$$

por lo que $f$ es constante en $\R ^2\smallsetminus [-M,M] \times[-M,M]$ (que es conexo). Así, basta redefinir $f$ restándole esa constante para que valga 0 fuera de $[-M,M] \times[-M,M]$. Luego también en el caso con soporte compacto las 1-formas cerradas son exactas y

$$H^1_c(\R ^2)=0$$

---

Aquí viene la mayor diferencia: $H^2_c(\R ^2)$ no es trivial. En el caso no compacto, para la 2-forma $k\d x\wedge\d y$ habíamos tomado 

$$g=0,\qquad h(x,y)=\int_0^x k(t,y)\d t$$

para que $\dfrac{\partial h}{\partial x}-\dfrac{\partial g}{\partial y}=k$, pero ahora es casi imposible que $h$ tenga soporte compacto. ¿Podemos elegir $g$ y $h$ más acertadamente? Pues, de hecho, casi nunca vamos a poder...

La mayor obstrucción es cuando $\int_{\R ^2} k(x,y)\neq 0$. Supongamos que $g$ y $h$ se anulan fuera de un cuadrado $K=[-M,M] \times[-M,M]$ (y sobre el borde). Entonces

$$
\begin{array}{rcl}
\displaystyle\int_{\R ^2} k(x,y)=\int_K k(x,y) & = & \displaystyle\int_{-M}^M \int_{-M}^M \dfrac{\partial h}{\partial x} \d x \d y-\int_{-M}^M \int_{-M}^M \dfrac{\partial g}{\partial y} \d y \d x\\
& = & \displaystyle\int_{-M}^M \bigl[h(x,y)\bigr]_{x=-M}^{x=M}\, \d y-\int_{-M}^M \bigl[g(x,y)\bigr]_{y=-M}^{y=M}\, \d x\\
& = & 0
\end{array}
$$

con lo que si $\int_{\R ^2} k(x,y)\neq 0$ no hay nada que hacer: $k\d x\wedge\d y$ es automáticamente cerrada, pero no es exacta. ¿Y si $\int_{\R ^2} k(x,y)=0$? Intentaremos hacer lo de antes y retocaremos si hace falta. Sea

$$h(x,y)=\int_{-M}^x k(t,y)\d t$$

Arriba, abajo y a la izquierda del cuadrado $h$ se anula, mientras que a la derecha toma los valores de una cierta función $v(y)$ con soporte en $[-M,M]$. Para corregir esta anomalía, tomamos una función diferenciable $\rho(x)$ que valga 0 en $(-\infty,-M]$ y 1 en $[M,\infty)$, y pasamos a la función

$$\tilde{h}(x,y)=h(x,y)-\rho(x)v(y)$$

¡que ahora tiene soporte compacto! Pero este cambio tiene un precio que tendremos que compensar con $g$:

$$\dfrac{\partial \tilde{h}}{\partial x}=\dfrac{\partial h}{\partial x}-\rho'(x)v(y)=k-\rho'(x)v(y)$$

así que necesitamos que $\dfrac{\partial g}{\partial y}=-\rho'(x)v(y)$, que se consigue tomando

$$g(x,y)=\int_{-M}^y -\rho'(x)v(t)\d t=-\rho'(x)\int_{-M}^y v(t)\d t$$

¡Magnífico! $g$ se anula fuera de $K$, también encima, porque

$$\int_{-M}^M v(t)\d t=\int_{\R ^2} k(x,y)=0$$

Como $\int_{\R ^2} k(x,y)$ decide la exactitud de la 2-forma, hay un grado de libertad y

$$H^2_c(\R ^2)\simeq\R $$