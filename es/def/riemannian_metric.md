Una **métrica riemanniana** en una variedad diferenciable $M$ es una colección $g$ de productos internos 

$$g_p=\langle\,\,,\,\rangle_p:T_pM\times T_pM \longrightarrow \R,\qquad p\in M$$

que es diferenciable en el sentido de que para cualesquiera dos campos vectoriales diferenciables $X$ e $Y$, la función

$$g(X,Y):M\longrightarrow \R,\qquad p\longmapsto g_p(X_p,Y_p)=\langle X_p,Y_p\rangle_p$$

es diferenciable

En este contexto, dada una carta $\varphi:U\longrightarrow M$ induciendo

$$\varphi^{-1}=(x^1,\cdots,x^n),\qquad x^i:\varphi(U)\longrightarrow \R$$
$$\{\partial_i\}_i=\left\{\frac{\partial}{\partial x^i}\right\}_i$$
$$\{\mathrm{d}x^i\}_i=\left\{\mathrm{d}(x^i)\right\}_i$$

las funciones (locales)

$$g_{ij}=g(\partial_i,\partial_j)=\langle\partial_i,\partial_j\rangle$$

son diferenciables, y podemos expresar

$$g=g_{ij}\mathrm{d}x^i\otimes\mathrm{d}x^j$$