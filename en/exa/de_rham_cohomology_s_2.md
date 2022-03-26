The case of the sphere $\S^2$ will be substantially more difficult than the previous ones. The ideas developed, however, will be key when studying Poincaré Lemma and Mayer-Vietoris sequences

Let's consider the sphere $\S^2\subset\R^3$ together with the two charts coming from the stereographic projection from the poles $N=(0,0,1)$ and $S=(0,0,-1)$. The domains of both charts are $\R^2$, and the images are the open sets $U=\S^2-\{N\}$, $V=\S^2-\{S\}$; let $W=U\cap V=\S^2-\{N,S\}$.

---

Let $f\in C^\infty(\S^2)$ with $\d f=0$. $f$ induce the restrictions $f_1=f|_U$, $f_2=f|_V$, which are identified with functions of domain $\R^2$. But according to [the cohomology of $\R^2$]( exa | de_rham_cohomology_r_2 ), $\d f_1=0$ and $\d f_2=0$ imply that $f_1$ and $f_2$ are constant, and since they coincide in the common domain $W$, $f$ has to be constant

$$H^0(\S^2)=\dfrac{\text{ker }\d_0}{\text{im }\d_{-1}}=\dfrac{\{f=cte\in\R\}}{0}\simeq\R$$

---

Now let $\alpha$ be a 1-form in $\S^2$ with $\d\alpha=0$. The restriction of $\alpha$ to $U$, $V$ induces the 1-forms $\alpha_1$ and $\alpha_2$, whose exterior derivative is also zero. Since $H^1(\R^2)=0$, closed 1-forms are exact and there exist functions $f_1$ and $f_2$ in $U$, $V$ with $\d f_1=\alpha_1$, $\d f_2=\alpha_2$. But how compatible are $f_1$ and $f_2$ in $W$? Here's the trick: in $W$, $\d(f_1-f_2)=\d f_1-\d f_2=\alpha_1-\alpha_2=\alpha-\alpha=0$. The exterior derivative of $f_1-f_2$ is 0 in $W$ and $W$ is connected, so $f_1-f_2$ is indeed some constant $c\in\R$. We define $\tilde{f}_2=f_2+c$, which stills satisfy $\d \tilde{f}_2=\alpha_2$, and now $f_1=\tilde{f}_2$ in $W$, so we may consider

$$f=
\begin{cases}
f_1 & \text{en $U$}\\
\tilde{f}_2 & \text{en $V$}
\end{cases}$$

This function satisfies $\d f=\alpha$, since it already does in $U$, $V$. Therefore 

$$H^1(\S^2)=\dfrac{\text{ker }\d_1}{\text{im }\d_0}=0$$

---

This is the subtle part. Let $\beta$ a 2-form in $\S^2$. Its domain is a manifold of dimension 2, so its exterior derivative is zero, and the same holds for $\beta_1=\beta|_U$, $\beta_2=\beta|_V$. Again $H^2(\R^2)=0$, and there exist suitable 1-forms $\alpha_1$, $\alpha_2$ defined in $U$, $V$ with $\d \alpha_i=\beta_i$. Now, how do $\alpha_1$ and $\alpha_2$ interact in the common domain $W$? $\d(\alpha_1-\alpha_2)=\d\alpha_1-\d\alpha_2=\beta_1-\beta_2=\beta-\beta=0$. But since we know nothing about the first cohomology group of $W$, we can't say anithing about its closed 1-forms. So let's study the cohomology of $W$ quickly

We may parameterize $W$ with $(\theta,z)\longmapsto(\sqrt{1-z^2}\cos(\theta),\sqrt{1-z^2}\sin(\theta),z)$, $(\theta,z)\in\R\times(-1,1)$. This induces the 1-forms $\d \theta$, $\d z$, and the functions $C^\infty(W)$ match the functions $f(\theta,z)$ which are differentiable and $2\pi$-periodic in $\theta$, which in turn admit the Fourier series representation $f(\theta,z)=\sum_{n}f_{n}(z)\ee^{\ii n\theta}$.

Let $\alpha=g\d \theta+h\d z$

