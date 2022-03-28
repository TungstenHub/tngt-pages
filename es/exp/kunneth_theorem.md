Let's focus on the cohomology of a product manifold 

Given two manifolds $M$ and $N$ of dimensions $m$ and $n$, the product $M\times N$ has a structure of manifold of dimension $m+n$. The product is projected over each factor, and much like in the [Poincaré Lemma]( lem | poincare_lemma ), forms in each factor induce forms in the product

$$
M\xleftarrow{\,\,\,\pi_1\,\,}M\times N \xrightarrow{\,\,\pi_2\,\,\,}N\qquad\qquad
\Omega^*(M) \xrightarrow{\,\,\pi_1^*\,\,\,}\Omega^*(M\times N)\xleftarrow{\,\,\,\pi_2^*\,\,}\Omega^*(N)
$$

The exterior product in forms allows us to define

$$
\Omega^a(M)\otimes\Omega^b(N)\longrightarrow\Omega^{a+b}(M\times N )\qquad\qquad\alpha\otimes\beta\longmapsto\pi_1^*(\alpha)\wedge\pi_2^*(\beta)
$$

and this exterior product works well with cohomology, so we also have

$$
H^a(M)\otimes H^b(N)\longrightarrow H^{a+b}(M\times N)\qquad\qquad
[\alpha]\otimes[\beta]\longmapsto[\pi_1^*(\alpha)\wedge\pi_2^*(\beta)]
$$

In fact, to obtain the maximum information about the cohomology of $M\times N$ of order $k$, we define the following map:

$$
\bigoplus_{a+b=k} H^a(M)\otimes H^b(N)\longrightarrow H^k(M\times N)\qquad\qquad
\sum[\alpha]\otimes[\beta]\longmapsto\sum[\pi_1^*(\alpha)\wedge\pi_2^*(\beta)]
$$

and we hope that it is at least surjective...