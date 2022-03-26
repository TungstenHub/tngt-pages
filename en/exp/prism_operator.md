Let $f$, $g:X\longrightarrow Y$ be homotopic (that is, interpolated by a continuous family of maps $h_t:X\longrightarrow Y$, $h_0=f$, $h_1=g$). It seems that $f_\ast$, $g_\ast:H_k(X)\longrightarrow H_k(Y)$ coincide, but to prove it formally, we may define the **prism operator** $P:C_k(X)\longrightarrow C_{k+1}(Y)$, obtained travelling the image of the homotopy:

{{ image | prism_operator }}

This operator satisfies $\partial P=g_\ast-f_\ast-P\partial$, as seen in the picture. When applied to a cycle, the term $P\partial\sigma$ dissapears and one has $\partial P\sigma=g_\ast\sigma-f_\ast\sigma$; since $f_\ast\sigma$ and $g_\ast\sigma$ differ in a boundary, they induce the same element of $H_k(Y)$

{{ image | prism_operator_homology }}