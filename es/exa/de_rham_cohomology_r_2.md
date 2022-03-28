In $\R^2$, differential forms are as follows:

<ul>
  <li>0-forms: $f:\R^2\longrightarrow\R$ differentiable</li>
  <li>1-forms: $g\d x+h\d y$, $g$, $h:\R^2\longrightarrow\R$ differentiable</li>
  <li>2-forms: $k\d x\wedge\d y$, $k:\R^2\longrightarrow\R$ differentiable</li>
</ul>

and the exterior derivative acts on them:

<ul>
  <li>$\d(f)=\d f=\dfrac{\partial f}{\partial x}\d x+\dfrac{\partial f}{\partial y}\d y$</li>
  <li>$\d(g\d x+h\d y)=
    \d g\wedge\d x+\d h\wedge\d y=
    \left(\dfrac{\partial g}{\partial x}\d x+\dfrac{\partial g}{\partial y}\d y\right)\wedge\d x+\left(\dfrac{\partial h}{\partial x}\d x+\dfrac{\partial h}{\partial y}\d y\right)\wedge\d y\\ \phantom{\d(g\d x+h\d y)}=
    \dfrac{\partial g}{\partial x}\d x\wedge\d x+\dfrac{\partial g}{\partial y}\d y\wedge\d x+\dfrac{\partial h}{\partial x}\d x\wedge\d y+\dfrac{\partial h}{\partial y}\d y\wedge\d y=
    \left(\dfrac{\partial h}{\partial x}-\dfrac{\partial g}{\partial y}\right)\d x\wedge\d y$</li>
  <li>$\d(k\d x\wedge\d y)=
    \d k\wedge\d x\wedge\d y=
    \left(\dfrac{\partial k}{\partial x}\d x+\dfrac{\partial k}{\partial y}\d y\right)\wedge\d x\wedge\d y=
    \dfrac{\partial k}{\partial x}\d x\wedge\d x\wedge\d y+\dfrac{\partial k}{\partial y}\d y\wedge\d x\wedge\d y=0$</li>
</ul>

Now we may compute the cohomology groups

---

<ul>
  <li>$\text{ker }\d_0=\left\{f\middle|\dfrac{\partial f}{\partial x}=\dfrac{\partial f}{\partial y}=0\right\}=\{f|f=cte\in\R\}$</li>
  <li>$\text{im }\d_{-1}=\{0\}$ (we take $\d_{-1}:0\longrightarrow\Omega^0(\R^2)$ the zero map)</li>
</ul>

$$H^0(\R^2)=\dfrac{\{f=cte\in\R\}}{0}\simeq\R$$

---

<ul>
  <li>$\text{ker }\d_1=\left\{g\d x+h\d y\middle|\dfrac{\partial h}{\partial x}-\dfrac{\partial g}{\partial y}=0\right\}$</li>
  <li>$\text{im }\d_0=\left\{\dfrac{\partial f}{\partial x}\d x+\dfrac{\partial f}{\partial y}\d y\right\}$</li>
</ul>

Obviously, $\text{im }\d_0\subset\text{ker }\d_1$, because $\dfrac{\partial (\partial f/\partial y)}{\partial x}-\dfrac{\partial (\partial f/\partial x)}{\partial y}=0$. Now we wonder whether equality holds. Let $g$, $h$ with $\dfrac{\partial h}{\partial x}=\dfrac{\partial g}{\partial y}$; there will exist some $f$ with $\dfrac{\partial f}{\partial x}=g$, $\dfrac{\partial f}{\partial y}=h$? If so, this function could be found by integration, moving along the $x$-axis and then vertically; let $f(0,0)=0$: 

$$f(x,y)=\int_0^x f_x(t,0)\d t+\int_0^y f_y(x,t)\d t=\int_0^x g(t,0)\d t+\int_0^y h(x,t)\d t$$

Does this function meet our requirements? 

$$\dfrac{\partial f}{\partial x}=g(x,0)+\int_0^y \dfrac{\partial h}{\partial x}(x,t)\d t=g(x,0)+\int_0^y \dfrac{\partial g}{\partial y}(x,t)\d t=g(x,0)+ [g(x,t)]_0^y=g(x,0)+g(x,y)-g(x,0)=g(x,y)$$ 

$$\dfrac{\partial f}{\partial y}=h(x,y)$$  

so $f$ is our desired function. Therefore there is equality in our previous sets and

$$H^1(\R^2)=\dfrac{\left\{g\d x+h\d y\middle|\dfrac{\partial h}{\partial x}-\dfrac{\partial g}{\partial y}=0\right\}}{\left\{\dfrac{\partial f}{\partial x}\d x+\dfrac{\partial f}{\partial y}\d y\right\}}=0$$

---

<ul>
  <li>$\text{ker }\d_2=\Omega^2(\R^2)=\{k\d x\wedge\d y\}$</li>
  <li>$\text{im }\d_1=\left\{\left(\dfrac{\partial h}{\partial x}-\dfrac{\partial g}{\partial y}\right)\d x\wedge\d y\right\}$</li>
</ul>

Given some fixed function $k$, there will exist $g$, $h$ with $\dfrac{\partial h}{\partial x}-\dfrac{\partial g}{\partial y}=k$? Now is very easy: we may take $g=0$ and $h(x,y)=\int_0^x k(t,y)\d t$, and everything is ok. So again kernel and image coincide and

$$H^2(\R^2)=\dfrac{\{k\d x\wedge\d y\}}{\left\{\left(\dfrac{\partial h}{\partial x}-\dfrac{\partial g}{\partial y}\right)\d x\wedge\d y\right\}}=0$$