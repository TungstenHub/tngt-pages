Let $M$ be a manifold. Then

$$H^\ast(M\times \R )\simeq H^\ast(M)$$
$$H^\ast_c(M\times \R )\simeq H_c^{\ast-1}(M)$$

+++
Proof
+++

The case with general cohomology comes directly from the fact that $M$ and $M\times\R$ have the same homotopy type. We may take as homotopic inverses the las projection $p:(x,t)\longmapsto x$ and section $s:x\longmapsto (x,0)$ maps; in this setting 

$$s^\ast:(\beta+\d t\wedge\alpha)\longmapsto \beta(0)$$
$$p^\ast:\beta\longmapsto \beta+\d t\wedge 0$$ 

($\beta$ independient of $t$) provide an isomorphism in cohomology

The compact support scenario is completely different; there is no functoriality and the lemma is indeed different: $H^\ast_c(M\times \R )\simeq H_c^{\ast-1}(M)$ means $H^k_c(M\times \R )\simeq H_c^{k-1}(M)$ for all $k$). We'll have to come up with a different, direct approach

Forms in $M\times \R $ are still of the type $\beta+\d t\wedge\alpha$, but now $\beta$ and $\alpha$ have compact support in $M\times \R$. Let's consider the following homomorphism: 

$$\pi:\Omega^k_c(M\times \R )\longrightarrow \Omega_c^{k-1}(M)$$
$$\pi(\beta+\d t\wedge\alpha)=\int_{\R }\alpha$$

The integral in well-defined because $\alpha$ has compact support along the fiber $x\times\R$, and since the support of $\int_{\R }\alpha$ is (contained in) the projection of the support of $\alpha$, the image in indeed in $\Omega_c^{k-1}(M)$. We assert that it induces another map $\pi:H^k_c(M\times \R )\longrightarrow H_c^{k-1}(M)$ that is isomorfism

First of all, $\pi$ is well-defined for cohomology:

$$\d \pi(\beta+\d t\wedge\alpha)=\d\left(\int_{\R }\alpha\right)=\int_{\R }\d\alpha$$
$$\pi\bar{\d}(\beta+\d t\wedge\alpha)=\pi\left(\d\beta+\d t\wedge\left(\dfrac{\partial \beta}{\partial t}-\d \alpha\right)\right)= \int_{\R }\left(\dfrac{\partial \beta}{\partial t}-\d \alpha\right)=-\int_{\R }\d\alpha$$

because $\displaystyle\int_{\R }\dfrac{\partial \beta}{\partial t}=\int_{-R}^R\dfrac{\partial \beta}{\partial t}=\beta(R)-\beta(-R)=0$ for $R$ big enough ($\beta$ has compact support in each fiber). So $\d \pi=-\pi\bar{\d}$; it's not the equality $\d \pi=\pi\bar{\d}$ required for $\pi$ to be a complex homomorphism, but it is enough for $\pi$ to be well-defined in cohomology: closed forms map to closed forms, exact forms map to exact forms

On the one hand, we have another homomorfism 

$$\sigma:\Omega_c^{k-1}(M)\longrightarrow \Omega_c^k(M\times\R )$$
$$\alpha\longmapsto \rho(t)\d t\wedge\alpha$$

where $\rho$ is some compact support function in $\R $ with $\displaystyle\int_\R \rho=1$. And it happens $\pi\circ\sigma=\text{id}_{\Omega_c^{k-1}(M)}$ and similarly $\pi\circ\sigma=\text{id}_{H_c^{k-1}}(M)$ in cohomology. In particular $\pi$ is surjective

To check that $\pi$ in injective (for cohomology), let's consider some closed form $\beta+\d t\wedge\alpha\longmapsto \displaystyle\int_{\R }\alpha$, and suppose that $\displaystyle\int_{\R }\alpha=\d \gamma$ is exact; is the starting form also exact? Let's study the composition of a hypothetical form whose exterior derivative is $\beta+\d t\wedge\alpha$

$$\bar{\d}(\delta+\d t\wedge \cdots)=\d \delta+\d t\wedge\cdots\Longrightarrow \beta=\d \delta$$

But we shouldn't forget that $\beta+\d t\wedge\alpha$ is closed:

$$\bar{\d}(\beta+\d t\wedge\alpha)=\left(\d\beta+\d t\wedge\left(\dfrac{\partial \beta}{\partial t}-\d \alpha\right)\right)=0\Longrightarrow 
\begin{cases}
\d\beta=0\\
\dfrac{\partial \beta}{\partial t}-\d \alpha=0
\end{cases}$$
$$\d\alpha=\dfrac{\partial \beta}{\partial t}=\dfrac{\partial \d \delta}{\partial t}=\d \dfrac{\partial \delta}{\partial t}$$

and it seems reasonable to think that $\dfrac{\partial \delta}{\partial t}=\alpha$, so we define $\delta=\int_{-\infty}^t\alpha$. For this choice, 

$$\bar{\d}\delta=\d\delta+\d t\wedge\dfrac{\partial \delta}{\partial t}=\d \int_{-\infty}^t\alpha+\d t\wedge\dfrac{\partial }{\partial t}\int_{-\infty}^t\alpha=\int_{-\infty}^t\d\alpha+\d t\wedge\alpha=\int_{-\infty}^t\dfrac{\partial \beta}{\partial t}+\d t\wedge\alpha=\beta+\d t\wedge\alpha$$

exactly as required. But: this form has compact support as to the projection on $M$, but as to the $\R$ direction, $\delta$ may be nonzero beyond the support of $\alpha$: 

$$\delta(R)=\int_{-\infty}^R\alpha=\d \gamma$$ 

for $R$ big enough. So we add a correction: 

$$\delta-\rho(t)\d \gamma-\d t\wedge\dfrac{\partial \rho(t)}{\partial t}\gamma$$

where $\rho$ is a differentiable function equal to 0 in $(-\infty,-1]$ and equal to 1 in $[1,\infty)$. $\rho(t)\d \gamma$ corrects $\delta$ and $\dfrac{\partial \rho(t)}{\partial t}$ has compact support; moreover 

$$\bar{\d}\left(\rho(t)\d \gamma+\d t\wedge\dfrac{\partial \rho(t)}{\partial t}\gamma\right)=\d(\rho(t)\d \gamma)+\d t\wedge\left(\dfrac{\partial \rho(t)}{\partial t}\d\gamma-\d\left(\dfrac{\partial \rho(t)}{\partial t}\gamma\right)\right)=0$$

This argument is not replicable in the non-compact case: $\displaystyle\int_{-\infty}^t\alpha$ may diverge, and if $\displaystyle\delta=\int_{0}^t\alpha$, then $\d \delta=\beta-\beta(0)$, which requires some additional $\delta_0$ satisfying $\d \delta_0=\beta(0)$, i.e. again everything points out the cohomology of $M$ of the same order

+++