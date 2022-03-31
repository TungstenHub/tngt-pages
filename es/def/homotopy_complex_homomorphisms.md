Sean $f$, $g:A_\ast\longrightarrow B_\ast$ homomorfismos de complejos. Una **homotopía entre $f$ y $g$** es una familia de aplicaciones $K:A_k\longrightarrow B_{k+1}$

{{ image | homotopy_complex_homomorphisms_homology }}

con $\partial_B\circ K+K\circ \partial_A=g-f:A_k\longrightarrow B_k$ para todo $k$

Si $f$ y $g$ son homótopas, las aplicaciones 

$$f_k,\,g_k:H_k(A_\ast)\longrightarrow H_k(B_\ast)$$

coinciden:

$$(g_k-f_k)([a])=[(g-f)(a)]=[(\partial_B\circ K+K\circ \partial_A)(a)]=[\partial_B(K(a))]+[K(\partial_A(a))]=0$$

porque $\partial_A(a)=0$ y $[\partial_B(\cdot)]=0$

La motivación para esta definición se puede ver muy bien en el [operador prisma]( exp | prism_operator )

---

[Cohomological version]

Sean $f$, $g:A^\ast\longrightarrow B^\ast$ homomorfismos de complejos. Una **homotopía entre $f$ y $g$** es una familia de aplicaciones $K:A^k\longrightarrow B^{k-1}$

{{ image | homotopy_complex_homomorphisms_cohomology }}

con $\mathrm{d}_B\circ K+K\circ \mathrm{d}_A=f-g:A^k\longrightarrow B^k$ para todo $k$

Si $f$ y $g$ son homótopas, las aplicaciones 

$$g^k,\,f^k:H^k(A^\ast)\longrightarrow H^k(B^\ast)$$

coinciden:

$$(g^k-f^k)([a])=[(g-f)(a)]=[(\mathrm{d}_B\circ K+K\circ \mathrm{d}_A)(a)]=[\mathrm{d}_B(K(a))]+[K(\mathrm{d}_A(a))]=0$$

porque $\mathrm{d}_A(a)=0$ y $[\mathrm{d}_B(\cdot)]=0$

La motivación para esta definición se puede ver muy bien en el [operador $K$ en la cohomología de aplicaciones homótopas]( thm | cohomology_homotopic_maps )