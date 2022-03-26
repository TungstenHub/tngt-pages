Let $h$ be a Hermitian metric on a complex manifold. The metric makes the manifold Kähler if and only if in each point $x$ of $M$ there exist holomorphic coordinates in which $h$ approximates the standard Hermitian metric up to second order, that is,

$$h_{jk}=\delta_{jk}+2r_{jk}$$

$$g_{j\bar{k}}=\dfrac{1}{2}\delta_{jk}+r_{jk}$$

with $r_{jk}(x)=0$, $\dfrac{\partial r_{jk}}{\partial z^l}(x)=\dfrac{\partial r_{jk}}{\partial \bar{z}^l}(x)=0$

+++
Proof
+++

First suppose that in each point we have holomorphic coordinates in which the metric matches the standard Hermitian metric up to order 2. Then

$$\omega=\ii g_{j\bar{k}}\d z^j\wedge\d z^{\bar{k}}\qquad g_{j\bar{k}}=\dfrac{1}{2}\delta_{jk}+r_{jk}$$ 

$$\d\omega=\ii\dfrac{\partial g_{j\bar{k}}}{\partial z^l}\d z^l\wedge\d z^j\wedge\d z^{\bar{k}}+\ii\dfrac{\partial g_{j\bar{k}}}{\partial \bar{z}^l}\d \bar{z}^l\wedge\d z^j\wedge\d z^{\bar{k}}$$

that vanishes in $x$. Since $x$ is any point, $\d\omega=0$ and the metric is Kähler.

Conversely, suppose that the metric is Kähler. Let $x\in M$; let's take some orthonormal basis of $T_{x}M$ of the form $\{e_1,\ldots,e_n,Je_1,\ldots,Je_n\}$ and a holomorphic chart $\{z^j=x^j+\ii y^j\}$ around $x$ such that

$$e_j=\dfrac{\partial}{\partial x^j}(x)\qquad Je_j=\dfrac{\partial}{\partial y^j}(x)$$

The Kähler form may be expressed as

$$\omega=\ii\left(\dfrac{1}{2}\delta_{jk}+a_{jkl}z^l+a_{jk\bar{l}}\bar{z}^l+o(d(x,z))\right)\d z^j\wedge\d\bar{z}^k=\ii g_{j\bar{k}}\d z^j\wedge\d\bar{z}^k$$

Since $g_{j\bar{k}}=\overline{g_{k\bar{j}}}$,

$$a_{jk\bar{l}}=\overline{a_{kjl}}$$

and if $\d\omega=0$, then

$$a_{jkl}=a_{lkj},\qquad a_{jk\bar{l}}=a_{jl\bar{k}}$$

according to the identities

$$\dfrac{\partial g_{j\bar{k}}}{\partial z^l}=\dfrac{\partial g_{l\bar{k}}}{\partial z^j},\quad \dfrac{\partial g_{j\bar{k}}}{\partial \bar{z}^l}=\dfrac{\partial g_{j\bar{l}}}{\partial \bar{z}^k}$$

Now we're looking for a change of coordinates in which first order terms vanish. Let

$$z^j=w^j+\dfrac{1}{2}b_{jkl}w^k w^l$$

where $b_{jkl}$ are complex numbers such that $b_{jkl}=b_{jlk}$ (so that the computations are easier). This change of coordinates is well-defined thanks to the holomorphic version of the Inverse Function Theorem. Now

$$\d z^j=\d w^j+b_{jkl}w^k\d w^l$$

and in this way

$$
\begin{array}{rcl}
\omega & = & \ii\left(\dfrac{1}{2}\delta_{jk}+a_{jkl}z^l+a_{jk\bar{l}}\bar{z}^l+o(d)\right)\d z^j\wedge\d\bar{z}^k\\
& = & \ii\left(\dfrac{1}{2}\delta_{jk}+a_{jkl}w^l+a_{jk\bar{l}}\bar{w}^l+o(d)\right)(\d w^j+b_{jst}w^s\d w^t)\wedge(\d\bar{w}^k+\overline{b_{kst}}\bar{w}^s\d\bar{w}^t)\\
& = & \ii\left(\dfrac{1}{2}\delta_{jk}+a_{jkl}w^l+a_{jk\bar{l}}\bar{w}^l+ b_{klj}w^l+\overline{b_{jlk}}\bar{w}^l+o(d)\right)\d w^j\wedge\d\overline{w}^k\\
\end{array}
$$

If we choose $b_{klj}=-a_{jkl}$ (that is possible because $a_{jkl}$ is symmetric in $j$ and $l$), then

$$\overline{b_{jlk}}=-\overline{a_{kjl}}=-a_{jk\bar{l}}$$

and therefore

$$\omega=\ii\left(\dfrac{1}{2}\delta_{jk}+o(d)\right)\d w^j\wedge\d\bar{w}^k$$

+++