In a Kähler manifold

$$\omega=\sum_{jk}\omega_{j\bar{k}}\mathrm{d} z^j\wedge\mathrm{d}\bar{z}^k=\mathrm{i}\sum_{jk}g_{j\bar{k}}\mathrm{d} z^j\wedge\mathrm{d}\bar{z}^k$$

$$\mathrm{d}\omega=\mathrm{i}\sum_{jk}\left(\dfrac{\partial g_{j\bar{k}}}{\partial z^l}\mathrm{d} z^l\wedge\mathrm{d} z^j\wedge\mathrm{d}\bar{z}^k+\dfrac{\partial g_{j\bar{k}}}{\partial \bar{z}^l}\mathrm{d}\bar{z}^l\wedge\mathrm{d} z^j\wedge\mathrm{d}\bar{z}^k\right)=0$$

and therefore

$$\dfrac{\partial g_{j\bar{k}}}{\partial z^l}=\dfrac{\partial g_{l\bar{k}}}{\partial z^j}$$ 
$$\dfrac{\partial g_{j\bar{k}}}{\partial \bar{z}^l}=\dfrac{\partial g_{j\bar{l}}}{\partial \bar{z}^k}$$

Integrating along the coordinate chart, the exists a function $\mathcal{K}$ 

$$g_{j\bar{k}}=\dfrac{\partial^2\mathcal{K}}{\partial z^j \partial \bar{z}^k}$$

and also

$$\omega=\mathrm{i}\sum_{jk}\dfrac{\partial^2\mathcal{K}}{\partial z^j \partial \bar{z}^k}\mathrm{d} z^j\wedge\mathrm{d}\bar{z}^k=\mathrm{i}\partial\bar{\partial}\mathcal{K}$$

This locally defined function $\mathcal{K}$ is called the **Kähler potential**