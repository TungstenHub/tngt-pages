The sequence 

$$
0\xrightarrow{}\Omega^*_c(U\cap V)\xrightarrow{j_*}\Omega^*_c(U)\times\Omega^*_c(V)\xrightarrow{i_*}\Omega^*_c(M)\xrightarrow{}0
$$

is a [short exact sequence of complexes]( def | short_exact_sequence_complexes )

+++
Proof
+++

As before, there are three points to check:

<ol>
  <li>
  $j_*$ is injective. If a form is zero in $U$ or in $V$, it is automatically zero in $U\cap V$
  </li>

  <li>
  $\text{ im }j_*=\text{ker }i_*$. In the one hand $\text{ im }j_*\subset\text{ker }i_*$ is straightforward, since $\delta\longmapsto(j_{1*}\delta,-j_{2*}\delta)\longmapsto(i_1\circ j_1)_*\delta-(i_2\circ j_2)_*\delta=0$. On the other hand, if $(\beta,\gamma)\longmapsto i_{1*}\beta+i_{2*}\gamma=0$, then $\beta$ is zero in $U-V$, $\gamma$ is zero in $V-U$ and $\beta=-\gamma$ in $U\cap V$, and a preimage for $j_*$ is induced
  </li>

  <li>
  $i_*$ is surjective. Once again a differentiable partition of unit is needed: given $\alpha\in\Omega^*_c(M)$, we take the usual $\rho_U\alpha\in\Omega^*_c(U)$ and $\rho_V\alpha\in\Omega^*_c(V)$, and $
  (\rho_U\alpha,\rho_V\alpha)\longmapsto\rho_U\alpha+\rho_V\alpha=\alpha$
  </li>
</ol>

+++