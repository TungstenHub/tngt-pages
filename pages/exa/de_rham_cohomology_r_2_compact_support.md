Differential forms in $\R ^2$ and the actuation of $\d$ are as before, but now $f$, $g$, $h$ and $k$ have compact support

---

$\text{ker }\d_0$ requires again the functions $f$ to be constant, but since compact support is also required, it turns out that $\text{ker }\d_0=\{f\equiv 0\}$ and

$$H^0_c(\R ^2)=\dfrac{\{f\equiv 0\}}{0}=0$$

---

For the next group, it was initially proposed the function 

$$ f(x,y)=\int_0^x f_x(t,0)\d t+\int_0^y f_y(x,t)\d t=\int_0^x g(t,0)\d t+\int_0^y h(x,t)\d t$$

that satisfied $\d f=g\d x+h\d y$, so every closed 1-form was exact. The issue is that $f$ may not have compact support even when $g$ and $h$ do. But this is easily fixed: if $g$ and $h$ are zero outside some compact set $[-M,M] \times[-M,M]$, there it is also true that 

$$\dfrac{\partial f}{\partial x}=g=0$$ 
$$\dfrac{\partial f}{\partial y}=h=0$$

so $f$ is constant in $\R ^2\smallsetminus [-M,M] \times[-M,M]$ (which is connected). So we may redefine $f$ substracting this constant, so that it is also zero outside $[-M,M] \times[-M,M]$. Therefore, in the compact case every closed 1-form is exact too, and

$$H^1_c(\R ^2)=0$$

---

Here comes the true difference: $H^2_c(\R ^2)$ is not trivial. In the non-compact case, from the 2-form $k\d x\wedge\d y$ we had taken 

$$g=0,\qquad h(x,y)=\int_0^x k(t,y)\d t$$

for $\dfrac{\partial h}{\partial x}-\dfrac{\partial g}{\partial y}=k$, but now it now it is very rare that $h$ has compact support. Can we choose $g$ and $h$ more wisely? Well, in fact, hardly ever...

The major obstruction is when $\int_{\R ^2} k(x,y)\neq 0$. Imagine that $g$ and $h$ are zero outside some $K=[-M,M] \times[-M,M]$ (and its boundary). Then

$$
\begin{array}{rcl}
\displaystyle\int_{\R ^2} k(x,y)=\int_K k(x,y) & = & \displaystyle\int_{-M}^M \int_{-M}^M \dfrac{\partial h}{\partial x} \d x \d y-\int_{-M}^M \int_{-M}^M \dfrac{\partial g}{\partial y} \d y \d x\\
& = & \displaystyle\int_{-M}^M \bigl[h(x,y)\bigr]_{x=-M}^{x=M}\, \d y-\int_{-M}^M \bigl[g(x,y)\bigr]_{y=-M}^{y=M}\, \d x\\
& = & 0
\end{array}
$$

so if $\int_{\R ^2} k(x,y)\neq 0$ there's nothing to do: $k\d x\wedge\d y$ is automatically closed, but it's not exact. And what if $\int_{\R ^2} k(x,y)=0$? We'll try the approach above and modify it if needed. Let 

$$h(x,y)=\int_{-M}^x k(t,y)\d t$$

Above, below and to the left of $K$, $h$ is identically zero, whereas to the right it equates some function $v(y)$ with support in $[-M,M]$. To correct this anomaly, let's take a differentiable function $\rho(x)$ that values 0 in $(-\infty,-M]$ and 1 in $[M,\infty)$, and we switch to

$$\tilde{h}(x,y)=h(x,y)-\rho(x)v(y)$$

which now has compact support! But this change comes at a cost that we expect to compensate with $g$:

$$\dfrac{\partial \tilde{h}}{\partial x}=\dfrac{\partial h}{\partial x}-\rho'(x)v(y)=k-\rho'(x)v(y)$$

and we need $\dfrac{\partial g}{\partial y}=-\rho'(x)v(y)$, and we're forced to take 

$$g(x,y)=\int_{-M}^y -\rho'(x)v(t)\d t=-\rho'(x)\int_{-M}^y v(t)\d t$$

Great! $g$ is zero outside $K$, also above it, because 

$$\int_{-M}^M v(t)\d t=\int_{\R ^2} k(x,y)=0$$

Since $\int_{\R ^2} k(x,y)$ determines the exactness of the 2-form, there is one degree of freedom and

$$H^2_c(\R ^2)\simeq\R $$