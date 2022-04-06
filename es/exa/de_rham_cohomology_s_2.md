Este caso es notablemente más complejo que los anteriores. Parte de las ideas de este ejemplo se estudiarán extensivamente en los Lemas de Poincaré y en las Secuencias de Mayer-Vietoris

Consideramos la esfera $\S^2\subset\R^3$ junto con las dos parametrizaciones dadas por la proyección estereográfica desde los polos $N=(0,0,1)$ y $S=(0,0,-1)$. Los dominios de estas parametrizaciones son $\R^2$, y las imágenes son los abiertos $U=\S^2-\{N\}$, $V=\S^2-\{S\}$; sea $W=U\cap V=\S^2-\{N,S\}$

---

Sea $f\in C^\infty(\S^2)$ con $\d f=0$. $f$ induce las restricciones $f_1=f|_U$, $f_2=f|_V$, que se identifican con funciones de dominio $\R^2$. Según se vio en [la cohomología de $\R^2$]( exa | de_rham_cohomology_r_2 ), $\d f_1=0$ y $\d f_2=0$ implican que $f_1$ y $f_2$ son constantes, y como han de coincidir en el dominio común $W$, $f$ debe ser constante

$$H^0(\S^2)=\dfrac{\text{ker }\d_0}{\text{im }\d_{-1}}=\dfrac{\{f=cte\in\R\}}{0}\simeq\R$$

---

Sea ahora $\alpha$ una 1-forma en $S^2$ con $\d\alpha=0$. La restricción de $\alpha$ a $U$, $V$ nos da las 1-formas $\alpha_1$ y $\alpha_2$, cuyas diferenciales exteriores son también nulas. Como $H^1(\R^2)=0$, las 1-formas cerradas son exactas y existen funciones $f_1$ y $f_2$ en $U$, $V$ con $\d f_1=\alpha_1$, $\d f_2=\alpha_2$. ¿Son compatibles $f_1$ y $f_2$ en $W$? Hacemos un truco: en $W$, $\d(f_1-f_2)=\d f_1-\d f_2=\alpha_1-\alpha_2=\alpha-\alpha=0$. Como la diferencial de la función $f_1-f_2$ es 0 en $W$ y $W$ es conexo, esto implica que $f_1-f_2$ es una cierta constante $c\in\R$. Así, podemos redefinir $\tilde{f}_2=f_2+c$, lo cual no cambia que $\d \tilde{f}_2=\alpha_2$, y ahora $f_1=\tilde{f}_2$ en $W$, por lo que tomamos la función global

$$f=
\begin{cases}
f_1 & \text{en $U$}\\
\tilde{f}_2 & \text{en $V$}
\end{cases}$$

Esta función cumple $\d f=\alpha$, pues lo cumple en $U$, $V$. De modo que

$$H^1(\S^2)=\dfrac{\text{ker }\d_1}{\text{im }\d_0}=0$$

---

Vamos a la parte delicada. Sea $\beta$ una 2-forma en $\S^2$. Por estar definida en una variedad de dimensión 2, su diferencial exterior es 0, y lo mismo ocurre en $\beta_1=\beta|_U$ y $\beta_2=\beta|_V$. Al ser $H^2(\R^2)=0$, existen 1-formas $\alpha_1$, $\alpha_2$ definidas en $U$, $V$ con $\d \alpha_i=\beta_i$. De nuevo, ¿cómo interactúan $\alpha_1$ y $\alpha_2$ en el dominio común $W$? $\d(\alpha_1-\alpha_2)=\d\alpha_1-\d\alpha_2=\beta_1-\beta_2=\beta-\beta=0$. Pero como no conocemos el primer grupo de cohomología de $W$, no podemos decir nada sobre sus 1-formas cerradas. Así que vamos a estudiar la cohomología de $W$ brevemente

Consideramos la parametrización de $W$ $(\theta,z)\longmapsto(\sqrt{1-z^2}\cos(\theta),\sqrt{1-z^2}\sin(\theta),z)$, $(\theta,z)\in\R\times(-1,1)$. Ésta induce las 1-formas $\d \theta$, $\d z$, y las funciones $C^\infty(W)$ están en biyección con las funciones $f(\theta,z)$ diferenciables y $2\pi$-periódicas en $\theta$, que a su vez admiten el desarrollo en serie de Fourier $f(\theta,z)=\sum_{n}f_{n}(z)\ee^{\ii n\theta}$.

Sea $\alpha=g\d \theta+h\d z$

$$\d \alpha=\left(\dfrac{\partial h}{\partial \theta}-\dfrac{\partial g}{\partial z}\right)\d \theta\wedge\d z=\sum_{n}(\ii nh_n(z)-g_n'(z))\ee^{\ii n\theta}\d \theta\wedge\d z$$

y para que $\alpha$ sea cerrada, se requiere $\ii nh_n(z)=g_n'(z)$ para todo $n$. Ahora buscamos $f=\sum_{n}f_{n}(z)\ee^{\ii n\theta}$ con $\d f=\alpha$, es decir, $\dfrac{\partial f}{\partial \theta}=g$, $\dfrac{\partial f}{\partial z}=h$, o lo que es lo mismo, $\ii nf_n(z)=g_n(z)$, $f_n'(z)=h_n(z)$. Si $n\neq 0$, no hay ningún problema en tomar $f_n(z)=\frac{g_n(z)}{\ii n}$ y todo funciona bien, pues $f_n'(z)=\frac{g_n'(z)}{\ii n}=\frac{\ii nh_n(z)}{\ii n}=h_n(z)$. Para $n=0$, $\ii 0h_0(z)=g_0'(z)$ se cumple cuando $g_0=c\in\R$ constante. Pero si $c\neq 0$, la condición $\ii 0f_0(z)=g_0(z)=c$ es imposible de cumplir. Por otro lado, es el único impedimento, pues si corregimos $g$ con $c=0$, entonces basta tomar $f_0(z)=\int_0^{z} h_0(t)\d t$. Así, $H^1(W)\simeq\R$, dependiente de la elección de $c$, y un generador del grupo es la clase de la 1-forma $\d \theta$, que a partir de ahora se denotará por $\gamma$

