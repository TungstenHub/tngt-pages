Let $M$ be an oriented manifold of dimension $n$ and $\alpha\in\Omega^{n-1}_c(M)$. Then

$$
\int_M \d\alpha=\int_{\partial M}\alpha
$$

where $\partial M$ has the orientation induced as boundary of $M$

+++
Proof
+++

To prove this theorem, we may use the characterization of the integral that makes use of a partition of unity and charts. Due to the linearity, it is enough to prove the theorem in the very special case in which $\alpha$ is a $(n-1)$-form in $\R ^n_+=\{(x_1,x_2,\cdots,x_n)| x_1\geqslant 0\}$.

{{ image | stokes_theorem_chart }}

$\alpha$ is of the form $\sum f_i \d x_1\wedge\cdots\wedge \d x_{i-1}\wedge\d x_{i+1}\wedge\cdots\wedge \d x_n$ with $f_i$ identically zero outside some compact set and $\d\alpha=\sum (-1)^{i-1}\dfrac{\partial f_i}{\partial x_i} \d x_1\wedge\cdots\wedge\d x_n$. Integrating one variable at a time in a sufficiently large parallelepiped we obtain

$$
\int_{\R ^n_+}\d\alpha=\int_{\R ^n_+}\sum (-1)^{i-1}\dfrac{\partial f_i}{\partial x_i}= \int_{\R ^n_+}\dfrac{\partial f_1}{\partial x_1}=-\int_{\partial\R ^n_+}f_1= \int_{\partial\R ^n_+}\alpha,
$$

where the last change of sign is due to the fact that the orientation that $\partial\R^n_+$ inherits from $\R^n_+$ is not the usual one ($e_1$ is ingoing, not outgoing)

+++