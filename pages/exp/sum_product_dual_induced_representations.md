As shown in the previous examples, one may get bigger representations from smaller ones

---

[{direct_sum}]

Given representations 

$$\sigma: G \ll \GL(V)$$
$$\tau: G \ll \GL(W)$$

it is induced the **direct sum representation**

$$\rho = \sigma\oplus\tau: G \ll \GL(V\oplus W)$$
$$g(v,w) = (gv, gw)$$

---

[{tensor_product}]

Given representations 

$$\sigma: G \ll \GL(V)$$
$$\tau: G \ll \GL(W)$$

it is induced the **tensor product representation**

$$\rho = \sigma\otimes\tau: G \ll \GL(V\otimes W)$$
$$g(v\otimes w) = gv \otimes gw$$

+++
Check well-defined
+++

Is it well-defined? For some fixed $g\in G$, we have

$$V\times W \ll V\times W$$
$$(v,w) \maps (gv,gw)$$

Combined with the canonical bilinear map $\varphi: V\times W \ll V\otimes W$, we have

$$V\times W \ll V\otimes W$$
$$(v,w) \maps gv \otimes gw$$

This latter map is still bilinear

$$(\lambda v,w) \maps g(\lambda v) \otimes gw = (\lambda gv) \otimes gw = \lambda gv \otimes gw$$
$$(v,\mu w) \maps gv \otimes g(\mu w) = gv \otimes (\mu gw) = \mu gv \otimes gw$$
$$(v_1 + v_2,w) \maps g(v_1 + v_2) \otimes gw = (gv_1 + gv_2) \otimes gw = gv_1 \otimes gw + gv_2 \otimes gw$$
$$(v,w_1 + w_2) \maps gv \otimes g(w_1 + w_2) = gv \otimes (gw_1 + gw_2) = gv \otimes gw_1 + gv \otimes gw_2$$

so it induces 

$$V\otimes W \ll V\otimes W$$
$$v\otimes w \maps gv \otimes gw$$

and of course, it works well wth the structure of $G$

+++

---

[{symmetric_alternate_products}]

In the same fashion, given

$$\rho: G \ll \GL(V)$$

we have maps

$$\rho_\otimes^k: G \ll \GL\bigl(\bigotimes^k V\bigr)$$
$$v_1 \otimes \cdots \otimes v_k \maps gv_1 \otimes \cdots \otimes gv_k$$

%% to explain further with formal definitions of symmetric and exterior algebras %%

Since these maps work well with symmetrization and anti-symmetrization processes, we also have

$$
\rho_\vee^k: G \ll \GL\bigl(\bigvee^k V\bigr) \qquad
\rho_\wedge^k: G \ll \GL\bigl(\bigwedge^k V\bigr)
$$
$$v_1 \vee \cdots \vee v_k \maps gv_1 \vee \cdots \vee gv_k$$
$$v_1 \wedge \cdots \wedge v_k \maps gv_1 \wedge \cdots \wedge gv_k$$

---

[{dual_representation}]

Representations also reach dual spaces: given

$$\rho: G \ll \GL(V)$$

it is induced 

$$\rho^*: G \ll \GL(V^*)$$
$$\rho^*(g) = \rho(g^{-1})^*: V^* \ll V^*$$

Taking the inverse of $g$ is needed for the product in $G$ to be respected

$$\rho^*(g_1 g_2) = \rho((g_1 g_2)^{-1})^* = \rho(g_2^{-1}g_1^{-1})^* = [\rho(g_2^{-1})\rho(g_1^{-1})]^* = \rho(g_1^{-1})^*\rho(g_2^{-1})^* = \rho^*(g_1)\rho^*(g_2)$$

It also makes sense in order to be compatible with the natural pairing $\langle\quad,\quad\rangle: V^*\times V \ll \C$

$$\langle \rho^*(g)v^*,\rho(g)v\rangle = \langle \rho(g^{-1})^*v^*,\rho(g)v\rangle = \langle v^*,\rho(g^{-1})\rho(g)v\rangle = \langle v^*,\rho(g^{-1}g)v\rangle = \langle v^*,v\rangle$$

That is: the elements of $G$ make $V$ spin, and they also make the elements of $V^*$ spin, in such a way that the natural pairing works well 