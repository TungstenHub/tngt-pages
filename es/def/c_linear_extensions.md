$\tilde{h}$, $g$ y $\omega$ se pueden extender $\mathbb{C}$-linealmente a $TM_\mathbb{C}\times TM_\mathbb{C}\longrightarrow\mathbb{C}$:

$$
\begin{array}{rcl}
\tilde{h} & = &  h_{jk}\mathrm{d} x^j\otimes\mathrm{d} x^k-\mathrm{i} h_{jk}\mathrm{d} x^j\otimes\mathrm{d} y^k+\mathrm{i} h_{jk}\mathrm{d} y^j\otimes\mathrm{d} x^k+h_{jk}\mathrm{d} y^j\otimes\mathrm{d} y^k\\ \\
& = &  h_{jk}\left(\dfrac{\mathrm{d} z^j+\mathrm{d}\bar{z}^j}{2}\right)\otimes\left(\dfrac{\mathrm{d} z^k+\mathrm{d}\bar{z}^k}{2}\right)
-\mathrm{i} h_{jk}\left(\dfrac{\mathrm{d} z^j+\mathrm{d}\bar{z}^j}{2}\right)\otimes\left(\dfrac{\mathrm{d} z^k-\mathrm{d}\bar{z}^k}{2\mathrm{i}}\right)\\ \\
& + & \mathrm{i} h_{jk}\left(\dfrac{\mathrm{d} z^j-\mathrm{d}\bar{z}^j}{2\mathrm{i}}\right)\otimes\left(\dfrac{\mathrm{d} z^k+\mathrm{d}\bar{z}^k}{2}\right)
+h_{jk}\left(\dfrac{\mathrm{d} z^j-\mathrm{d}\bar{z}^j}{2\mathrm{i}}\right)\otimes\left(\dfrac{\mathrm{d} z^k-\mathrm{d}\bar{z}^k}{2\mathrm{i}}\right)\\ \\
& = &\dfrac{1}{4}[(h_{jk}-h_{jk}+h_{jk}-h_{jk})\mathrm{d} z^j\otimes\mathrm{d} z^k
+(h_{jk}+h_{jk}+h_{jk}+h_{jk})\mathrm{d} z^j\otimes\mathrm{d} \bar{z}^k\\ \\
& + & (h_{jk}-h_{jk}-h_{jk}+h_{jk})\mathrm{d} \bar{z}^j\otimes\mathrm{d} z^k
+(h_{jk}+h_{jk}-h_{jk}-h_{jk})\mathrm{d} \bar{z}^j\otimes\mathrm{d} \bar{z}^k]\\ \\
& = & h_{jk}\mathrm{d} z^j\otimes\mathrm{d} \bar{z}^k\\
&&\\
&&\\
g & = & \alpha_{jk}\mathrm{d} x^j\otimes\mathrm{d} x^k+\beta_{jk}\mathrm{d} x^j\otimes\mathrm{d} y^k-\beta_{jk}\mathrm{d} y^j\otimes\mathrm{d} x^k+\alpha_{jk}\mathrm{d} y^j\otimes\mathrm{d} y^k\\ \\
& = & \alpha_{jk}\left(\dfrac{\mathrm{d} z^j+\mathrm{d}\bar{z}^j}{2}\right)\otimes\left(\dfrac{\mathrm{d} z^k+\mathrm{d}\bar{z}^k}{2}\right)
+\beta_{jk}\left(\dfrac{\mathrm{d} z^j+\mathrm{d}\bar{z}^j}{2}\right)\otimes\left(\dfrac{\mathrm{d} z^k-\mathrm{d}\bar{z}^k}{2\mathrm{i}}\right)\\ \\
& - & \beta_{jk}\left(\dfrac{\mathrm{d} z^j-\mathrm{d}\bar{z}^j}{2\mathrm{i}}\right)\otimes\left(\dfrac{\mathrm{d} z^k+\mathrm{d}\bar{z}^k}{2}\right)
+\alpha_{jk}\left(\dfrac{\mathrm{d} z^j-\mathrm{d}\bar{z}^j}{2\mathrm{i}}\right)\otimes\left(\dfrac{\mathrm{d} z^k-\mathrm{d}\bar{z}^k}{2\mathrm{i}}\right)\\ \\
& = & \dfrac{1}{4}[(\alpha_{jk}-\mathrm{i}\beta_{jk}+\mathrm{i}\beta_{jk}-\alpha_{jk})\mathrm{d} z^j\otimes\mathrm{d} z^k
+(\alpha_{jk}+\mathrm{i}\beta_{jk}+\mathrm{i}\beta_{jk}+\alpha_{jk})\mathrm{d} z^j\otimes\mathrm{d}\bar{z}^k\\ \\
& + & (\alpha_{jk}-\mathrm{i}\beta_{jk}-\mathrm{i}\beta_{jk}+\alpha_{jk})\mathrm{d}\bar{z}^j\otimes\mathrm{d} z^k
+(\alpha_{jk}+\mathrm{i}\beta_{jk}-\mathrm{i}\beta_{jk}-\alpha_{jk})\mathrm{d}\bar{z}^j\otimes\mathrm{d}\bar{z}^k]\\ \\
& = & \dfrac{h_{jk}}{2}\mathrm{d} z^j\otimes\mathrm{d}\bar{z}^k+\dfrac{\overline{h_{jk}}}{2}\mathrm{d}\bar{z}^j\otimes\mathrm{d} z^k
= g_{j\bar{k}}\mathrm{d} z^j\otimes\mathrm{d}\bar{z}^k+g_{\bar{j}k}\mathrm{d}\bar{z}^j\otimes\mathrm{d} z^k\\
&&\\
&&\\
\omega & = & -\beta_{jk}\mathrm{d} x^j\otimes\mathrm{d} x^k-\alpha_{jk}\mathrm{d} x^j\otimes\mathrm{d} y^k\alpha_{jk}\mathrm{d} y^j\otimes\mathrm{d} x^k+\beta_{jk}\mathrm{d} y^j\otimes\mathrm{d} y^k\\ \\
& = & -\beta_{jk}\left(\dfrac{\mathrm{d} z^j+\mathrm{d}\bar{z}^j}{2}\right)\otimes\left(\dfrac{\mathrm{d} z^k+\mathrm{d}\bar{z}^k}{2}\right)
-\alpha_{jk}\left(\dfrac{\mathrm{d} z^j+\mathrm{d}\bar{z}^j}{2}\right)\otimes\left(\dfrac{\mathrm{d} z^k-\mathrm{d}\bar{z}^k}{2\mathrm{i}}\right)\\ \\
& + & \alpha_{jk}\left(\dfrac{\mathrm{d} z^j-\mathrm{d}\bar{z}^j}{2\mathrm{i}}\right)\otimes\left(\dfrac{\mathrm{d} z^k+\mathrm{d}\bar{z}^k}{2}\right)
+\beta_{jk}\left(\dfrac{\mathrm{d} z^j-\mathrm{d}\bar{z}^j}{2\mathrm{i}}\right)\otimes\left(\dfrac{\mathrm{d} z^k-\mathrm{d}\bar{z}^k}{2\mathrm{i}}\right)\\ \\
& = & -\dfrac{1}{4}[(\beta_{jk}+\mathrm{i}\alpha_{jk}-\mathrm{i}\alpha_{jk}-\beta_{jk})\mathrm{d} z^j\otimes\mathrm{d} z^k
+(\beta_{jk}-\mathrm{i}\alpha_{jk}-\mathrm{i}\alpha_{jk}+\beta_{jk})\mathrm{d} z^j\otimes\mathrm{d}\bar{z}^k\\ \\
& + & (\beta_{jk}+\mathrm{i}\alpha_{jk}+\mathrm{i}\alpha_{jk}+\beta_{jk})\mathrm{d}\bar{z}^j\otimes\mathrm{d} z^k
+(\beta_{jk}-\mathrm{i}\alpha_{jk}+\mathrm{i}\alpha_{jk}-\beta_{jk})\mathrm{d}\bar{z}^j\otimes\mathrm{d}\bar{z}^k]\\ \\
& = & \dfrac{\mathrm{i} h_{jk}}{2}\mathrm{d} z^j\otimes\mathrm{d}\bar{z}^k-\dfrac{\mathrm{i}\overline{h_{jk}}}{2}\mathrm{d}\bar{z}^j\otimes\mathrm{d} z^k
=\omega_{j\bar{k}}\mathrm{d} z^j\otimes\mathrm{d}\bar{z}^k+\omega_{\bar{j}k}\mathrm{d}\bar{z}^j\otimes\mathrm{d} z^k\\
\end{array}
$$

