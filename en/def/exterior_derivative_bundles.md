In the context of vector bundles, it will very useful to reformulate the concept of connection with an analogy of the exterior derivative $\mathrm{d}$:

The exterior derivative (in functions) is a map $\mathrm{d}:C^\infty(M)=\Omega^0(M)\longrightarrow\Omega^1(M)$, that associates to each function a 1-form describing the degree of increase of the function with respect to a direction. In the same spirit, given a connection $\nabla$, we may introduce an **exterior derivative** $\mathrm{d}_\nabla:\Gamma(E)=\Omega^0(E)\longrightarrow\Omega^1(E)=\Omega^1(M)\otimes\Gamma(E)$ 1-forms with values in $E$, defined by $\mathrm{d}_\nabla(\sigma)(X)=\nabla_X\sigma$, that in each direction measures the mismatch with respect to the parallel transport. This derivative satisfies

<ol>
<li>$\mathrm{d}_\nabla(\sigma+\tau)=\mathrm{d}_\nabla(\sigma)+\mathrm{d}_\nabla(\tau)$</li>
<li>$\mathrm{d}_\nabla(f\sigma)=\mathrm{d} f\otimes\sigma+f\mathrm{d}_\nabla(\sigma)$</li>
</ol>

On the other hand, it is equivalent to define a connection $\nabla$ or a derivative $\Omega^0(E)\longrightarrow\Omega^1(E)$ satisfying the properties above