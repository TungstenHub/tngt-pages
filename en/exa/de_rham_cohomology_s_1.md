In $\S^1$ we have the standard $2\pi$-periodic parameterization $\R\longrightarrow\S^1$, $\theta\longmapsto \ee^{\ii\theta}$. This parameterization induces a global 1-form, $\d \theta$, and $C^{\infty}(\S^1)$ is identified with the set of differentiable and $2\pi$-periodic functions $\R\longrightarrow\R$

<ul>
  <li>0-forms: $f:\R\longrightarrow\R$ differentiable and $2\pi$-periodic</li>
  <li>1-forms: $g\d \theta$, $g:\R\longrightarrow\R$ differentiable and $2\pi$-periodic</li>
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

and we wonder whether every $2\pi$-periodic function $g$ may be expressed as the derivative of some other $2\pi$-periodic function $f$. It should be then $f(\theta)=\int_0^\theta g(t)\d t$ (up to constants), but for $f$ to be $2\pi$-periodic it is needed that $\int_0^{2\pi} g(t)\d t=0$. Obviously not every $2\pi$-periodic function $g$ meets this requirement, but one may overcome this by slightly modifying $g$: $\tilde{g}=g-\frac{1}{2\pi}\int_0^{2\pi} g(t)\d t$. This way every $g$ is expressed in a unique way as the sum of a constant function and a function of the type $\dfrac{\partial f}{\partial \theta}$. As a consequence, 

$$H^1(\S^1)=\dfrac{\{g\d\theta\}}{\left\{\dfrac{\partial f}{\partial \theta}\d\theta\right\}}\simeq\R$$

In this case, $\d\theta$ acts as a generator of $H^1(\S^1)$. Same to $\R^2-(0,0)$, it is closed (locally related to the angle function $\theta$) and assigns nonzero values to nonzero homological objects, i.e. the circumference loop itself