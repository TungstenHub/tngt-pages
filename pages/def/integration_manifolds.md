Suppose we have an oriented manifold $M$. Now we should be able to define the integration of forms rigorously...

{{ image | integration_manifolds_sum width = 480 }}

Let's start with $\R^n$

A maximal order form in $\R^n$ matches the pattern $\alpha=f(x_1,x_2,...,x_n)\d x_1\wedge\d x_2\wedge...\wedge\d x_n$. Since $\d x_1\wedge\d x_2\wedge...\wedge\d x_n$ is the standard volume when evaluated in positive basis, it seems natural to define

$$
\int_{\R ^n}\alpha=\int_{\R ^n}f(x_1,x_2,...,x_n)\d x_1\wedge\d x_2\wedge...\wedge\d x_n=\int_{\R ^n}f(x_1,x_2,...,x_n)\d x_1\d x_2...\d x_n,
$$

where the last integral is the usual one in $\R^n$. To avoid convergence issues, we'll require $f$ to have compact support, that is, $\alpha\in\Omega^n_c(\R ^n)$.

On the other hand, suppose we have a maximal order form $\alpha$ in $M$ oriented manifold and $\varphi:U\longrightarrow M$ positive chart. On $U\subset \R^n$ we have the $n$-form $\varphi^*\alpha$; the last is defined to keep the valuation of $\alpha$, so it's reasonable that $\int_U \varphi^*\alpha=\int_{\varphi(U)}\alpha$. This should be enough to integrate over $M$, since we know how to do it locally

{{ image | integration_manifolds_euclidean_chart }}

>>>
Let $M$ be an oriented manifold of dimension $n$. There exists a unique linear map

$$\int_M:\Omega^n_c(M)\longrightarrow \R$$

satisfying the following property: if $\varphi:U\longrightarrow M$ is a positively oriented chart and the support of $\alpha\in\Omega^n_c(M)$ is contained in $\varphi(U)$, then $\int_M\alpha=\int_U \varphi^*\alpha$.

If $\{\varphi_i:U_i\longrightarrow M\}$ is a collection of charts covering $M$ and $\{\rho_i\}$ is a partition of unity associated to the open sets $\{\varphi_i(U_i)\}$, it holds that $\int_M\alpha=\sum_i \int_{U_i}\varphi_i^*(\rho_i\alpha)$.
<<<

The validity of the previous statements ultimately lies in proving that the last expression is independent of the chosen charts and partition of unity. For now, we'll limit ourselves to check the key fact: that $\int_M\alpha=\int_U \varphi^*\alpha$ holds when considering diffeomorphisms between to open sets of $\R^n$, keeping in mind that here the usual integral applies

Let $\varphi:U\longrightarrow V$ be a positively oriented diffeomorphism between open sets of $\R^n$ and $\alpha=f(y)\d y_1\wedge...\wedge\d y_n$ a $n$-form in $V$. Then

$$
\begin{array}{rcl}
\varphi^*(f(y)\d y_1\wedge...\wedge\d y_n) & = & (f\circ \varphi)\d(\varphi_1)\wedge...\wedge \d(\varphi_n)\\\\
& = & (f\circ \varphi)\left(\sum \dfrac{\partial \varphi_1}{\partial x_j}\d x_j\right)\wedge...\wedge\left(\sum \dfrac{\partial \varphi_n}{\partial x_j}\d x_j\right)\\\\
& = & (f\circ \varphi)\text{Det}\left(\dfrac{\partial \varphi_i}{\partial x_j}\right)\d x_1\wedge...\wedge\d x_n,
\end{array}
$$

the determinant appearing due to the antisymmetry of the wedge product. The Change of Variables Theorem ensures that

$$
\int_V\alpha=\int_V f\d y=\int_U (f\circ \varphi)\left|\text{Det}\left(\dfrac{\partial \varphi_i}{\partial x_j}\right)\right|\d x=\int_U (f\circ \varphi)\text{Det}\left(\dfrac{\partial \varphi_i}{\partial x_j}\right)\d x=\int_U\varphi^*\alpha,
$$

because $\varphi$ is a positively oriented diffeomorphism and therefore the determinant of the Jacobian matrix is positive

Two more notes:

<ol>
<li>If we switch the orientation of $M$ (positive basis becoming negative and viceversa), all the integrals get multiplied by $-1$</li>
<li>If $f:M\longrightarrow N$ is a positively oriented diffeomorphism, then $ \int_N\alpha=\int_M f^*\alpha$ para todo $\alpha\in\Omega^n_c(N)$</li>
</ol>