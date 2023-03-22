Vamos a centrarnos en la cohomología de la variedad producto

Dadas dos variedades $M$ y $N$ de dimensiones $m$ y $n$, el producto $M\times N$ tiene una estructura de variedad de dimensión $m+n$. El producto se proyecta sobre cada factor, y similar a como pasaba en el [Lema de Poincaré]( lem | poincare_lemma ), formas en cada factor inducen formas en el producto

$$
M\xleftarrow{\,\,\,\pi_1\,\,}M\times N \xrightarrow{\,\,\pi_2\,\,\,}N\qquad\qquad
\Omega^*(M) \xrightarrow{\,\,\pi_1^*\,\,\,}\Omega^*(M\times N)\xleftarrow{\,\,\,\pi_2^*\,\,}\Omega^*(N)
$$

El producto exterior en formas nos permite definir

$$
\Omega^a(M)\otimes\Omega^b(N)\longrightarrow\Omega^{a+b}(M\times N )\qquad\qquad\alpha\otimes\beta\longmapsto\pi_1^*(\alpha)\wedge\pi_2^*(\beta)
$$

y este producto exterior va bien con la cohomología, por lo que también tenemos

$$
H^a(M)\otimes H^b(N)\longrightarrow H^{a+b}(M\times N)\qquad\qquad
[\alpha]\otimes[\beta]\longmapsto[\pi_1^*(\alpha)\wedge\pi_2^*(\beta)]
$$

De hecho, para obtener la máxima información sobre la cohomología de $M\times N$ de orden $k$, definimos la siguiente aplicación:

$$
\bigoplus_{a+b=k} H^a(M)\otimes H^b(N)\longrightarrow H^k(M\times N)\qquad\qquad
\sum[\alpha]\otimes[\beta]\longmapsto\sum[\pi_1^*(\alpha)\wedge\pi_2^*(\beta)]
$$

esperando que al menos sea sobreyectiva...