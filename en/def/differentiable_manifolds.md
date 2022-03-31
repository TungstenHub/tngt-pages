A $n$-dimensional **differentiable manifold** is a pair $(X, A)$, where $A$ is a collection of charts $(\varphi_\alpha : V_\alpha \longrightarrow U_\alpha)$ such that the images cover $X$:

$$X = \displaystyle{ \bigcup_\alpha U_\alpha }$$

where $U_a = \varphi_\alpha(V_\alpha)$ and for every pair of charts $ \varphi_\alpha : V_\alpha \rightarrow U_\alpha$ and $\varphi_\beta : V_\beta \rightarrow U_\beta$, the sets $\varphi^{-1}_\beta(U_\alpha \cap U_\beta)\subset \mathbb{R}^n$ and $\varphi^{-1}_\alpha (U_\alpha \cap U_\beta)\subset \mathbb{R}^n$ are open, and the functions  

$$\varphi^{-1}_\alpha \circ \varphi_\beta \: : \:  \varphi^{-1}_\beta(U_\alpha \cap U_\beta) \rightarrow \varphi^{-1}_\alpha (U_\alpha \cap U_\beta)$$

and 

$$\varphi^{-1}_\beta \circ \varphi_\alpha \: : \:  \varphi^{-1}_\alpha(U_\alpha \cap U_\beta) \rightarrow \varphi^{-1}_\beta (U_\alpha \cap U_\beta)$$

are differentiable.