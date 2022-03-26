Let $(X,T)$, $(Y,T_2)$ be two topological spaces, $\sim$ an equivalence relation in $X$ and $g:X\longrightarrow Y$ a map

<ol>
  <li>There exists $\bar g: \bar X\longrightarrow Y$ with $\bar g\circ \pi=g$ if and only if $x\sim x'\Longrightarrow g(x)=g(x')$</li>
  <li>$\bar g:(\bar X, \bar T)\longrightarrow (Y,T_2)$ is continuous if and only if $g:(X,T)\longrightarrow (Y,T_2)$ is continuous</li>
  <li>$\bar g$ is surjective if and only if $g$ is surjective</li>
  <li>$\bar g$ is injective if and only if $g(x)=g(x')\Longrightarrow x\sim x'$</li>
</ol>

+++
Proof
+++

<ol>
  <li>It is enough to define $\bar g([x])=g(x)$, that does not depend on the $x\in X$ chosen</li>
  <li>Let $V\in T_2$. Then $\bar g^{-1}(V)\in \bar T \Longleftrightarrow \pi^{-1}(\bar g^{-1}(V)) \in T \Longleftrightarrow g^{-1}(V)\in T$. So $\bar g$ is continuous $\Longleftrightarrow g$ is continuous</li>
  <li>$\bar g(\bar X)= \bar g(\pi(X))=g (X)$</li>
  <li>Suppose that $\bar g$ is injective. Then $g(x)=g(x')\Longrightarrow \bar g(\pi(x))=\bar g(\pi(x'))\Longrightarrow \pi(x)=\pi(x')\Longrightarrow x\sim x'$. Conversely, suppose that $g(x)=g(x')\Longrightarrow x\sim x'$; then $\bar g([x])=\bar g([x'])\Longrightarrow g(x)=g(x')\Longrightarrow x\sim x' \Longrightarrow [x]=[x']$, that is, $\bar g$ is injective</li>
</ol>

+++