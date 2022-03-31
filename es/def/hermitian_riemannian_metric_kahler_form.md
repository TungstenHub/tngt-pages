Una **métrica hermítica en un espacio vectorial complejo $V$** es una aplicación $h:V\times V\longrightarrow \mathbb{C}$ que satisface 

<ol>
<li>$h$ es $\mathbb{R}$-bilineal</li>
<li>$h(\alpha u,v)=\alpha h(u,v)$</li>
<li>$h(u,\alpha v)=\overline{\alpha} h(u,v)$</li>
<li>$h(v,u)=\overline{h(u,v)}$</li>
<li>$h(u,u)\in\mathbb{R}$, $h(u,u)>0$ si $u\neq 0$</li>
</ol>

$\forall u$, $v\in V$, $\alpha\in\mathbb{C}$.

---

Una **métrica hermítica en una variedad compleja $M$** es una aplicación $h:T^{1,0}M\times T^{1,0}M\longrightarrow\mathbb{C}$ tal que para cada punto es una métrica hermítica $h_p:T^{1,0}_p M\times T^{1,0}_p M\longrightarrow\mathbb{C}$.

$h$ está localmente determinada por los coeficientes $h_{jk}=h\left(\dfrac{\partial}{\partial z^j},\dfrac{\partial}{\partial z^k}\right)=\alpha_{jk}+\mathrm{i} \beta_{jk}$; de la hermiticidad tenemos que $\alpha_{jk}=\alpha_{kj}$, $\beta_{jk}=-\beta_{kj}$.

Del mismo modo, $h$ induce un tensor $\tilde{h}:TM\times TM\longrightarrow \mathbb{C}$ $J$-hermítico, en el sentido de que $\tilde{h}(Ju,v)=\mathrm{i}\tilde{h}(u,v)$, $\tilde{h}(u,Jv)=-\mathrm{i}\tilde{h}(u,v)$, definido por $\tilde{h}(u,v)=h(\theta(u),\theta(v))$.

$$
\begin{array}{rrrrr}
\tilde{h}\left(\dfrac{\partial}{\partial x^j},\dfrac{\partial}{\partial x^k}\right) & = & h\left(\dfrac{\partial}{\partial z^j},\dfrac{\partial}{\partial z^k}\right) & = & h_{jk}\\ \\
\tilde{h}\left(\dfrac{\partial}{\partial x^j},\dfrac{\partial}{\partial y^k}\right) & = & h\left(\dfrac{\partial}{\partial z^j},\mathrm{i}\dfrac{\partial}{\partial z^k}\right) & = & -\mathrm{i} h_{jk}\\ \\
\tilde{h}\left(\dfrac{\partial}{\partial y^j},\dfrac{\partial}{\partial x^k}\right) & = & h\left(\mathrm{i}\dfrac{\partial}{\partial z^j},\dfrac{\partial}{\partial z^k}\right) & = & \mathrm{i} h_{jk}\\ \\
\tilde{h}\left(\dfrac{\partial}{\partial y^j},\dfrac{\partial}{\partial y^k}\right) & = & h\left(\mathrm{i}\dfrac{\partial}{\partial z^j},\mathrm{i}d\frac{\partial}{\partial z^k}\right) & = & h_{jk}\\
\end{array}
$$

Así, incluso cuando $h$ no se puede describir como un tensor (no es $\mathbb{C}$-lineal), $\tilde{h}$ es de hecho un tensor $\mathbb{C}$-valuado sobre $TM$:

$$\tilde{h}=h_{jk}\mathrm{d} x^j\otimes\mathrm{d} x^k-\mathrm{i} h_{jk}\mathrm{d} x^j\otimes\mathrm{d} y^k+\mathrm{i} h_{jk}\mathrm{d} y^j\otimes\mathrm{d} x^k+h_{jk}\mathrm{d} y^j\otimes\mathrm{d} y^k$$

De $h$ obtenemos también una **métrica riemanniana** $g:TM\times TM\longrightarrow\mathbb{R}$, $g=\text{Re}(\tilde{h})$ y una 2-forma $\omega:TM\times TM\longrightarrow\mathbb{R}$, $\omega=-\text{Im}(\tilde{h})$, llamada **forma de Kähler**

$$g=\alpha_{jk}\mathrm{d} x^j\otimes\mathrm{d} x^k+\beta_{jk}\mathrm{d} x^j\otimes\mathrm{d} y^k-\beta_{jk}\mathrm{d} y^j\otimes\mathrm{d} x^k+\alpha_{jk}\mathrm{d} y^j\otimes\mathrm{d} y^k$$

$$\omega=-\beta_{jk}\mathrm{d} x^j\otimes\mathrm{d} x^k-\alpha_{jk}\mathrm{d} x^j\otimes\mathrm{d} y^k+\alpha_{jk}\mathrm{d} y^j\otimes\mathrm{d} x^k+\beta_{jk}\mathrm{d} y^j\otimes\mathrm{d} y^k$$

y se tienen las siguientes relaciones

$$h(Ju,Jv)=h(u,v)\qquad g(Ju,Jv)=g(u,v)$$

$$\omega(Ju,Jv)=\omega(u,v)\qquad \omega(u,v)=g(Ju,v)$$

que se pueden verificar si se prueban en los elementos de la base