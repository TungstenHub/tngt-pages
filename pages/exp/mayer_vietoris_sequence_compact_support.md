For compact support cohomology, the Mayer-Vietoris sequence is quite different. First of all, there is no functoriality, that is, maps between manifolds do not induce maps over forms. But there is hope for inclussions - _and in a way that has no non-compact equivalent_

Let $M$ be a manifold and $U$ an open set of $M$. The inclussion induces the map $i_*:\Omega^k_c(U)\longrightarrow\Omega^k_c(M)$ (note the opposite direction!), defined by 

$$
i_*(\alpha)=
\begin{cases}
\alpha & \text{in \(U\)}\\
0 & \text{in \(M-\text{sop}(\alpha)\)}
\end{cases}
$$

That is, since $\alpha$ has compact support, its support doesn't reach the "border" of $U$ and can be extended by zero differentiably

And again we may gather everything up and build this chain:

{{ image | union_open_sets_injection_compact_form_chain }}