y de nuevo $\tilde{h}=g-\mathrm{i}\omega$, aunque ahora ya no tiene sentido decir que $g=\text{Re}(\tilde{h})$, $\omega=-\text{Im}(\tilde{h})$ ($g$ y $\omega$ tienen valores complejos). Además, se debe remarcar que viendo la extensión compleja de $\tilde{h}$ como $\tilde{h}:T^{1,0}M\times T^{0,1}M\longrightarrow\mathbb{C}$, entonces $\tilde{h}=h\circ(\text{id}\times c)$ (es como ajustar $h$ para que sea $\mathbb{C}$-lineal y además un tensor).

Vemos además que

$$
\begin{array}{rcl}
\omega & = & \dfrac{\mathrm{i} h_{jk}}{2}\mathrm{d} z^j\otimes\mathrm{d}\bar{z}^k-\dfrac{\mathrm{i}\overline{h_{jk}}}{2}\mathrm{d}\bar{z}^j\otimes\mathrm{d} z^k =\dfrac{\mathrm{i} h_{jk}}{2}\mathrm{d} z^j\otimes\mathrm{d}\bar{z}^k-\dfrac{\mathrm{i}\overline{h_{kj}}}{2}\mathrm{d}\bar{z}^k\otimes\mathrm{d} z^j\\ \\
& = &  \dfrac{\mathrm{i} h_{jk}}{2}(\mathrm{d} z^j\otimes\mathrm{d}\bar{z}^k-\mathrm{d}\bar{z}^k\otimes\mathrm{d} z^j)=\dfrac{\mathrm{i} h_{jk}}{2}\mathrm{d} z^j\wedge\mathrm{d}\bar{z}^k=\omega_{j\bar{k}}\mathrm{d} z^j\wedge\mathrm{d}\bar{z}^k\\
\end{array}
$$

con lo que $\omega$ es una (1,1)-forma