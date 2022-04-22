Imagina que tenemos una variedad cociente, es decir, una variedad $\tilde{M}$ que se construye cuando un grupo $G$ actúa propia y discontinuamente sobre una variedad $M$. Esto significaría que hay un homomorfismo inyectivo $\varphi:G\longrightarrow \mathrm{Diffeo}(M)$ ($v(g)=v_g:M\longrightarrow M$); discontinuamente significa que cada punto de $M$ tiene un entorno $U$ que no se solapa con ninguna imagen $\varphi_g(U)$, $g\neq e$. El cociente $\tilde{M}=M/G$ viene de $M$ al identificar puntos en la misma órbita bajo las transformaciones $\varphi_g$

{{ image | group_action_manifold }}

Ahora bien, ¿tienen algo que ver las cohomologías de $M$ y $\tilde{M}$? Vamos a ver

Por una parte tenemos la proyección natural

$$\pi:M\longrightarrow \tilde{M}\qquad\qquad p\longmapsto [p]$$

que induce 

$$\pi^*:H^k(\tilde{M})\longrightarrow H^k(M)$$

Por otra parte, para cada $g\in G$ se tiene

$$\varphi_g:M\longrightarrow M$$

induciendo

$$\varphi_g^*:H^k(M)\longrightarrow H^k(M)$$

Como $\pi\circ\varphi_g=\pi$, también es verdad que

$$\varphi_g^*\circ\pi^*=\pi^*$$

Ok, ¿y ahora qué?