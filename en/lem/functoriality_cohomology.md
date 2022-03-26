A differentiable map $f:M\longrightarrow N$ induces pullback functions $f^*:\Omega^k(N)\longrightarrow \Omega^k(M)$. But since the identity $\d\circ f^*=f^*\circ\d$, we indeed have a [complex homomorphism]( def | complex_homomorphism )

$$f^*:\Omega^*(N)\longrightarrow \Omega^*(M)$$

that is,

$$
\begin{CD}
\cdots @>>> \Omega^{k-1}(N) @>{\d^{k-1}}>> \Omega^{k}(N) @>{\d^{k}}>> \Omega^{k+1}(N) @>>> \cdots\\
@.          @V{f^{k-1}}VV                  @V{f^{k}}VV                @V{f^{k+1}}VV @.           \\
\cdots @>>> \Omega^{k-1}(M) @>{\d^{k-1}}>> \Omega^{k}(M) @>{\d^{k}}>> \Omega^{k+1}(M) @>>> \cdots\\
\end{CD}
$$

which induces homomorphisms in cohomology

$$f^*:H^k(N)\longrightarrow H^k(M)$$

for each $k$. The usual properties $(f\circ g)^*=g^*\circ f^*$, $(\mathrm{id}_M)^*=\mathrm{id}_{H(M)}$ hold. Therefore a diffeomorphism $f:M\longrightarrow N$ induces isomorphisms in the cohomology groups