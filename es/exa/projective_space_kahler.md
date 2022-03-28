The projective space $\C P^n$ has a special metric, the Fubini-Study metric, in which projectivities are isometries. It is described by a Kähler potential in each affine chart: 

$$\mathcal{K}=\log(1+|z|^2)$$

where every other coefficients of the metric follows:

$$h_{jk}=2\dfrac{\partial ^2}{\partial z_j\partial \bar{z}_k}\log(1+|z|^2)=2\dfrac{\partial }{\partial z_j}\left(\dfrac{z_k}{1+|z|^2}\right)=2\dfrac{\delta_{jk}(1+|z|^2)-\bar{z}_j z_k}{(1+|z|^2)^2}$$

$$\tilde{h}=2\sum_{jk}\dfrac{\partial ^2}{\partial z_j\partial \bar{z}_k}\log(1+|z|^2)\d z_j\otimes\d\bar{z}_k$$

$$g=\sum_{jk}\left(\dfrac{\partial ^2}{\partial z_j\partial \bar{z}_k}\log(1+|z|^2)\d z_j\otimes\d\bar{z}_k+\dfrac{\partial ^2}{\partial \bar{z}_j\partial z_k}\log(1+|z|^2)\d\bar{z}_j\otimes\d z_k\right)$$

$$\omega=\ii\sum_{jk}\left(\dfrac{\partial ^2}{\partial z_j\partial \bar{z}_k}\log(1+|z|^2)\d z_j\otimes\d\bar{z}_k-\dfrac{\partial ^2}{\partial \bar{z}_j\partial z_k}\log(1+|z|^2)\d\bar{z}_j\otimes\d z_k\right)=\ii\partial\bar{\partial}\log(1+|z|^2)$$

To compute the Christoffel symbols and other curvature coefficients may be very difficult, so we'll try an indirect approach. Instead of deriving directly, we'll compute the determinant of the metric.

$$
g=(g_{j\bar{k}})_{jk}=\left(\dfrac{\partial ^2}{\partial z_j\partial \bar{z}_k}\log(1+|z|^2)\right)_{jk}=\dfrac{1}{(1+|z|^2)^2}(\delta_{jk}(1+|z|^2)-\bar{z}_j z_k)_{jk}=\dfrac{-1}{(1+|z|^2)^2}(B-(1+|z|^2)I)
$$
$$
B=
\begin{pmatrix}
\bar{z}_1 z_1 & \cdots & \bar{z}_1 z_n \\
\vdots        & \ddots & \vdots        \\
\bar{z}_n z_1 & \cdots & \bar{z}_n z_n \\
\end{pmatrix}
$$

This way, 

$$\det g=\left(\dfrac{-1}{(1+|z|^2)^2}\right)^n\det(B-(1+|z|^2)I)=\left(\dfrac{-1}{(1+|z|^2)^2}\right)^n P_B(1+|z|^2)$$  

where $P_B(\lambda)=\det(B-\lambda I)$ is the characteristic polynomial of $B$. But how is this characteristic polynomial? Since $B$ has rank 1, it has the eigenvalue 0 with multiplicity $n-1$, so in fact 

$$P_B(\lambda)=(-1)^n \lambda^{n-1}(\lambda-\text{tr} B)$$

(since the trace comes with the term of degree $n-1$), and in the end 

$$\det g=\left(\dfrac{-1}{(1+|z|^2)^2}\right)^n(-1)^n(1+|z|^2)^{n-1}(1+|z|^2-|z|^2)=\dfrac{1}{(1+|z|^2)^{n+1}}$$

Having found the determinant, we have the Ricci tensor and form 

$$\rho=-\ii\partial\bar{\partial}\log\det g=\ii(n+1)\partial\bar{\partial}\log(1+|z^2|)=(n+1)\omega$$

and in the same way

$$R_{j\bar{k}}=(n+1)g_{j\bar{k}}$$

That is, the Fubini-Study metric in $\C P^n$ is Einstein with constant $n+1$, and in particular has constant scalar curvature

$$Sc=(n+1)g^{j\bar{k}}g_{j\bar{k}}=n(n+1)$$