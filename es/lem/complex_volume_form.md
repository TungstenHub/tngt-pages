The metrics are described by the following matrices:

$$
g_{\R}=\begin{pmatrix}
\alpha_{11} & \beta_{11} & \cdots & \alpha_{1n} & \beta_{1n}\\
-\beta_{11} & \alpha_{11}& \cdots & -\beta_{1n} & \alpha_{1n}\\
\cdots & \cdots & \cdots & \cdots & \cdots\\
\cdots & \cdots & \cdots & \cdots & \cdots\\
\alpha_{n1} & \beta_{n1} & \cdots & \alpha_{nn} & \beta_{nn}\\
-\beta_{n1} & \alpha_{n1}& \cdots & -\beta_{nn} & \alpha_{nn}\\
\end{pmatrix}
$$

$$
g_{\C}=\begin{pmatrix}
0 & g_{1\bar{1}} & \cdots & 0 & g_{1\bar{n}}\\
g_{\bar{1}1} & 0& \cdots & g_{\bar{1}n} & 0\\
\cdots & \cdots & \cdots & \cdots & \cdots\\
\cdots & \cdots & \cdots & \cdots & \cdots\\
0 & g_{n\bar{1}} & \cdots & 0 & g_{n\bar{n}}\\
g_{\bar{n}1} & 0& \cdots & g_{\bar{n}n} & 0\\
\end{pmatrix}
$$

$$
C=\begin{pmatrix}
\dfrac{1}{2}  & \dfrac{1}{2}   &&&\\
\dfrac{-\ii}{2} & \dfrac{\ii}{2} &&&\\
&&\ddots&&\\
&&&\dfrac{1}{2} & \dfrac{1}{2}\\
&&&\dfrac{-\ii}{2}  & \dfrac{\ii}{2}\\
\end{pmatrix}
$$

$$
g=\begin{pmatrix}
g_{1\overline{1}} &  \cdots & g_{1\overline{n}} \\
\vdots&\ddots&\vdots\\
g_{n\overline{1}} & \cdots & g_{n\overline{n}}\\
\end{pmatrix}
$$

$g_{\R}$ expresses the metric with respect to $\left\{\dfrac{\partial}{\partial x^1},\dfrac{\partial}{\partial y^1},...,\dfrac{\partial}{\partial x^n},\dfrac{\partial}{\partial y^n}\right\}$, whereas $g_{\C}$ expresses it with respect to $\left\{\dfrac{\partial}{\partial z^1},\dfrac{\partial}{\partial \bar{z}^1},...,\dfrac{\partial}{\partial z^n},\dfrac{\partial}{\partial \bar{z}^n}\right\}$. $C$ is the basis change matrix, and $g_{\C}=C^{T}g_{\R}C$, as may be checked blockwise:  

$$
\begin{pmatrix}
\dfrac{1}{2} & \dfrac{-\ii}{2}\\
\dfrac{1}{2} & \dfrac{\ii}{2}\\
\end{pmatrix}
\begin{pmatrix}
\alpha_{jk}  & \beta_{jk} \\
-\beta_{jk}  & \alpha_{jk} \\
\end{pmatrix}
\begin{pmatrix}
\dfrac{1}{2} & \dfrac{1}{2}\\
\dfrac{-\ii}{2} & \dfrac{\ii}{2}\\
\end{pmatrix}=
\begin{pmatrix}
\dfrac{1}{2} & \dfrac{-\ii}{2}\\
\dfrac{1}{2} & \dfrac{\ii}{2}\\
\end{pmatrix}
\begin{pmatrix}
\dfrac{\overline{h_{jk}}}{2} & \dfrac{h_{jk}}{2}\\
\dfrac{-\ii\bar{h}_{jk}}{2} & \dfrac{\ii h_{jk}}{2}\\
\end{pmatrix}=
\begin{pmatrix}
0 & \dfrac{h_{jk}}{2}\\
\dfrac{\overline{h_{jk}}}{2} & 0\\
\end{pmatrix}=
\begin{pmatrix}
0 & g_{j\bar{k}}\\
g_{\bar{j}k} & 0\\
\end{pmatrix}
$$

In particular, 

$$\det g_{\C}=\det g_{\R}(\det C)^2=\left(\dfrac{\ii}{2}\right)^{2n}\det g_{\R}$$

Moreover, according to the properties of the determinant,

