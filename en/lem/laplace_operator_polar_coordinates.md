The Laplace operator

$$\Delta=\dfrac{\partial^2}{\partial x^2}+\dfrac{\partial^2}{\partial y^2}$$

is transformed into

$$\Delta=\dfrac{\partial^2 v}{\partial r^2}+\dfrac{1}{r}\dfrac{\partial v}{\partial r}+\dfrac{1}{r^2}\dfrac{\partial^2 v}{\partial\theta^2}$$

in polar coordinates

+++
Proof
+++

Polar coordinates are

$$x=r\cos(\theta),\,y=r\sin(\theta)$$ 
$$r=\sqrt{x^2+y^2},\,\theta=\arctan\left(\dfrac{y}{x}\right)$$

respect to which we have the following partial derivatives

$$\dfrac{\partial r}{\partial x}=\dfrac{x}{r}\qquad\dfrac{\partial r}{\partial y}=\dfrac{y}{r}$$
$$\dfrac{\partial \theta}{\partial x}=\dfrac{-y}{r^2}\qquad\dfrac{\partial \theta}{\partial y}=\dfrac{x}{r^2}$$

Let $u$ and $v$ be the expression of a function with respect to standard and polar coordinates

$$v(r,\theta)=u(x,y)$$

We use the derivatives above and compute

$$\dfrac{\partial u}{\partial x}=\dfrac{\partial v}{\partial r}\dfrac{\partial r}{\partial x}+\dfrac{\partial v}{\partial \theta}\dfrac{\partial \theta}{\partial x}=\dfrac{\partial v}{\partial r}\dfrac{x}{r}+\dfrac{\partial v}{\partial \theta}\dfrac{-y}{r^2}$$

$$
\begin{array}{rcl}
\dfrac{\partial^2 u}{\partial x^2}&=&\left(\dfrac{\partial^2 v}{\partial r^2}\dfrac{\partial r}{\partial x}+\dfrac{\partial^2 v}{\partial \theta\partial r}\dfrac{\partial \theta}{\partial x}\right)\dfrac{x}{r}+\dfrac{\partial v}{\partial r}\dfrac{r-\frac{x}{r}x}{r^2}-
\left(\dfrac{\partial^2 v}{\partial r\partial \theta}\dfrac{\partial r}{\partial x}+\dfrac{\partial^2 v}{\partial\theta^2}\dfrac{\partial \theta}{\partial x}\right)\dfrac{y}{r^2}-\dfrac{\partial v}{\partial \theta}\dfrac{-2r\frac{x}{r}y}{r^4}\\\\
&=&\left(\dfrac{\partial^2 v}{\partial r^2}\dfrac{x}{r}+\dfrac{\partial^2 v}{\partial \theta\partial r}\dfrac{-y}{r^2}\right)\dfrac{x}{r}+\dfrac{\partial v}{\partial r}\dfrac{r-\frac{x}{r}x}{r^2}-
\left(\dfrac{\partial^2 v}{\partial r\partial \theta}\dfrac{x}{r}+\dfrac{\partial^2 v}{\partial\theta^2}\dfrac{-y}{r^2}\right)\dfrac{y}{r^2}-\dfrac{\partial v}{\partial \theta}\dfrac{-2r\frac{x}{r}y}{r^4}\\\\
&=&\dfrac{\partial^2 v}{\partial r^2}\dfrac{x^2}{r^2}-\dfrac{\partial^2 v}{\partial \theta\partial r}\dfrac{xy}{r^3}+\dfrac{\partial v}{\partial r}\dfrac{r^2-x^2}{r^3}-\dfrac{\partial^2 v}{\partial r\partial \theta}\dfrac{xy}{r^3}+\dfrac{\partial^2 v}{\partial\theta^2}\dfrac{y^2}{r^4}+2\dfrac{\partial v}{\partial \theta}\dfrac{xy}{r^4}\\\\
\end{array}
$$

