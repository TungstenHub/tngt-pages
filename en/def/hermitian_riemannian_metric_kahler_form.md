A **Hermitian metric on a complex vector space $V$** is a map $h:V\times V\longrightarrow \mathbb{C}$ satisfying 

<ol>
<li>$h$ is $\mathbb{R}$-bilinear</li>
<li>$h(\alpha u,v)=\alpha h(u,v)$</li>
<li>$h(u,\alpha v)=\overline{\alpha} h(u,v)$</li>
<li>$h(v,u)=\overline{h(u,v)}$</li>
<li>$h(u,u)\in\mathbb{R}$, $h(u,u)>0$ if $u\neq 0$</li>
</ol>

$\forall u$, $v\in V$, $\alpha\in\mathbb{C}$.

---

A **Hermitian metric on a complex manifold $M$** is a map $h:T^{1,0}M\times T^{1,0}M\longrightarrow\mathbb{C}$ that for each point is a Hermitian metric $h_p:T^{1,0}_p M\times T^{1,0}_p M\longrightarrow\mathbb{C}$.

$h$ is locally determined by the coefficients $h_{jk}=h\left(\dfrac{\partial}{\partial z^j},\dfrac{\partial}{\partial z^k}\right)=\alpha_{jk}+\mathrm{i} \beta_{jk}$; from the Hermiticity we have that $\alpha_{jk}=\alpha_{kj}$, $\beta_{jk}=-\beta_{kj}$.

Likewise, $h$ induces a tensor $\tilde{h}:TM\times TM\longrightarrow \mathbb{C}$ $J$-Hermitian, in the sense that $\tilde{h}(Ju,v)=\mathrm{i}\tilde{h}(u,v)$, $\tilde{h}(u,Jv)=-\mathrm{i}\tilde{h}(u,v)$, defined by $\tilde{h}(u,v)=h(\theta(u),\theta(v))$.

$$
\begin{array}{rrrrr}
\tilde{h}\left(\dfrac{\partial}{\partial x^j},\dfrac{\partial}{\partial x^k}\right) & = & h\left(\dfrac{\partial}{\partial z^j},\dfrac{\partial}{\partial z^k}\right) & = & h_{jk}\\ \\
\tilde{h}\left(\dfrac{\partial}{\partial x^j},\dfrac{\partial}{\partial y^k}\right) & = & h\left(\dfrac{\partial}{\partial z^j},\mathrm{i}\dfrac{\partial}{\partial z^k}\right) & = & -\mathrm{i} h_{jk}\\ \\
\tilde{h}\left(\dfrac{\partial}{\partial y^j},\dfrac{\partial}{\partial x^k}\right) & = & h\left(\mathrm{i}\dfrac{\partial}{\partial z^j},\dfrac{\partial}{\partial z^k}\right) & = & \mathrm{i} h_{jk}\\ \\
\tilde{h}\left(\dfrac{\partial}{\partial y^j},\dfrac{\partial}{\partial y^k}\right) & = & h\left(\mathrm{i}\dfrac{\partial}{\partial z^j},\mathrm{i}d\frac{\partial}{\partial z^k}\right) & = & h_{jk}\\
\end{array}
$$

Therefore, even when $h$ cannot be described as a tensor (it is not $\mathbb{C}$-linear), $\tilde{h}$ is indeed a $\mathbb{C}$-valued tensor over $TM$:

$$\tilde{h}=h_{jk}\mathrm{d} x^j\otimes\mathrm{d} x^k-\mathrm{i} h_{jk}\mathrm{d} x^j\otimes\mathrm{d} y^k+\mathrm{i} h_{jk}\mathrm{d} y^j\otimes\mathrm{d} x^k+h_{jk}\mathrm{d} y^j\otimes\mathrm{d} y^k$$

From $h$ we also obtain a **Riemannian metric** $g:TM\times TM\longrightarrow\mathbb{R}$, $g=\text{Re}(\tilde{h})$ and a 2-form $\omega:TM\times TM\longrightarrow\mathbb{R}$, $\omega=-\text{Im}(\tilde{h})$, called **Kähler form**

$$g=\alpha_{jk}\mathrm{d} x^j\otimes\mathrm{d} x^k+\beta_{jk}\mathrm{d} x^j\otimes\mathrm{d} y^k-\beta_{jk}\mathrm{d} y^j\otimes\mathrm{d} x^k+\alpha_{jk}\mathrm{d} y^j\otimes\mathrm{d} y^k$$

$$\omega=-\beta_{jk}\mathrm{d} x^j\otimes\mathrm{d} x^k-\alpha_{jk}\mathrm{d} x^j\otimes\mathrm{d} y^k+\alpha_{jk}\mathrm{d} y^j\otimes\mathrm{d} x^k+\beta_{jk}\mathrm{d} y^j\otimes\mathrm{d} y^k$$

and the following relations hold

$$h(Ju,Jv)=h(u,v)\qquad g(Ju,Jv)=g(u,v)$$

$$\omega(Ju,Jv)=\omega(u,v)\qquad \omega(u,v)=g(Ju,v)$$

which may be verified after proving them right in the basis elements