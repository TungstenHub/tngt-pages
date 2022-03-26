How to describe $\d_\nabla$ in a chart? Let 

$$\sigma=\vect{\sigma^1, \sigma^2, \vdots, \sigma^k}=\sigma^i e_i:U_\alpha\longrightarrow\R^k$$

be a section (everything is analogous for $\C^k$) 

$$\d_\nabla(\sigma)=\d_\nabla(\sigma^i e_i)=\d(\sigma^i)\otimes e_i+\sigma^i\d_\nabla e_i$$

The first part may be symbolically expressed as

$$
\vect{\d\sigma^1, \d\sigma^2, \vdots, \d\sigma^k}=\d\vect{\sigma^1, \sigma^2, \vdots, \sigma^k}=\d(\sigma)
$$ 

as long as we keep in mind that this is component-wise derivation, non-intrinsic but chart-dependent. In the second part we find terms $\d_\nabla e_i$, which are really defining the derivative. Let $\d_\nabla e_i=\omega_i^j\otimes e_j$, where $\omega_i^j$ are 1-forms. We then get

$$
\sigma^i\d_\nabla e_i=\sigma^i\omega_i^j\otimes e_j=\vect{\sigma^i\omega_i^1, \sigma^i\omega_i^2, \vdots, \sigma^i\omega_i^k}=
\begin{pmatrix}
\omega_1^1 & \omega_2^1 & \cdots & \omega_k^1 \\
\omega_1^2 & \omega_2^2 & \cdots & \omega_k^2 \\
\vdots     & \vdots     & \ddots & \vdots     \\
\omega_1^k & \omega_2^k & \cdots & \omega_k^k \\
\end{pmatrix}\vect{\sigma^1, \sigma^2, \vdots, \sigma^k}=A\sigma
$$

with $A$ 1-form-valued matrix. Summing up, we may simbolically write $\d_\nabla\sigma=(\d+A)\sigma$, the first term acting component-wise, the second acting like matrix product