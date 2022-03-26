Imagine now that we have a quotient manifold, that is, a manifold $\tilde{M}$ that is built when a group $G$ acts properly and discontinuously upon a manifold $M$. This would mean that there is an injective homomorphism $\varphi:G\longrightarrow \mathrm{Diffeo}(M)$ ($v(g)=v_g:M\longrightarrow M$); discontinuity requires that each point in $M$ has a neighborhood $U$ that does not overlap with any image $\varphi_g(U)$, $g\neq e$. The quotient $\tilde{M}=M/G$ comes from $M$ when identifying points in the same orbit under the transformations $\varphi_g$

{{ image | group_action_manifold }}

Now, are the cohomology of $M$ and $\tilde{M}$ related in some way? Let's see 

In the one hand we have a natural projection

$$\pi:M\longrightarrow \tilde{M}\qquad\qquad p\longmapsto [p]$$

which induces 

$$\pi^*:H^k(\tilde{M})\longrightarrow H^k(M)$$

On the other hand, for each $g\in G$ we have

$$\varphi_g:M\longrightarrow M$$

inducing

$$\varphi_g^*:H^k(M)\longrightarrow H^k(M)$$

Since $\pi\circ\varphi_g=\pi$, it is also true that 

$$\varphi_g^*\circ\pi^*=\pi^*$$

Ok, and now what?