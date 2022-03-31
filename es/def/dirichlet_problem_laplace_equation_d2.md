Sea 

$$D^2=\{(x,y)\in\mathbb{R}^2\vert x^2+y^2 < 1\}$$ 

el disco unidad en $\mathbb{R}^2$ y 

$$\mathcal{C}_{2\pi}(\mathbb{R})=\{f:\mathbb{R}\longrightarrow\mathbb{R}\vert f \text{ es continua y \(2\pi\)-periódica}\}$$

el conjunto de las funciones reales continuas y $2\pi$-periódicas. El **problema de Dirichlet para la ecuación de Laplace en el disco unidad** se plantea como

$$
\begin{cases}
\Delta u = 0 & \text{ in \(D^2\)}\\
u=f          & \text{ in \(\partial D^2\)}\\
\end{cases},
\qquad u\in\mathcal{C}^2(D^2)\cup\mathcal{C}(\overline{D^2})
$$

para $\Delta=\dfrac{\partial^2}{\partial x^2}+\dfrac{\partial^2}{\partial y^2}$ el operador de Laplace y alguna $f\in\mathcal{C}_{2\pi}(\mathbb{R})$ induciendo $f\in\mathcal{C}(\partial D^2)$ por la parametrización $\mathbb{R}\longrightarrow\partial D^2$, $t\longmapsto(\cos t,\sin t)$