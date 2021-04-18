Let's compute the Levi-Civita connection in a Kähler manifold. To simplify notation, we'll denote $\partial_{j}=\dfrac{\partial}{\partial z^j}$, $\partial_{\overline{j}}=\dfrac{\partial}{\partial \bar{z}^j}$.

The connection is described by the Christoffel symbols:

$$\nabla_{\partial_{j}}\partial_{k}=\Gamma_{jk}^l\partial_{l}+\Gamma_{jk}^{\bar{l}}\partial_{\overline{l}} \qquad \nabla_{\partial_{j}}\partial_{\overline{k}}=\Gamma_{j\bar{k}}^l\partial_{l}+\Gamma_{j\bar{k}}^{\bar{l}}\partial_{\overline{l}}$$

$$\nabla_{\partial_{\overline{j}}}\partial_{k}=\Gamma_{\bar{j}k}^l\partial_{l}+\Gamma_{\bar{j}k}^{\bar{l}}\partial_{\overline{l}} \qquad \nabla_{\partial_{\overline{j}}}\partial_{\overline{k}}=\Gamma_{\bar{j}\bar{k}}^l\partial_{l}+\Gamma_{\bar{j}\bar{k}}^{\bar{l}}\partial_{\overline{l}}$$

Since $\nabla J=0$, $\nabla_v(Jw)=(\nabla_v J)(w)+J(\nabla_v w)=J(\nabla_v w)$. Then,

$$
\begin{array}{rcrclcccccccl}
%%%
\ii(\Gamma_{jk}^l\partial_{l}+\Gamma_{jk}^{\bar{l}}\partial_{\overline{l}}) & = & \ii\nabla_{\partial_{j}}\partial_{k} & = &\nabla_{\partial_{j}}(\ii\partial_{k}) & = & \nabla_{\partial_{j}}(J\partial_{k}) & = &J(\nabla_{\partial_{j}}\partial_{k}) & = & J(\Gamma_{jk}^l\partial_{l}+\Gamma_{jk}^{\bar{l}}\partial_{\overline{l}}) & = & \ii\Gamma_{jk}^l\partial_{l}-\ii\Gamma_{jk}^{\bar{l}}\partial_{\overline{l}}\\\\
%%%
-\ii(\Gamma_{j\bar{k}}^l\partial_{l}+\Gamma_{j\bar{k}}^{\bar{l}}\partial_{\overline{l}}) & = & -\ii\nabla_{\partial_{j}}\partial_{\overline{k}} & = & \nabla_{\partial_{j}}(-\ii\partial_{\overline{k}}) & = & \nabla_{\partial_{j}}(J\partial_{\overline{k}}) & = & J(\nabla_{\partial_{j}}\partial_{\overline{k}}) & = & J(\Gamma_{j\bar{k}}^l\partial_{l}+\Gamma_{j\bar{k}}^{\bar{l}}\partial_{\overline{l}}) & = & \ii\Gamma_{j\bar{k}}^l\partial_{l}-\ii\Gamma_{j\bar{k}}^{\bar{l}}\partial_{\overline{l}}\\\\
%%%
\ii(\Gamma_{\bar{j}k}^l\partial_{l}+\Gamma_{\bar{j}k}^{\bar{l}}\partial_{\overline{l}}) & = & \ii\nabla_{\partial_{\overline{j}}}\partial_{k} & = & \nabla_{\partial_{\overline{j}}}(\ii\partial_{k}) & = & \nabla_{\partial_{\overline{j}}}(J\partial_{k}) & = & J(\nabla_{\partial_{\overline{j}}}\partial_{k}) & = & J(\Gamma_{\bar{j}k}^l\partial_{l}+ \Gamma_{\bar{j}k}^{\bar{l}}\partial_{\overline{l}}) & = & \ii\Gamma_{\bar{j}k}^l\partial_{l}-\ii\Gamma_{\bar{j}k}^{\bar{l}}\partial_{\overline{l}}\\\\
%%%
-\ii(\Gamma_{\bar{j}\bar{k}}^l\partial_{l}+\Gamma_{\bar{j}\bar{k}}^{\bar{l}}\partial_{\overline{l}}) & = & -\ii\nabla_{\partial_{\overline{j}}}\partial_{\overline{k}} & = & \nabla_{\partial_{\overline{j}}}(-\ii\partial_{\overline{k}}) & = & \nabla_{\partial_{\overline{j}}}(J\partial_{\overline{k}}) & = & J(\nabla_{\partial_{\overline{j}}}\partial_{\overline{k}}) & = & J(\Gamma_{\bar{j}\bar{k}}^l\partial_{l}+ \Gamma_{\bar{j}\bar{k}}^{\bar{l}}\partial_{\overline{l}}) & = & \ii\Gamma_{\bar{j}\bar{k}}^l\partial_{l}-\ii\Gamma_{\bar{j}\bar{k}}^{\bar{l}}\partial_{\overline{l}}\\\\
%%%
\end{array}
$$

and therefore $\Gamma_{jk}^{\bar{l}}=\Gamma_{j\bar{k}}^l=\Gamma_{\bar{j}k}^{\bar{l}}=\Gamma_{\bar{j}\bar{k}}^l=0$, and due to the symmetry, also $\Gamma_{j\bar{k}}^{\bar{l}}=\Gamma_{\bar{j}k}^{l}=0$.

On the other hand, 

$$\dfrac{\partial g_{k\bar{m}}}{\partial z^j}=\dfrac{\partial}{\partial z^j}g(\partial_{k},\partial_{\overline{m}})=g(\nabla_{\partial_{j}}\partial_{k},\partial_{\overline{m}})+g(\partial_{k},\nabla_{\partial_{j}}\partial_{\overline{m}})=g(\Gamma_{jk}^l\partial_{l},\partial_{\overline{m}})=\Gamma_{jk}^l g_{l\bar{m}}$$

$$\dfrac{\partial g_{\bar{k}m}}{\partial \bar{z}^{j}}=\dfrac{\partial}{\partial \bar{z}^{j}}g(\partial_{\overline{k}},\partial_{m})=g(\nabla_{\partial_{\overline{j}}}\partial_{\overline{k}},\partial_{m})+g(\partial_{\overline{k}},\nabla_{\partial_{\overline{j}}}\partial_{m})=g(\Gamma_{\bar{j}\bar{k}}^{\bar{l}}\partial_{\overline{l}},\partial_{m})=\Gamma_{\bar{j}\bar{k}}^{\bar{l}} g_{\bar{l}m}$$

and in the end

$$\Gamma_{jk}^l=g^{l\bar{m}}\dfrac{\partial g_{k\bar{m}}}{\partial z^j}=g^{l\bar{m}}\dfrac{\partial g_{j\bar{m}}}{\partial z^k}$$

$$\Gamma_{\bar{j}\bar{k}}^{\bar{l}}= g^{\bar{l}m}\dfrac{\partial g_{\bar{k}m}}{\partial \bar{z}^{j}}= g^{\bar{l}m}\dfrac{\partial g_{\bar{j}m}}{\partial \bar{z}^{k}}=\overline{\Gamma_{jk}^l}$$ 

$$\Gamma_{ab}^c=0\qquad\text{otherwise}$$