A **Riemannian metric** on a differentiable manifold $M$ is a collection $g$ of inner products 

$$g_p=\langle\,\,,\,\rangle_p:T_pM\times T_pM \longrightarrow \R,\qquad p\in M$$

that is differentiable in the sense that for any two differentiable vector fields $X$ and $Y$, the function

$$g(X,Y):M\longrightarrow \R,\qquad p\longmapsto g_p(X_p,Y_p)=\langle X_p,Y_p\rangle_p$$

is differentiable

In this context, given a chart $\varphi:U\longrightarrow M$ inducing

$$\varphi^{-1}=(x^1,\cdots,x^n),\qquad x^i:\varphi(U)\longrightarrow \R$$
$$\{\partial_i\}_i=\left\{\frac{\partial}{\partial x^i}\right\}_i$$
$$\{\mathrm{d}x^i\}_i=\left\{\mathrm{d}(x^i)\right\}_i$$

the (local) functions

$$g_{ij}=g(\partial_i,\partial_j)=\langle\partial_i,\partial_j\rangle$$

are differentiable, and we may express

$$g=g_{ij}\mathrm{d}x^i\otimes\mathrm{d}x^j$$