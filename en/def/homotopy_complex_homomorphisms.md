Let $f$, $g:A_\ast\longrightarrow B_\ast$ be complex homomorphisms. A **homotopy between $f$ and $g$** is a family of maps $K:A_k\longrightarrow B_{k+1}$

{{ image | homotopy_complex_homomorphisms_homology }}

with $\partial_B\circ K+K\circ \partial_A=g-f:A_k\longrightarrow B_k$ for all $k$

If $f$ and $g$ are homotopic, the maps 

$$f_k,\,g_k:H_k(A_\ast)\longrightarrow H_k(B_\ast)$$

coincide:

$$(g_k-f_k)([a])=[(g-f)(a)]=[(\partial_B\circ K+K\circ \partial_A)(a)]=[\partial_B(K(a))]+[K(\partial_A(a))]=0$$

because $\partial_A(a)=0$ and $[\partial_B(\cdot)]=0$

The motivation of this definition is best seen in the [prism operator]( exp | prism_operator )

---

[Cohomological version]

Let $f$, $g:A^\ast\longrightarrow B^\ast$ be complex homomorphisms. A **homotopy between $f$ and $g$** is a family of maps $K:A^k\longrightarrow B^{k-1}$

{{ image | homotopy_complex_homomorphisms_cohomology }}

with $\mathrm{d}_B\circ K+K\circ \mathrm{d}_A=f-g:A^k\longrightarrow B^k$ for all $k$

If $f$ and $g$ are homotopic, the maps 

$$g^k,\,f^k:H^k(A^\ast)\longrightarrow H^k(B^\ast)$$

coincide:

$$(g^k-f^k)([a])=[(g-f)(a)]=[(\mathrm{d}_B\circ K+K\circ \mathrm{d}_A)(a)]=[\mathrm{d}_B(K(a))]+[K(\mathrm{d}_A(a))]=0$$

because $\mathrm{d}_A(a)=0$ and $[\mathrm{d}_B(\cdot)]=0$

The motivation of this definition is best seen in the [$K$ operator in the cohomology of homotopic maps]( thm | cohomology_homotopic_maps )