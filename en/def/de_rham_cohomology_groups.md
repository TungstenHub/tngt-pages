Once defined the spaces of forms and the exterior derivative, we have the following chain of maps

$$
\Omega^0(M)\xrightarrow{\mathrm{d}}\Omega^1(M)\xrightarrow{\mathrm{d}}\Omega^2(M)\xrightarrow{\mathrm{d}}\cdots \xrightarrow{\mathrm{d}}\Omega^{k-1}(M)\xrightarrow{\mathrm{d}}\Omega^k(M)\xrightarrow{\mathrm{d}}\Omega^{k+1}(M)\xrightarrow{\mathrm{d}}\cdots\xrightarrow{\mathrm{d}}\Omega^n(M)
$$

called **de Rham complex**. A [_complex_]( def | complex_homology ) is a chain of homomorphisms between abelian groups satisfying $\mathrm{d}\circ\mathrm{d}=0$

We're looking for closed forms that are not exact. Much like in homology, quotients are the right way to go:

Let 

$$
\Omega^0(M)\xrightarrow{\mathrm{d}^0}\Omega^1(M)\xrightarrow{\mathrm{d}^1}\Omega^2(M)\xrightarrow{\mathrm{d}^2}\cdots \xrightarrow{\mathrm{d}^{k-1}}\Omega^k(M)\xrightarrow{\mathrm{d}^k}\cdots\xrightarrow{\mathrm{d}^{n-1}}\Omega^n(M)
$$

be the de Rham Complex associated to the manifold $M$. We define the **cohomology groups of $M$**

$$H^k(M)=\dfrac{\text{ker }\mathrm{d}^k}{\text{im }\mathrm{d}^{k-1}}=\dfrac{Z^k(M)}{B^k(M)}$$