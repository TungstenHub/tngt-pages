Let 

$$D^2=\{(x,y)\in\mathbb{R}^2\vert x^2+y^2 < 1\}$$ 

be the unit disc in $\mathbb{R}^2$ and 

$$\mathcal{C}_{2\pi}(\mathbb{R})=\{f:\mathbb{R}\longrightarrow\mathbb{R}\vert f \text{ is continuous and \(2\pi\)-periodic}\}$$

the set of continuous and $2\pi$-periodic real functions. The **Dirichlet problem for the Laplace equation in the unit disc** is stated as

$$
\begin{cases}
\Delta u = 0 & \text{ in \(D^2\)}\\
u=f          & \text{ in \(\partial D^2\)}\\
\end{cases},
\qquad u\in\mathcal{C}^2(D^2)\cup\mathcal{C}(\overline{D^2})
$$

for $\Delta=\dfrac{\partial^2}{\partial x^2}+\dfrac{\partial^2}{\partial y^2}$ the Laplace operator and some $f\in\mathcal{C}_{2\pi}(\mathbb{R})$ inducing $f\in\mathcal{C}(\partial D^2)$ by the parameterization $\mathbb{R}\longrightarrow\partial D^2$, $t\longmapsto(\cos t,\sin t)$