Ya hemos estudiado parte de la cohomología de $W$. Teníamos $\d(\alpha_1-\alpha_2)=0$; por lo que acabamos de ver, $\alpha_1-\alpha_2=\lambda\gamma+\d f$ para un cierto $\lambda\in\R $ y una cierta función $f$ en $W$. Supongamos por un momento que $\lambda=0$ y vamos a comprobar que, en ese caso, somos capaces de encontrar un $\alpha$ global con $\d \alpha=\beta$. Pero antes necesitamos introducir dos funciones _de soporte compacto_

Elegimos $\rho_1$ y $\rho_2$ funciones positivas definidas en $[-1,1]$ tal que $\rho_1$ se anula en $[1/3,1]$, $\rho_2$ se anula en $[-1,-1/3]$ y $\rho_1+\rho_2=1$. Al aplicar estas funciones a la altura de la esfera obtenemos otras dos funciones (que seguiremos llamando $\rho_1$ y $\rho_2$) tal que la primera tiene su soporte contenido en $U$ y la segunda en $V$, es decir, $\{\rho_1,\rho_2\}$ es una partición diferenciable de la unidad subordinada a $\{U,V\}$

{{ image | compact_support_functions }}

¿Esto por qué es útil? Por razones de extensibilidad. La función $f$ puede no ser extensible a los polos, pero se puede arreglar con nuestras funciones. Si definimos $f_1=f\rho_2$ y $f_2=f\rho_1$ (obsérvese el cambio de índices) y extendemos por la función nula, entonces $f_1$ es una función diferenciable en $U$, $f_2$ es una función diferenciable en $V$ y $f_1+f_2=f$ en $W$

{{ image | compact_support_transformation }}

¡Genial! Ahora redefinimos $\tilde{\alpha}_1=\alpha_1-\d f_1$, $\tilde{\alpha}_2=\alpha_2+\d f_2$. Se sigue teniendo $\d \tilde{\alpha}_1=\beta_1$ y $\d \tilde{\alpha}_2=\beta_2$, pero ahora $\tilde{\alpha}_1-\tilde{\alpha}_2=\alpha_1-\d f_1-\alpha_2-\d f_2=\d f-\d(f_1+f_2)=0$ en $W$. Como hay coincidencia en el dominio común, definimos

$$\alpha=
\begin{cases}
\tilde{\alpha}_1 & \text{en $U$}\\
\tilde{\alpha}_2 & \text{en $V$}
\end{cases}$$

y es cierto que $\d \alpha=\beta$ en $\S^2$. Es decir, $\alpha_1$ y $\alpha_2$ podían ser no extensibles, pero en nuestra corrección hemos conseguido quitar esta no-extensibilidad

Si $\lambda\neq 0$, este proceso es imposible: si tenemos $\alpha$ global

$$
\begin{array}{rl}
\d(\alpha-\alpha_1)=\beta-\beta_1=0 \Longrightarrow \alpha-\alpha_1=\d f_1 & \qquad\text{en $U$, para alguna $f_1$} \\
\d(\alpha-\alpha_2)=\beta-\beta_2=0 \Longrightarrow \alpha-\alpha_2=\d f_2 & \qquad\text{en $V$, para alguna $f_2$} \\
\alpha_1-\alpha_2=\alpha-\d f_1 -\alpha+\d f_2=\d (f_2-f_1) & \qquad\text{en $W$} \\
\end{array}
$$

pero teníamos $\alpha_1-\alpha_2=\lambda\gamma+\d f$, y sabemos que $\gamma$ no es la diferencial de ninguna función

Para terminar de establecer que en la esfera hay 2-formas cerradas y no exactas, debemos encontrar un $\beta$ para el cual, con los $\alpha_i$ inducidos, se tenga $\alpha_1-\alpha_2=\lambda\gamma+\d f$ con $\lambda\neq 0$. Tomamos $\beta_1=\d(\rho_2\gamma)$, $\beta_2=\d(\rho_1\gamma)$. En $W$,

$$\beta_1+\beta_2=\d(\rho_2\gamma+\rho_1\gamma)=\d \gamma=0$$

y así tenemos

$$\beta=
\begin{cases}
\beta_1 & \text{en $U$}\\
-\beta_2 & \text{en $V$}
\end{cases}$$ 

Las 1-formas inducidas son, salvo la diferencial de una función, $\alpha_1=\rho_2\gamma$ y $\alpha_2=-\rho_1\gamma$, y 

$$\alpha_1-\alpha_2=(\rho_2+\rho_1)\gamma=\gamma\leadsto\lambda=1$$

Ahora podemos asegurar que

$$H^2(\S^2)=\dfrac{\text{ker }\d_2}{\text{im }\d_1}\simeq\R$$

porque la exactitud de la 2-forma cerrada $\beta$ depende del coeficiente $\lambda$ inducido

---

Un generador explícito de $H^2(\S^2)$ podría se $\d\theta\wedge\d z$, que resulta coincidir con la medida de superficie de la esfera como subconjunto de $\R^3$