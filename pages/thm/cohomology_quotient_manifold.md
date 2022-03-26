Let $\tilde{M}=M/G$. If $G$ is finite, the map $\pi^*$ is injective and its image is 

$$
H^k(M)^G=\{[\alpha]\in H^k(M)\quad|\quad\varphi_g^*[\alpha]=[\alpha]\quad\forall g\in G\}
$$

+++
Proof
+++

The proof has three steps:

<ol>
  <li>
  **$\pi^*$ is injective**

  Suppose $\pi^*[\alpha]=0$

  $$\pi^*[\alpha]=0\Longrightarrow \exists \beta|\pi^*\alpha=\mathrm{d}\beta$$

  The form $\pi^*\alpha$ is compatible with the transformations of $G$ (that is, $\varphi_g^*(\pi^*\alpha)= (\pi\circ\varphi_g)^*\alpha=\pi^*\alpha$), but perhaps $\beta$ is not. So we'll take an average: 

  $$\tilde{\beta}=\frac{1}{l}\sum_{g\in G}\varphi_g^*\beta$$

  where $l$ is the number of elements in $G$. Then 

  $$\mathrm{d}\tilde{\beta}=\frac{1}{l}\sum_g\mathrm{d}\varphi_g^*\beta=\frac{1}{l}\sum_g\varphi_g^*\mathrm{d}\beta=\frac{1}{l}\sum_g\varphi_g^*\pi^*\alpha=\frac{1}{l}\sum_g\pi^*\alpha=\pi^*\alpha$$ 

  and also

  $$\varphi_g^*\tilde{\beta}=\frac{1}{l}\sum_{g'}\varphi_{gg'}^*\beta=\tilde{\beta}$$

  So $\tilde{\beta}$ is compatible with $G$; this implies that $\tilde{\beta}=\pi^*\hat{\beta}$ for some $\hat{\beta}\in \Omega^{k-1}(M)$. And now

  $$\pi^*\alpha=\mathrm{d}\beta=\mathrm{d}\tilde{\beta}= \mathrm{d}\pi^*\hat{\beta}=\pi^*\mathrm{d}\hat{\beta}\Longrightarrow \alpha=\mathrm{d}\hat{\beta}\Longrightarrow[\alpha]=0$$ 

  because $\pi$ is local diffeomorphism
  </li>

  <li>
  **$\text{im }\pi^*\subset H^k(M)^G$**

  $\varphi_g^*(\pi^*[\alpha])= (\pi\circ\varphi_g)^*[\alpha]=\pi^*[\alpha]$
  </li>

  <li>
  **$\text{im }\pi^*\supset H^k(M)^G$**

  Let $[\beta]\in H^k(M)^G\Longrightarrow \varphi_g^*[\beta]=[\beta]$. Again, we take an average: 

  $$\tilde{\beta}=\frac{1}{l}\sum_g\varphi_g^*\beta$$ 

  $\tilde{\beta}$ is closed: 

  $$\mathrm{d}\tilde{\beta}=\frac{1}{l}\sum_g\mathrm{d}\varphi_g^*\beta= \frac{1}{l}\sum_g\varphi_g^*\mathrm{d}\beta=0$$

  and as before, it is compatible with $G$, so $\tilde{\beta}=\pi^*\hat{\beta}$. But then $\pi^*[\hat{\beta}]=[\tilde{\beta}]=\frac{1}{l}\sum_g[\beta]=[\beta]$
  </li>
</ol>

+++