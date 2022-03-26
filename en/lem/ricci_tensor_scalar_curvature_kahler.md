The Ricci tensor is obtained by taking the trace of the curvature tensor: $R_{ab}=g^{cd}R_{acbd}$. For the coefficient to be non-zero, $a$ and $c$ must be of distinct type (in the decomposition $T^{1,0}M$, $T^{0,1}M$), and likewise $b$ and $d$, $c$ and $d$, so $a$ and $b$ must be of distinct type too. So due to the symmetry, the only coefficient to be computed is essentially

$$
\begin{array}{rcl}
R_{j\bar{k}} & = & g^{l\bar{m}}R_{j\bar{m}\bar{k}l}\\\\
& & \qquad \text{[Bianchi ident.]}\\\\
& = & -g^{l\bar{m}}R_{j\bar{k}l\bar{m}}\\\\
& = & -g^{l\bar{m}}\left (\dfrac{\partial ^2 g_{l\bar{m}}}{\partial z^j \partial \bar{z}^k}-g^{s\bar{t}}\dfrac{\partial g_{l\bar{t}}}{\partial z^j}\dfrac{\partial g_{s\bar{m}}}{\partial \bar{z}^k}\right)\\\\
& = & -g^{l\bar{m}}\dfrac{\partial ^2 g_{l\bar{m}}}{\partial z^j \partial \bar{z}^k}-\dfrac{\partial g^{s\bar{m}}}{\partial z^j}\dfrac{\partial g_{s\bar{m}}}{\partial \bar{z}^k}\\\\
\end{array}
$$

On the other hand,

$$\dfrac{\partial ^2}{\partial z^j \partial \bar{z}^k}(\log \det g)=\dfrac{\partial}{\partial z^j}\left (\dfrac{1}{\det g}\det g g^{l\bar{m}}\dfrac{\partial g_{l\bar{m}}}{\partial \bar{z}^k}\right)=g^{l\bar{m}}\dfrac{\partial ^2 g_{l\bar{m}}}{\partial z^j \partial \bar{z}^k}+\dfrac{\partial g^{l\bar{m}}}{\partial z^j}\dfrac{\partial g_{l\bar{m}}}{\partial \bar{z}^k}$$

from where

$$R_{j\bar{k}}=-\dfrac{\partial ^2}{\partial z^j \partial \bar{z}^k}(\log \det g)$$

and the scalar curvature is 

$$Sc=g^{j\bar{k}}R_{j\bar{k}}=-g^{j\bar{k}}\dfrac{\partial ^2}{\partial z^j \partial \bar{z}^k}(\log \det g)$$