$$\dfrac{\partial u}{\partial y}=\dfrac{\partial v}{\partial r}\dfrac{\partial r}{\partial y}+\dfrac{\partial v}{\partial \theta}\dfrac{\partial \theta}{\partial y}=\dfrac{\partial v}{\partial r}\dfrac{y}{r}+\dfrac{\partial v}{\partial \theta}\dfrac{x}{r^2}$$

$$
\begin{array}{rcl}
\dfrac{\partial^2 u}{\partial y^2}&=&\left(\dfrac{\partial^2 v}{\partial r^2}\dfrac{\partial r}{\partial y}+\dfrac{\partial^2 v}{\partial \theta\partial r}\dfrac{\partial \theta}{\partial y}\right)\dfrac{y}{r}+\dfrac{\partial v}{\partial r}\dfrac{r-\frac{y}{r}y}{r^2}+
\left(\dfrac{\partial^2 v}{\partial r\partial \theta}\dfrac{\partial r}{\partial y}+\dfrac{\partial^2 v}{\partial\theta^2}\dfrac{\partial \theta}{\partial y}\right)\dfrac{x}{r^2}+\dfrac{\partial v}{\partial \theta}\dfrac{-2r\frac{y}{r}x}{r^4}\\\\
&=&\left(\dfrac{\partial^2 v}{\partial r^2}\dfrac{y}{r}+\dfrac{\partial^2 v}{\partial \theta\partial r}\dfrac{x}{r^2}\right)\dfrac{y}{r}+\dfrac{\partial v}{\partial r}\dfrac{r-\frac{y}{r}y}{r^2}+
\left(\dfrac{\partial^2 v}{\partial r\partial \theta}\dfrac{y}{r}+\dfrac{\partial^2 v}{\partial\theta^2}\dfrac{x}{r^2}\right)\dfrac{x}{r^2}+\dfrac{\partial v}{\partial \theta}\dfrac{-2r\frac{y}{r}x}{r^4}\\\\
&=&\dfrac{\partial^2 v}{\partial r^2}\dfrac{y^2}{r^2}+\dfrac{\partial^2 v}{\partial \theta\partial r}\dfrac{xy}{r^3}+\dfrac{\partial v}{\partial r}\dfrac{r^2-y^2}{r^3}+\dfrac{\partial^2 v}{\partial r\partial \theta}\dfrac{xy}{r^3}+\dfrac{\partial^2 v}{\partial\theta^2}\dfrac{x^2}{r^4}-2\dfrac{\partial v}{\partial \theta}\dfrac{xy}{r^4}\\\\
\end{array}
$$

having finally

$$
\begin{array}{rcl}
\Delta u = \dfrac{\partial^2 u}{\partial x^2}+\dfrac{\partial^2 u}{\partial y^2} & = & \dfrac{\partial^2 v}{\partial r^2}\left(\dfrac{x^2}{r^2}+\dfrac{y^2}{r^2}\right)\\\\
& + & \dfrac{\partial^2 v}{\partial r\partial \theta}\left(\dfrac{xy}{r^3}+\dfrac{xy}{r^3}-\dfrac{xy}{r^3}-\dfrac{xy}{r^3}\right)\\\\
& + & \dfrac{\partial v}{\partial r}\left(\dfrac{r^2-x^2}{r^3}+\dfrac{r^2-y^2}{r^3}\right)\\\\
& + & \dfrac{\partial^2 v}{\partial\theta^2}\left(\dfrac{y^2}{r^4}+\dfrac{x^2}{r^4}\right)\\\\
& + & 2\dfrac{\partial v}{\partial \theta}\left(\dfrac{xy}{r^4}-\dfrac{xy}{r^4}\right)\\\\
& = & \dfrac{\partial^2 v}{\partial r^2}+\dfrac{1}{r}\dfrac{\partial v}{\partial r}+\dfrac{1}{r^2}\dfrac{\partial^2 v}{\partial\theta^2}\\\\
\end{array}
$$

+++