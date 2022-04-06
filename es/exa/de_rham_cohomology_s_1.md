Para $\S^1$ tenemos la parametrización $2\pi$-periódica $\R\longrightarrow\S^1$, $\theta\longmapsto \ee^{\ii\theta}$. Con esta parametrización, tenemos una 1-forma global, $\d \theta$, y $C^{\infty}(\S^1)$ se identifica con las funciones $\R\longrightarrow\R$ diferenciables y $2\pi$-periódicas

<ul>
  <li>0-formas: $f:\R\longrightarrow\R$ diferenciable y $2\pi$-periódica</li>
  <li>1-formas: $g\d \theta$, $g:\R\longrightarrow\R$ diferenciable y $2\pi$-periódica</li>
  <li>$\d(f)=\d f=\dfrac{\partial f}{\partial \theta}\d \theta$</li>
  <li>$\d(g\d\theta)=\d g\wedge\d \theta=\dfrac{\partial g}{\partial \theta}\d \theta\wedge\d \theta=0$</li>
</ul>

---

<ul>
  <li>$\text{ker }\d_0=\left\{f\middle|\dfrac{\partial f}{\partial \theta}=0\right\}=\{f|f=cte\in\R\}$</li>
  <li>$\text{im }\d_{-1}=\{0\}$ </li>
</ul>

$$H^0(\S^1)=\dfrac{\{f=cte\in\R\}}{0}\simeq\R$$

---

<ul>
  <li>$\text{ker }\d_1=\{g\d\theta\}$</li>
  <li>$\text{im }\d_0=\left\{\dfrac{\partial f}{\partial \theta}\d\theta\right\}$</li>
</ul>

y nos preguntamos si todas las funciones $g$ $2\pi$-periódicas se pueden expresar como la derivada de alguna función $f$ $2\pi$-periódica. Sólo queda la posibilidad $f(\theta)=\int_0^\theta g(t)\d t$ (salvo constantes), pero para que $f$ sea $2\pi$-periódica se requiere que $\int_0^{2\pi} g(t)\d t=0$. Esto no lo cumplen todas las $g$ $2\pi$-periódicas, pero dada una que no lo cumpla, se puede conseguir que lo cumpla restando una constante adecuada: $\tilde{g}=g-\frac{1}{2\pi}\int_0^{2\pi} g(t)\d t$. Así, toda función $g$ se escribe de modo único como la suma de una función constante y una función del tipo $\dfrac{\partial f}{\partial \theta}$. En consecuencia,

$$H^1(\S^1)=\dfrac{\{g\d\theta\}}{\left\{\dfrac{\partial f}{\partial \theta}\d\theta\right\}}\simeq\R$$

En este caso, $\d\theta$ es uno de los elementos no triviales de $H^1(\S^1)$. Igual que en $\R^2-(0,0)$, se trata de una forma cerrada (se relaciona localmente con la función ángulo $\theta$) pero da valores no nulos a curvas homológicamente no triviales, es decir, que dan varias vueltas a la circunferencia