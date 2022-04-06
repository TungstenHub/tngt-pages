En $\R^2$, las formas diferenciales son del siguiente tipo:

<ul>
  <li>0-formas: $f:\R^2\longrightarrow\R$ diferenciable</li>
  <li>1-formas: $g\d x+h\d y$, $g$, $h:\R^2\longrightarrow\R$ diferenciables</li>
  <li>2-formas: $k\d x\wedge\d y$, $k:\R^2\longrightarrow\R$ diferenciable</li>
</ul>

y la diferencial exterior actúa en ellas de este modo:

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

Ahora podemos calcular los grupos de cohomología

---

<ul>
  <li>$\text{ker }\d_0=\left\{f\middle|\dfrac{\partial f}{\partial x}=\dfrac{\partial f}{\partial y}=0\right\}=\{f|f=cte\in\R\}$</li>
  <li>$\text{im }\d_{-1}=\{0\}$ (tomamos $\d_{-1}:0\longrightarrow\Omega^0(\R^2)$ la aplicación nula)</li>
</ul>

$$H^0(\R^2)=\dfrac{\{f=cte\in\R\}}{0}\simeq\R$$

---

<ul>
  <li>$\text{ker }\d_1=\left\{g\d x+h\d y\middle|\dfrac{\partial h}{\partial x}-\dfrac{\partial g}{\partial y}=0\right\}$</li>
  <li>$\text{im }\d_0=\left\{\dfrac{\partial f}{\partial x}\d x+\dfrac{\partial f}{\partial y}\d y\right\}$</li>
</ul>

Evidentemente, $\text{im }\d_0\subset\text{ker }\d_1$, pues $\dfrac{\partial (\partial f/\partial y)}{\partial x}-\dfrac{\partial (\partial f/\partial x)}{\partial y}=0$. Nos preguntamos si se da la igualdad. Sean $g$, $h$ con $\dfrac{\partial h}{\partial x}=\dfrac{\partial g}{\partial y}$; ¿existirá una $f$ con $\dfrac{\partial f}{\partial x}=g$, $\dfrac{\partial f}{\partial y}=h$? En caso afirmativo, esta función se podría hallar por integración, desplazándose por el eje $x$ y luego verticalmente; tomamos $f(0,0)=0$: 

$$f(x,y)=\int_0^x f_x(t,0)\d t+\int_0^y f_y(x,t)\d t=\int_0^x g(t,0)\d t+\int_0^y h(x,t)\d t$$

¿Cumple esta función lo que queremos?

$$\dfrac{\partial f}{\partial x}=g(x,0)+\int_0^y \dfrac{\partial h}{\partial x}(x,t)\d t=g(x,0)+\int_0^y \dfrac{\partial g}{\partial y}(x,t)\d t=g(x,0)+ [g(x,t)]_0^y=g(x,0)+g(x,y)-g(x,0)=g(x,y)$$ 

$$\dfrac{\partial f}{\partial y}=h(x,y)$$  

así que $f$ es la función buscada. Por tanto se tiene una igualdad entre los conjuntos anteriores y

$$H^1(\R^2)=\dfrac{\left\{g\d x+h\d y\middle|\dfrac{\partial h}{\partial x}-\dfrac{\partial g}{\partial y}=0\right\}}{\left\{\dfrac{\partial f}{\partial x}\d x+\dfrac{\partial f}{\partial y}\d y\right\}}=0$$

---

<ul>
  <li>$\text{ker }\d_2=\Omega^2(\R^2)=\{k\d x\wedge\d y\}$</li>
  <li>$\text{im }\d_1=\left\{\left(\dfrac{\partial h}{\partial x}-\dfrac{\partial g}{\partial y}\right)\d x\wedge\d y\right\}$</li>
</ul>

Dada una función $k$ fija, ¿existirán $g$, $h$ con $\dfrac{\partial h}{\partial x}-\dfrac{\partial g}{\partial y}=k$? Ahora es muy fácil: podemos tomar $g=0$ y $h(x,y)=\int_0^x k(t,y)\d t$, y se cumple el requisito anterior. Así que de nuevo el núcleo y la imagen coinciden y

$$H^2(\R^2)=\dfrac{\{k\d x\wedge\d y\}}{\left\{\left(\dfrac{\partial h}{\partial x}-\dfrac{\partial g}{\partial y}\right)\d x\wedge\d y\right\}}=0$$