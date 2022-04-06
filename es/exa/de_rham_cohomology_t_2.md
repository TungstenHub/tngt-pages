Consideremos ahora el toro $\T^2=\S^1\times\S^1$. De nuevo, el recubrimiento $\R^2\longrightarrow\T^2$, $(\alpha,\beta)\longmapsto(\ee^{\ii\alpha},\ee^{\ii\beta})$ nos proporciona dos 1-formas globales $\d \alpha$, $\d \beta$

<ul>
  <li>0-formas: $f:\R^2\longrightarrow\R$</li>
  <li>1-formas: $g\d \alpha+h\d \beta$</li>
  <li>2-formas: $k\d \alpha\wedge\d \beta$</li>
</ul>

donde todas las funciones que aparecen son diferenciables y $2\pi$-periódicas _en cada variable_. La actuación de $\d$ es la misma que en $\R^2$

---

$$H^0(\T^2)=\dfrac{\text{ker }\d_0}{\text{im }\d_{-1}}=\dfrac{\left\{f\middle|\dfrac{\partial f}{\partial \alpha}=\dfrac{\partial f}{\partial \beta}=0\right\}}{0}=\dfrac{\{f=cte\in\R\}}{0}\simeq\R$$

---

Para los siguientes grupos utilizamos el desarrollo en serie de Fourier de estas funciones periódicas: $f(\alpha,\beta)=\sum_{\substack{m,n=-\infty}}^\infty f_{mn}\ee^{\ii m\alpha}\ee^{\ii n\beta}$, y lo mismo para $g$, $h$ y $k$. Utilizaremos este desarrollo de modo completamente formal, sin incurrir en cuestiones de convergencia, que no alteran la validez de lo que sigue

$$\d (g\d \alpha+h\d\beta)=\left(\dfrac{\partial h}{\partial \alpha}-\dfrac{\partial g}{\partial \beta}\right)\d \alpha\wedge\d\beta=\ii\sum_{mn}(mh_{mn}-ng_{mn})\ee^{\ii m\alpha}\ee^{\ii n\beta}\d \alpha\wedge\d\beta$$

y es igual a 0 si $mh_{mn}=ng_{mn}$ para todo $m$, $n$; por otra parte 

$$\d(f)=\dfrac{\partial f}{\partial \alpha}\d \alpha+\dfrac{\partial f}{\partial \beta}\d \beta=\ii\sum_{mn}mf_{mn}\ee^{\ii m\alpha} \ee^{\ii n\beta} \d\alpha+ \ii\sum_{mn}nf_{mn}\ee^{\ii m\alpha}\ee^{\ii n\beta}\d\beta$$ 

Así pues, dados $g_{mn}$, $h_{mn}$ con $mh_{mn}=ng_{mn}$, buscamos $f_{mn}$ con $g_{mn}=\ii mf_{mn}$, $h_{mn}=\ii nf_{mn}$

Para $m\neq 0$, podemos tomar $f_{mn}=\frac{1}{\ii m}g_{mn}$, y 

$$\ii mf_{mn}=g_{mn},\qquad\ii nf_{mn}=\frac{\ii n}{\ii m}g_{mn}=\frac{1}{m}mh_{mn}=h_{mn}$$

Igualmente, si $n\neq 0$, tomamos $f_{mn}=\frac{1}{\ii n}h_{mn}$. El problema está en $m=n=0$: $0h_{00}=0g_{00}$ se cumple siempre, mientras que $g_{00}=\ii0f_{00}$ y $h_{00}=\ii0f_{00}$ sólo se cumple para $g_{00}=h_{00}=0$. Así, no todas las funciones $g$, $h$ con $\dfrac{\partial h}{\partial \alpha}-\dfrac{\partial g}{\partial \beta}=0$ son del tipo $\dfrac{\partial f}{\partial \alpha}$, $\dfrac{\partial f}{\partial \beta}$; hay que hacer antes la corrección $g_{00}=h_{00}=0$. Por eso,

$$H^1(\T^2)=\dfrac{\left\{g\d\alpha+h\d\beta\middle|\dfrac{\partial h}{\partial \alpha}-\dfrac{\partial g}{\partial \beta}=0\right\}}{\left\{\dfrac{\partial f}{\partial \alpha}\d \alpha+\dfrac{\partial f}{\partial \beta}\d \beta\right\}}\simeq\R^2$$

pues en $g$ y $h$ tenemos dos grados de libertad extra

Dos generadores de $H^1(\T^2)$ son $\d\alpha$ ($g_{00}=1$) y $\d \beta$ ($h_{00}=1$). Como en el caso de la circunferencia, están estrechamente ligados a ciclos no triviales en $H_1(\T^2)$

---

$\d(k\d \alpha\wedge\d\beta)=0$, luego el núcleo de $\d_2$ es todo $\Omega^2(\T^2)$. Por otro lado, 

$$\d (g\d \alpha+h\d\beta)=\ii\sum_{mn}(mh_{mn}-ng_{mn})\ee^{\ii m\alpha}\ee^{\ii n\beta}\d \alpha\wedge\d\beta$$

Nos preguntamos si dados los coeficientes $k_{mn}$ se pueden encontrar $g_{mn}$, $h_{mn}$ con $\ii mh_{mn}-\ii ng_{mn}=k_{mn}$ para todo $m$, $n$

Si $m\neq 0$ o $n\neq 0$ podemos tomar $g_{mn}=0$, $h_{mn}=\frac{1}{\ii m}k_{mn}$ o bien $g_{mn}=-\frac{1}{\ii n}k_{mn}$ y $h_{mn}=0$. Como antes, el problema está en $m=n=0$. $h_{00}$ es libre pero, para que $h\in \text{im } \d_1$, se requiere $h_{00}=0$. Así pues,

$$H^2(\T^2)=\dfrac{\{k\d\alpha\wedge\d\beta\}}{\left\{\left(\dfrac{\partial h}{\partial \alpha}-\dfrac{\partial g}{\partial \beta}\right)\d\alpha\wedge\d\beta\right\}}\simeq\R$$

y un generador de $H^2(\T^2)$ es $\d\alpha\wedge\d\beta$ ($h_{00}=1$)