$$\det g_{\C}=(-1)^n\det\begin{pmatrix}
g_{1\overline{1}} &  \cdots & g_{1\overline{n}} \\
\vdots&\ddots&\vdots\\
g_{n\overline{1}} & \cdots & g_{n\overline{n}}\\
\end{pmatrix}
\det\begin{pmatrix}
g_{\overline{1}1} &  \cdots & g_{\overline{1}n} \\
\vdots&\ddots&\vdots\\
g_{\overline{n}1} & \cdots & g_{\overline{n}n}\\
\end{pmatrix}$$ 

but since the last two matrices are transpose of each other,

$$\det g_{\C}=(-1)^n(\det g)^2$$

The volume form is therefore

$$
\begin{array}{rcl}
\d V & = & \sqrt{\det g_{\R}}\dfrac{\partial}{\partial x^1}\wedge\dfrac{\partial}{\partial y^1}\wedge...\wedge\dfrac{\partial}{\partial x^n}\wedge\dfrac{\partial}{\partial y^n}\\\\
& = & \left(\dfrac{2}{\ii}\right)^n\sqrt{\det g_{\C}}\left(\dfrac{\ii}{2}\right)^n\dfrac{\partial}{\partial z^1}\wedge\dfrac{\partial}{\partial \bar{z}^1}\wedge...\wedge\dfrac{\partial}{\partial z^n}\wedge\dfrac{\partial}{\partial \bar{z}^n}\\\\
& = & \sqrt{\det g_{\C}}\dfrac{\partial}{\partial z^1}\wedge\dfrac{\partial}{\partial \bar{z}^1}\wedge...\wedge\dfrac{\partial}{\partial z^n}\wedge\dfrac{\partial}{\partial \bar{z}^n}\\\\
& = & \ii^n\det g \dfrac{\partial}{\partial z^1}\wedge\dfrac{\partial}{\partial \bar{z}^1}\wedge...\wedge\dfrac{\partial}{\partial z^n}\wedge\dfrac{\partial}{\partial \bar{z}^n}\\\\
\end{array}
$$

Also 

$$
\begin{array}{rcl}
\omega\wedge\overset{n}{\cdots}\wedge\omega\left(\dfrac{\partial}{\partial z^1},\dfrac{\partial}{\partial \bar{z}^1},...,\dfrac{\partial}{\partial z^n},\dfrac{\partial}{\partial \bar{z}^n}\right) & = & \ii^n\left(\sum_{j_1\bar{k}_1}g_{j_1\bar{k}_1}\d z^{j_1}\wedge\d 
\bar{z}^{k_1}\right)\wedge\cdots\wedge\left(\sum_{j_n\bar{k}_n}g_{j_n\bar{k}_n}\d z^{j_n}\wedge\d\bar{z}^{k_n}\right)\left(\dfrac{\partial}{\partial z^1},\dfrac{\partial}{\partial \bar{z}^1},...,\dfrac{\partial}{\partial z^n},\dfrac{\partial}{\partial \bar{z}^n}\right)\\\\
& = & \ii^n\sum g_{j_1\bar{k}_1}\cdots g_{j_n\bar{k}_n}\d z^{j_1}\wedge\d\bar{z}^{k_1}\wedge\cdots \wedge\d z^{j_n}\wedge\d\bar{z}^{k_n}\left(\dfrac{\partial}{\partial z^1},\dfrac{\partial}{\partial \bar{z}^1},...,\dfrac{\partial}{\partial z^n},\dfrac{\partial}{\partial \bar{z}^n}\right)\\\\
&   & \qquad\text{[the term is zero unless \(\{j_1,...,j_n\}\) and \(\{k_1,...,k_n\}\) are permutations of \(\{1,...,n\}\)]}\\\\
& = & \ii^n\sum_{\sigma\tau}(-1)^{\sigma}(-1)^{\tau}g_{\sigma(1)\overline{\tau(1)}}\cdots g_{\sigma(n)\overline{\tau(n)}}\\\\
&   & \qquad[\rho=\sigma^{-1}\tau]\\\\
& = & \ii^n n!\sum_{\rho}(-1)^{\rho}g_{1\overline{\rho(1)}}\cdots g_{n\overline{\rho(n)}}\\\\
& = & \ii^n n!\det g\\\\
\end{array}
$$

and therefore

$$ \omega^n=n!\d V$$