Let's consider the torus $\T^2=\S^1\times\S^1$. Again, the covering $\R^2\longrightarrow\T^2$, $(\alpha,\beta)\longmapsto(\ee^{\ii\alpha},\ee^{\ii\beta})$ provides two global 1-forms $\d \alpha$, $\d \beta$

<ul>
  <li>0-forms: $f:\R^2\longrightarrow\R$</li>
  <li>1-forms: $g\d \alpha+h\d \beta$</li>
  <li>2-forms: $k\d \alpha\wedge\d \beta$</li>
</ul>

where every function is differentiable and $2\pi$-periodic _in each variable_. $\d$ acts as in $\R^2$

---

$$H^0(\T^2)=\dfrac{\text{ker }\d_0}{\text{im }\d_{-1}}=\dfrac{\left\{f\middle|\dfrac{\partial f}{\partial \alpha}=\dfrac{\partial f}{\partial \beta}=0\right\}}{0}=\dfrac{\{f=cte\in\R\}}{0}\simeq\R$$

---

To compute the next cohomology groups we will use the Fourier series of these periodic functions: $f(\alpha,\beta)=\sum_{\substack{m,n=-\infty}}^\infty f_{mn}\ee^{\ii m\alpha}\ee^{\ii n\beta}$, and the same for $g$, $h$ y $k$. This decomposition will be merely formal, without minding convergence or differentiability, in a totally heuristic fashion which, however, yields completely right results

$$\d (g\d \alpha+h\d\beta)=\left(\dfrac{\partial h}{\partial \alpha}-\dfrac{\partial g}{\partial \beta}\right)\d \alpha\wedge\d\beta=\ii\sum_{mn}(mh_{mn}-ng_{mn})\ee^{\ii m\alpha}\ee^{\ii n\beta}\d \alpha\wedge\d\beta$$

and equals 0 if $mh_{mn}=ng_{mn}$ for all $m$, $n$; on the other hand 

$$\d(f)=\dfrac{\partial f}{\partial \alpha}\d \alpha+\dfrac{\partial f}{\partial \beta}\d \beta=\ii\sum_{mn}mf_{mn}\ee^{\ii m\alpha} \ee^{\ii n\beta} \d\alpha+ \ii\sum_{mn}nf_{mn}\ee^{\ii m\alpha}\ee^{\ii n\beta}\d\beta$$ 

Therefore, given $g_{mn}$, $h_{mn}$ with $mh_{mn}=ng_{mn}$, we're looking for $f_{mn}$ with $g_{mn}=\ii mf_{mn}$, $h_{mn}=\ii nf_{mn}$

For $m\neq 0$, we may take $f_{mn}=\frac{1}{\ii m}g_{mn}$, and 

$$\ii mf_{mn}=g_{mn},\qquad\ii nf_{mn}=\frac{\ii n}{\ii m}g_{mn}=\frac{1}{m}mh_{mn}=h_{mn}$$

In the same way, if $n\neq 0$, we take $f_{mn}=\frac{1}{\ii n}h_{mn}$. The very problem is $m=n=0$: $0h_{00}=0g_{00}$ always holds, but $g_{00}=\ii0f_{00}$ and $h_{00}=\ii0f_{00}$ only holds if $g_{00}=h_{00}=0$. This way, not every pair of functions $g$, $h$ with $\dfrac{\partial h}{\partial \alpha}-\dfrac{\partial g}{\partial \beta}=0$ follow the pattern $\dfrac{\partial f}{\partial \alpha}$, $\dfrac{\partial f}{\partial \beta}$; previously we have to adjust $g_{00}=h_{00}=0$. Therefore,

$$H^1(\T^2)=\dfrac{\left\{g\d\alpha+h\d\beta\middle|\dfrac{\partial h}{\partial \alpha}-\dfrac{\partial g}{\partial \beta}=0\right\}}{\left\{\dfrac{\partial f}{\partial \alpha}\d \alpha+\dfrac{\partial f}{\partial \beta}\d \beta\right\}}\simeq\R^2$$

because $g$ and $h$ retain two extra degrees of freedom

Two generators of $H^1(\T^2)$ are $\d\alpha$ ($g_{00}=1$) and $\d \beta$ ($h_{00}=1$). As with the circumference, these are closely related to the homology generators of $H_1(\T^2)$

---

$\d(k\d \alpha\wedge\d\beta)=0$, so the kernel of $\d_2$ is the entire $\Omega^2(\T^2)$. On the other hand, 

$$\d (g\d \alpha+h\d\beta)=\ii\sum_{mn}(mh_{mn}-ng_{mn})\ee^{\ii m\alpha}\ee^{\ii n\beta}\d \alpha\wedge\d\beta$$

We need to study if given $k_{mn}$ we may find $g_{mn}$, $h_{mn}$ with $\ii mh_{mn}-\ii ng_{mn}=k_{mn}$ for all $m$, $n$

If $m\neq 0$ or $n\neq 0$ we may take $g_{mn}=0$, $h_{mn}=\frac{1}{\ii m}k_{mn}$ or $g_{mn}=-\frac{1}{\ii n}k_{mn}$ and $h_{mn}=0$. As before, the problem resides in $m=n=0$. $h_{00}$ is free, but for $h\in \text{im } \d_1$, it is required that $h_{00}=0$. So in the end,

$$H^2(\T^2)=\dfrac{\{k\d\alpha\wedge\d\beta\}}{\left\{\left(\dfrac{\partial h}{\partial \alpha}-\dfrac{\partial g}{\partial \beta}\right)\d\alpha\wedge\d\beta\right\}}\simeq\R$$

and a generator of $H^2(\T^2)$ is $\d\alpha\wedge\d\beta$ ($h_{00}=1$)