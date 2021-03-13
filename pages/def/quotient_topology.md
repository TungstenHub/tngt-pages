Let $(X,T)$ be a topological space and $\sim$ an equivalence relation in $X$. We define the **quotient topological space** as $\bar X=X/\sim$ with the quotient topology $\bar T=\{\bar V\subset \bar X\, \vert \, \pi^{-1}(\bar V)\in T\}$, where $\pi:X\to X/\sim$ is the quotient map.

Let's check that $\bar T$ is indeed a topology:

<ol>
  <li>$\varnothing, \bar X \in \bar T$ because $\pi^{-1}(\varnothing)=\varnothing \in T$ and $\pi^{-1}(\bar X)=X\in T$</li>
  <li>If $V_1,V_2\in \bar T$ then $\pi^{-1}(V_1), \pi^{-1}(V_2)\in T$. Therefore $\pi^{-1}(V_1\cap V_2)=\pi^{-1}(V_1)\cap  \pi^{-1}(V_2)\in T$ and $V_1\cap V_2\in \bar T$</li>
  <li>If $V_\alpha\in \bar T$, $\alpha\in \Lambda$, then $\pi^{-1}(V_\alpha) \in T$. Therefore $\pi^{-1}(\bigcup V_\alpha)=\bigcup \pi^{-1}(V_\alpha) \in T$ and $\bigcup V_\alpha \in \bar T$</li>
</ol>

A subset $A\subset X$ is **saturated** if it is a union of equivalence classes, that is, if $x\in A, y\sim x \Rightarrow
y\in A$ or equivalently if $A=\pi^{-1}(\pi(A))$. This being said, the quotient topology is made up by the images of the saturated open subsets,

$$
\bar T = \{ \pi(U) \, | \, U\subset X \text{ saturated open set}\}
$$