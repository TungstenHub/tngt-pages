Sean $(X,T)$, $(Y,T_2)$ dos espacios topológicos, $\sim$ una relación en $X$ y $g:X\longrightarrow Y$ una aplicación

<ol>
  <li>Existe $\bar g: \bar X\longrightarrow Y$ con $\bar g\circ \pi=g$ si y sólo si $x\sim x'\Longrightarrow g(x)=g(x')$</li>
  <li>$\bar g:(\bar X, \bar T)\longrightarrow (Y,T_2)$ es continua si y sólo si $g:(X,T)\longrightarrow (Y,T_2)$ es continua</li>
  <li>$\bar g$ es sobreyectiva si y sólo si $g$ es sobreyectiva</li>
  <li>$\bar g$ es inyectiva si y sólo si $g(x)=g(x')\Longrightarrow x\sim x'$</li>
</ol>

+++
Demostración
+++

<ol>
  <li>Basta definir $\bar g([x])=g(x)$, que no depende del $x\in X$ tomado</li>
  <li>Sea $V\in T_2$. Entonces $\bar g^{-1}(V)\in \bar T \Longleftrightarrow \pi^{-1}(\bar g^{-1}(V)) \in T \Longleftrightarrow g^{-1}(V)\in T$. Luego $\bar g$ es continua $\Longleftrightarrow g$ es continua</li>
  <li>$\bar g(\bar X)= \bar g(\pi(X))=g (X)$</li>
  <li>Supongamos que $\bar g$ es inyectiva. Entonces $g(x)=g(x')\Longrightarrow \bar g(\pi(x))=\bar g(\pi(x'))\Longrightarrow \pi(x)=\pi(x')\Longrightarrow x\sim x'$. Recíprocamente, supongamos que $g(x)=g(x')\Longrightarrow x\sim x'$; entonces $\bar g([x])=\bar g([x'])\Longrightarrow g(x)=g(x')\Longrightarrow x\sim x' \Longrightarrow [x]=[x']$, es decir, $\bar g$ es inyectiva</li>
</ol>

+++