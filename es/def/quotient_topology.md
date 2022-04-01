Sea $(X,T)$ un espacio topológico y $\sim$ una relación de equivalencia en $X$. Definimos el **espacio topológico cociente** como $\bar X=X/\sim$ con la topología cociente $\bar T=\{\bar V\subset \bar X\, \vert \, \pi^{-1}(\bar V)\in T\}$, donde $\pi:X\to X/\sim$ es la aplicación cociente.

Veamos que $\bar T$ es de hecho una topología:

<ol>
  <li>$\varnothing, \bar X \in \bar T$ porque $\pi^{-1}(\varnothing)=\varnothing \in T$ y $\pi^{-1}(\bar X)=X\in T$</li>
  <li>Si $V_1,V_2\in \bar T$ entonces $\pi^{-1}(V_1), \pi^{-1}(V_2)\in T$. Por tanto, $\pi^{-1}(V_1\cap V_2)=\pi^{-1}(V_1)\cap  \pi^{-1}(V_2)\in T$ y $V_1\cap V_2\in \bar T$</li>
  <li>Si $V_\alpha\in \bar T$, $\alpha\in \Lambda$, entonces $\pi^{-1}(V_\alpha) \in T$. Por tanto $\pi^{-1}(\bigcup V_\alpha)=\bigcup \pi^{-1}(V_\alpha) \in T$ y $\bigcup V_\alpha \in \bar T$</li>
</ol>

Un subconjunto $A\subset X$ se dice **saturado** si es una unión de clases de equivalencia, es decir, si $x\in A, y\sim x \Rightarrow
y\in A$ o equivalentemente si $A=\pi^{-1}(\pi(A))$. Dicho esto, la topología cociente está constituida por las imágenes de los abiertos saturados,

$$
\bar T = \{ \pi(U) \, | \, U\subset X \text{ abierto saturado}\}
$$