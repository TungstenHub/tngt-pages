Let $M$ and $N$ be manifolds. If $f$, $g:M\longrightarrow N$ are homotopic, the maps $f^\ast$, $g^\ast:H^k(N)\longrightarrow H^k(M)$ coincide

+++
Proof
+++

Before dealing with the main statement, let's study the forms in the space $M\times \R $.

In $\R ^{n+1}$, a basis for the alternate forms of order $k$ is $\{\d x_{i_1}\wedge...\wedge\d x_{i_k}:1\leqslant i_1 < ... < i_k \leqslant n+1\}$. Some of this elements have $\d x_{n+1}$ but others don't; dividing into two groups, any $k$-form is decomposable in a unique way as $\beta+\alpha\wedge\d x_{n+1}$, where $\beta$ is a $k$-form in $\R ^n$ and $\alpha$ is a $(k-1)$-form in $\R ^n$

When considering manifolds, any $k$-form in $M\times \R $ is decomposable in a unique way as $\beta+\d t\wedge\alpha$, where $\beta$ and $\alpha$ are forms in $M$ of order $k$ and $k-1$ _dependent on $x\in M$ and $t\in \R $_. That is, given a chart of $M$ these forms are expressed as 

$$\beta=\sum \beta_{i_1 i_2... i_k}(x,t)\d x_{i_1}\wedge...\wedge\d x_{i_k},\qquad 1\leqslant i_1 < ... < i_k \leqslant n$$
$$\alpha=\sum \alpha_{i_1 i_2... i_{k-1}}(x,t)\d x_{i_1}\wedge...\wedge\d x_{i_{k-1}},\qquad 1\leqslant i_1 < ... < i_{k-1} \leqslant n$$

Usual calculus in the second argument allows us to _derive and integrate a form $\beta(t)\in \Omega^k(M)$ along the $\R$ fiber_:

$$
\begin{array}{rl}
\displaystyle\dfrac{\partial \beta}{\partial t}, & \displaystyle\qquad\dfrac{\partial \beta}{\partial t}(v_1,...,v_k)=\dfrac{\partial }{\partial t}[\beta(v_1,...,v_k)]\\\\
\displaystyle\int_a^b \beta, & \displaystyle\qquad\left(\int_a^b \beta\right)(v_1,...,v_k)=\int_a^b (\beta(v_1,...,v_k))\\
\end{array}
$$

The first operation outputs a $k$-form in $M$ for each $t$ in which derivation is performed; the second operation outputs a $k$-form for each interval $[a,b]$

Let $\d$ be the exterior derivative in $M$ and $\bar{\d}$ the exterior derivative in $M\times \R $. For brevity, $\d x_{i_1}\wedge...\wedge\d x_{i_k}$ will be denoted $\d x_I$

$$
\bar{\d}(f(x,t)\d x_I)=\bar{\d}(f(x,t))\wedge\d x_I=\left(\sum \dfrac{\partial f}{\partial x_i}\d x_i + \dfrac{\partial f}{\partial t}\d t\right)\wedge\d x_I=\d(f\d x_I)+\d t\wedge\left(\dfrac{\partial f}{\partial t}\d x_I\right)
$$
$$
\bar{\d}(f(x,t)\d t\wedge\d x_I)=\bar{\d}(f(x,t))\wedge \d t \wedge\d x_I=\left(\sum \dfrac{\partial f}{\partial x_i}\d x_i + \dfrac{\partial f}{\partial t}\d t\right)\wedge\d t\wedge\d x_I= \\\\ -\sum \dfrac{\partial f}{\partial x_i}\d t\wedge\d x_i\wedge\d x_I=-\d t\wedge\d(f(x,t)\wedge\d x_I)
$$

and summing up everything, 

$$\bar{\d}(\beta+\d t\wedge\alpha)=\d \beta+\d t\wedge\left(\dfrac{\partial \beta}{\partial t}-\d \alpha\right)$$

Now we return to the main problem. We have $f$, $g:M\longrightarrow N$ inducing $f^\ast$, $g^\ast:\Omega^k(N)\longrightarrow \Omega^k(M)$. And we'd like to build a [homotopy of complex homomorphisms]( def | homotopy_complex_homomorphisms ) between $f^\ast$ and $g^\ast$, much in the way the [prism operator]( exp | prism_operator ) provided a homotopy for homology. What are our tools? We have a homotopy 

$$H:M\times [0,1]\longrightarrow N$$ 
$$h_t:M\longrightarrow N,\qquad h_t(x)=H(x,t)$$
$$h_0=f\qquad h_1=g$$
$$h_t=H\circ s_t$$

with $s_t$ the natural immersion of $M$ in $M\times\R $ at level $t$. That is,

$$\Omega^k(N)\xrightarrow{h_t^\ast}\Omega^k(M)\quad\leadsto\quad\Omega^k(N)\xrightarrow{H^\ast}\Omega^k(M\times\R )\xrightarrow{s_t^\ast}\Omega^k(M)$$

Let's do it! Let $\gamma\in\Omega^k(N)$, with $H^\ast(\gamma)=\beta+\d t\wedge\alpha\in\Omega^k(M\times\R )$. In the inclusion $s_t$, the vertical component does nothing, so 

$$s_t^\ast(\beta+\d t\wedge\alpha)=\beta(t)$$

This way, 

$$f^\ast(\gamma)=(H\circ s_0)^\ast(\gamma)=s_0^\ast(H^\ast(\gamma))=s_0^\ast(\beta+\d t\wedge\alpha)=\beta(0)$$ 
$$g^\ast(\gamma)=(H\circ s_1)^\ast(\gamma)=s_1^\ast(H^\ast(\gamma))=s_1^\ast(\beta+\d t\wedge\alpha)=\beta(1)$$

We define the following operator

$$K:\Omega^k(N)\longrightarrow\Omega^{k-1}(M),\qquad K(\gamma)=\int_0^1\alpha$$

Is this a homotopy between $f^\ast$ and $g^\ast$? Does $\d\circ K+K\circ\d=g^\ast-f^\ast$ hold? On one side

$$\d K(\gamma)=\d \int_0^1\alpha=\int_0^1\d\alpha$$

because integration behaves as a ponderated sum of the $\alpha$ found along the fiber, and $\d$ is a linear operator. On the other side, 

$$H^\ast(\d \gamma)=\bar{\d} H^\ast(\gamma)=\bar{\d}(\beta+\d t\wedge\alpha)=\d \beta+\d t\wedge\left(\dfrac{\partial \beta}{\partial t}-\d \alpha\right)$$

and therefore

$$K\d \gamma=\int_0^1\left(\dfrac{\partial \beta}{\partial t}-\d \alpha\right)=\beta(1)-\beta(0)-\int_0^1\d\alpha$$

having finally

$$(\d K+K\d)(\gamma)=\int_0^1\d\alpha+\beta(1)-\beta(0)-\int_0^1\d\alpha=\beta(1)-\beta(0)=(g^\ast -f^\ast)(\gamma)$$

so $K$ effectively induces a homotopy between $f^\ast$ and $g^\ast$ and the maps in cohomology coincide. It is remarkable that the $K$ operator is indeed closely related to the prism operator: if $\sigma$ is a submanifold of $M$ whose dimension matches the order of $\gamma$, then

$$\int_{P\sigma}\gamma=\int_{\sigma}K\gamma$$

+++