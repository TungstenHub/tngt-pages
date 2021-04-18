Let's work with the curvature tensor: 

$$R(u,v)w=\nabla_v\nabla_u w-\nabla_u\nabla_v w+\nabla_{[u,v]}w=(\nabla_{v,u}^2-\nabla_{u,v}^2)w$$ 

$$R(u,v,w,x)=g(R(u,v)w,x)$$

Since $J$ is parallel, it holds that $R(u,v)Jw=JR(u,v)w$, and hence $R(u,v,Jw,Jx)=R(u,v,w,x)$. For this equality and for the symmetries of the curvature tensor, it happens that when describing $R$ in local coordinates, the only terms to be computed are $R_{j\bar{k}l\bar{m}}=R(\partial_{j},\partial_{\overline{k}},\partial_{l},\partial_{\overline{m}})$. Now

$$
\begin{array}{rcl}
R(\partial_{j},\partial_{\overline{k}})\partial_{l} & = & \nabla_{\partial_{\overline{k}}}\nabla_{\partial_{j}} \partial_{l}-\nabla_{\partial_{j}}\nabla_{\partial_{\overline{k}}} \partial_{l}+\nabla_{[\partial_{j},\partial_{\overline{k}}]}\partial_{l}\\\\
& = & \nabla_{\partial_{\overline{k}}}\nabla_{\partial_{j}} \partial_{l}=\nabla_{\partial_{\overline{k}}}(\Gamma_{jl}^s \partial_{s})\\\\
& = & \dfrac{\partial \Gamma_{jl}^s}{\partial \bar{z}^k}\partial_{s}+\Gamma_{jl}^s\nabla_{\partial_{\overline{k}}} \partial_{s}\\\\
& = & \dfrac{\partial \Gamma_{jl}^s}{\partial \bar{z}^k}\partial_{s}\\\\
& & \\\\
{R_{j\bar{k}l}}^s & = & \dfrac{\partial \Gamma_{jl}^s}{\partial \bar{z}^k}\\\\
\end{array}
$$

and also

$$
\begin{array}{rcl}
g(R(\partial_{j},\partial_{\overline{k}})\partial_{l},\partial_{\overline{m}}) & = & \dfrac{\partial \left(g^{s\bar{t}}\dfrac{\partial g_{l\bar{t}}}{\partial z^j}\right)}{\partial \bar{z}^k}g_{s\bar{m}}\\\\
& = & \left(\dfrac{\partial g^{s\bar{t}}}{\partial \bar{z}^k} \dfrac{\partial g_{l\bar{t}}}{\partial z^j}+g^{s\bar{t}}\dfrac{\partial ^2 g_{l\bar{t}}}{\partial z^j \partial \bar{z}^k}\right)g_{s\bar{m}}\\\\
& = & g_{s\bar{m}}\dfrac{\partial g^{s\bar{t}}}{\partial \bar{z}^k} \dfrac{\partial g_{l\bar{t}}}{\partial z^j}+\dfrac{\partial ^2 g_{l\bar{m}}}{\partial z^j \partial \bar{z}^k}\\\\
\end{array}
$$

In general, 

$$0=\dfrac{\partial \delta_d^b}{\partial z^c}=\dfrac{\partial g_{ad}g^{ab}}{\partial z^c}=g^{ab}\dfrac{\partial g_{ad}}{\partial z^c}+g_{ad}\dfrac{\partial g^{ab}}{\partial z^c}$$ 

so $\dfrac{\partial g^{ab}}{\partial z^c}=-g^{ad}g^{eb}\dfrac{\partial g_{ed}}{\partial z^c}$. Therefore, 

$$g_{s\bar{m}}\dfrac{\partial g^{s\bar{t}}}{\partial \bar{z}^k}=-g_{s\bar{m}}g^{s\bar{q}}g^{p\bar{t}}\dfrac{\partial g_{p\bar{q}}}{\partial \bar{z}^k}=-g^{p\bar{t}}\dfrac{\partial g_{p\bar{m}}}{\partial \bar{z}^k}$$

and finally

$$R_{j\bar{k}l\bar{m}}=\dfrac{\partial ^2 g_{l\bar{m}}}{\partial z^j \partial \bar{z}^k}-g^{s\bar{t}}\dfrac{\partial g_{l\bar{t}}}{\partial z^j}\dfrac{\partial g_{s\bar{m}}}{\partial \bar{z}^k}$$