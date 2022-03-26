The sequence 

$$
0\xrightarrow{}\Omega^*(M)\xrightarrow{i^*}\Omega^*(U)\times\Omega^*(V)\xrightarrow{j^*}\Omega^*( U\cap V)\xrightarrow{}0
$$

is a [short exact sequence of complexes]( def | short_exact_sequence_complexes )

+++
Proof
+++

There are three points to check:

<ol>
  <li>
  $\Omega^*(M)\xrightarrow{i^*}\Omega^*(U)\times\Omega^*(V)$ is injective. Given a form $\alpha$, if $\alpha|_U$ and $\alpha|_V$ are zero (that is, they are identically zero in each tangent space) then $\alpha$ is zero in all $M$
  </li>

  <li>
  $\text{ im }i^*=\text{ker }j^*$. Of course, $\text{im }i^*\subset\text{ker }j^*$, because $\alpha\longmapsto(\alpha|_U,\alpha|_V)\longmapsto\alpha|_{ U\cap V}-\alpha|_{ U\cap V}=0$. But if $(\beta,\gamma)\longmapsto\beta|_{ U\cap V}-\gamma|_{ U\cap V}=0$, then $\beta$ and $\gamma$ match along the common domain and we may define 

  $$\alpha=
  \begin{cases}
  \beta & \text{in $U$}\\
  \gamma & \text{in $V$}
  \end{cases},$$

  so $(\beta,\gamma)=i^*(\alpha)\in\text{ im }i^*$.
  </li>

  <li>
  $\Omega^*(U)\times\Omega^*(V)\xrightarrow{j^*}\Omega^*(U\cup V)$ is surjective. This is the trickiest point. As with the sphere, it's not trivial to extend forms to bigger open sets; the best strategy is to use compact support functions or, more concretely, a differentiable partition of unit. 

  Let $\{U,V\}$ be an open cover of $M$; associated with it we have the differentiable partition of unit $\{\rho_U,\rho_V\}$. These functions satisfy: they're differentiable, $\rho_U+\rho_V=1$, the support of $\rho_U$ is contained in $U$ and that of $\rho_V$ in $V$. Let $\delta\in\Omega^k(U\cap V)$. When we multiply $\delta$ and the partition functions, we get a pair of easily extensible functions: $\rho_V$ is zero out of $V$, so we take 
  $$\beta=
  \begin{cases}
  \rho_V \delta & \text{in $U\cap V$}\\
  0 & \text{in $U-\text{sop}(\rho_V)$}
  \end{cases},$$ 

  and $\rho_U$ is zero out of $U$, so we take 

  $$\gamma=
  \begin{cases}
  -\rho_U \delta & \text{in $U\cap V$}\\
  0 & \text{in $V-\text{sop}(\rho_U)$}
  \end{cases}.$$ 

  Now $(\beta,\gamma)\longmapsto\beta|_{ U\cap V}-\gamma|_{ U\cap V}=\rho_V \delta-(-\rho_U \delta)=(\rho_V+\rho_U)\delta=\delta$, so $j^*$ is surjective
  </li>
</ol>

+++