%% ajustar ancho con props %%

{{ image | torus_manifold }}

El toro de dimensión $n$ se define como el producto de $n$ circunferencias: 

$$\T^n= \S^1\times \cdots \times \S^1$$ 

Por lo que podemos aplicar el [Teorema de Künneth]( thm | kunneth_theorem ) directamente:

$$H^*(\T^n)=H^*(\S^1)\otimes\cdots\otimes H^*(\S^1)$$ 

Como $H^0(\S^1_i)=\langle [1] \rangle$ y $H^1(\S^1_i)=\langle [\mathrm{d}\theta_i] \rangle$, resulta que

$$\{[\mathrm{d}\theta_{i_1}\wedge...\wedge\mathrm{d}\theta_{i_k}] :1\leqslant i_1 <...< i_k\leqslant n\}$$

es una base de $H^k(\T^n)$. En particular, 

$$H^k(\T^n)\simeq \R ^{\binom{n}{k}}$$