$$\d \alpha=\left(\dfrac{\partial h}{\partial \theta}-\dfrac{\partial g}{\partial z}\right)\d \theta\wedge\d z=\sum_{n}(\ii nh_n(z)-g_n'(z))\ee^{\ii n\theta}\d \theta\wedge\d z$$

and for $\alpha$ to be closed it is required $\ii nh_n(z)=g_n'(z)$ for all $n$. Now we're looking for some $f=\sum_{n}f_{n}(z)\ee^{\ii n\theta}$ with $\d f=\alpha$, that is, $\dfrac{\partial f}{\partial \theta}=g$, $\dfrac{\partial f}{\partial z}=h$, or equivalently, $\ii nf_n(z)=g_n(z)$, $f_n'(z)=h_n(z)$. If $n\neq 0$, there is no problem in taking $f_n(z)=\frac{g_n(z)}{\ii n}$ and everything is fine, because $f_n'(z)=\frac{g_n'(z)}{\ii n}=\frac{\ii nh_n(z)}{\ii n}=h_n(z)$. For $n=0$, $\ii 0h_0(z)=g_0'(z)$ holds when $g_0=c\in\R$ is constant. But if $c\neq 0$, the condition $\ii 0f_0(z)=g_0(z)=c$ cannot be satisfied. On the other hand, this is the only obstruction: if we correct $g$ with $c=0$, then it is enough to take $f_0(z)=\int_0^{z} h_0(t)\d t$. So $H^1(W)\simeq\R$, depending on the choice of $c$, and a generator of the group is the class of the 1-form $\d \theta$, which we will denote $\gamma$ from now on

We have studied part of the cohomology of $W$, now for the sphere. We had $\d(\alpha_1-\alpha_2)=0$; now we know that $\alpha_1-\alpha_2=\lambda\gamma+\d f$ for some $\lambda\in\R$ and some function $f$ in $W$. Suppose for a moment that $\lambda=0$; in this case we'll find a global $\alpha$ with $\d \alpha=\beta$. But before we have to introduce two functions _of compact support_

Let $\rho_1$ and $\rho_2$ be two positive differentiable functions defined in $[-1,1]$ such that $\rho_1$ is zero in $[1/3,1]$, $\rho_2$ is zero in $[-1,-1/3]$ and $\rho_1+\rho_2=1$. When applying this functions to the height of the sphere we get another two functions (that will again be denoted $\rho_1$ and $\rho_2$) such that the first has its support contained in $U$ and the second has its support contained in $V$, that, $\{\rho_1,\rho_2\}$ is a differentiable partition of unity subordinate to the open cover $\{U,V\}$

{{ image | compact_support_functions }}

Why is this going to be useful? For extensibility reasons. The function $f$ may be non-extendable to the poles. But: if we define $f_1=f\rho_2$ and $f_2=f\rho_1$ (note the change of indexes!) and extend by zero, then $f_1$ is a differentiable function in $U$, $f_2$ is a differentiable function in $V$ and $f_1+f_2=f$ in $W$

{{ image | compact_support_transformation }}

Great! Let $\tilde{\alpha}_1=\alpha_1-\d f_1$, $\tilde{\alpha}_2=\alpha_2+\d f_2$. It is still true that $\d \tilde{\alpha}_1=\beta_1$ and $\d \tilde{\alpha}_2=\beta_2$, but now $\tilde{\alpha}_1-\tilde{\alpha}_2=\alpha_1-\d f_1-\alpha_2-\d f_2=\d f-\d(f_1+f_2)=0$ in $W$. So we end up with a global form 

$$\alpha=
\begin{cases}
\tilde{\alpha}_1 & \text{en $U$}\\
\tilde{\alpha}_2 & \text{en $V$}
\end{cases}$$

that satisfies $\d \alpha=\beta$ n $\S^2$. That, $\alpha_1$ and $\alpha_2$ could be non-extensible, but we have managed to correct this non-extensibility

If $\lambda\neq 0$, this process is not possible: if there is some global $\alpha$, 

$$
\begin{array}{rl}
\d(\alpha-\alpha_1)=\beta-\beta_1=0 \Longrightarrow \alpha-\alpha_1=\d f_1 & \qquad\text{in $U$, for some $f_1$} \\
\d(\alpha-\alpha_2)=\beta-\beta_2=0 \Longrightarrow \alpha-\alpha_2=\d f_2 & \qquad\text{in $V$, for some $f_2$} \\
\alpha_1-\alpha_2=\alpha-\d f_1 -\alpha+\d f_2=\d (f_2-f_1) & \qquad\text{in $W$} \\
\end{array}
$$

but we had $\alpha_1-\alpha_2=\lambda\gamma+\d f$, and we know that $\gamma$ is not the exterior derivative of any function

To definitely establish that there exist closed and non-exact 2-forms in the sphere, we have to finde some $\beta$ for which, with the induced $\alpha_i$, $\alpha_1-\alpha_2=\lambda\gamma+\d f$ with $\lambda\neq 0$. Let $\beta_1=\d(\rho_2\gamma)$, $\beta_2=\d(\rho_1\gamma)$. In $W$,

$$\beta_1+\beta_2=\d(\rho_2\gamma+\rho_1\gamma)=\d \gamma=0$$

and we may define 

$$\beta=
\begin{cases}
\beta_1 & \text{en $U$}\\
-\beta_2 & \text{en $V$}
\end{cases}$$ 

The induced 1-forms are, up to the derivative of a function, $\alpha_1=\rho_2\gamma$ and $\alpha_2=-\rho_1\gamma$, and 

$$\alpha_1-\alpha_2=(\rho_2+\rho_1)\gamma=\gamma\leadsto\lambda=1$$

Now it is sure that

$$H^2(\S^2)=\dfrac{\text{ker }\d_2}{\text{im }\d_1}\simeq\R$$

because the exactness of the closed 2-form $\beta$ depends on the induced coefficient $\lambda$

---

One explicit generator of $H^2(\S^2)$ could be $\d\theta\wedge\d z$, which happens to match the surface measure of the sphere as subset of $\R^3$