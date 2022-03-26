%% to adjust width with props %%

{{ image | torus_manifold }}

The torus of dimension $n$ is defined as the product of $n$ circunferences: 

$$\T^n= \S^1\times \cdots \times \S^1$$ 

So we can apply [Künneth Theorem]( thm | kunneth_theorem ) right away:

$$H^*(\T^n)=H^*(\S^1)\otimes\cdots\otimes H^*(\S^1)$$ 

Since $H^0(\S^1_i)=\langle [1] \rangle$ and $H^1(\S^1_i)=\langle [\mathrm{d}\theta_i] \rangle$, it turns out that

$$\{[\mathrm{d}\theta_{i_1}\wedge...\wedge\mathrm{d}\theta_{i_k}] :1\leqslant i_1 <...< i_k\leqslant n\}$$

is a basis of $H^k(\T^n)$. In particular, 

$$H^k(\T^n)\simeq \R ^{\binom{n}{k}}$$