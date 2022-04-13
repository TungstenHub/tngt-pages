[{a}]

$$<<< \int e^x\cos x\dd x$$

+++
Solución
+++

$$<<< 
\int e^x\cos x\dd x
\\ \qquad 
\oveq{ u=\cos x\quad u'=-\sin x\\ v'=e^x\quad v=e^x }
e^x\cos x-\int -e^x\sin x\dd x
\\ \qquad 
= e^x\cos x+\int e^x\sin x\dd x
\\ \qquad 
\oveq{ u=\sin x\quad u'=\cos x\\ v'=e^x\quad v=e^x }
e^x\cos x+e^x\sin x-\int e^x\cos x\dd x
\\ \qquad 
\Longrightarrow \int e^x\cos x\dd x=
\hl{\dfrac{1}{2}e^x(\cos x+\sin x)+k}
$$

Las dos veces hemos asignado la parte trigonométrica a $u$ y la parte exponencial a $v$. Si cambiamos de roles también funciona:

$$<<< 
\int e^x\cos x\dd x
\\ \qquad 
\oveq{ u=e^x\quad u'=e^x\\ v'=\cos x\quad v=\sin x }
e^x\sin x-\int e^x\sin x\dd x
\\ \qquad 
\oveq{ u=e^x\quad u'=e^x\\ v'=\sin x\quad v=-\cos x }
e^x\sin x-\left(-e^x\cos x-\int -e^x\cos x\dd x\right)
\\ \qquad 
= e^x\sin x+e^x\cos x-\int e^x\cos x\dd x
\\ \qquad 
\Longrightarrow \int e^x\cos x\dd x=
\hl{\dfrac{1}{2}e^x(\cos x+\sin x)+k}
$$

_Pero mezclando roles no funciona:_

$$<<< 
\int e^x\cos x\dd x
\\ \qquad 
\oveq{ u=\cos x\quad u'=-\sin x\\ v'=e^x\quad v=e^x }
e^x\cos x-\int -e^x\sin x\dd x
\\ \qquad 
= e^x\cos x+\int e^x\sin x\dd x
\\ \qquad 
\oveq{ u=e^x\quad u'=e^x\\ v'=\sin x\quad v=-\cos x }
e^x\cos x-e^x\cos x-\int -e^x\cos x\dd x
\\ \qquad 
= \int e^x\cos x\dd x
$$

porque nos sale la misma integral con la que empezamos

+++

---
[{b}]

$$<<< \int e^{ax}\cos (bx)\dd x$$

+++
Solución
+++

$$<<< 
\int e^{ax}\cos (bx)\dd x
\\ \qquad 
\oveq{ u=\cos (bx)\quad u'=-b\sin (bx)\\ v'=e^{ax}\quad v=\frac{1}{a}e^{ax} }
\dfrac{1}{a}e^{ax}\cos (bx)-\int -\dfrac{b}{a}e^{ax}\sin (bx)\dd x
\\ \qquad 
= \dfrac{1}{a}e^{ax}\cos (bx)+\dfrac{b}{a}\int e^{ax}\sin (bx)\dd x
\\ \qquad 
\oveq{ u=\sin (bx)\quad u'=b\cos (bx)\\ v'=e^{ax}\quad v=\frac{1}{a}e^{ax} }
\dfrac{1}{a}e^{ax}\cos (bx)+\dfrac{b}{a^2}e^{ax}\sin (bx)-\dfrac{b^2}{a^2}e^{ax}\cos (bx)\dd x
\\ \qquad 
\Longrightarrow 
\int e^x\cos x\dd x=\dfrac{1}{1+\frac{b^2}{a^2}}\left(\dfrac{1}{a}e^{ax}\cos (bx)+\dfrac{b}{a^2}e^{ax}\sin (bx) \right)
\\ \qquad 
= \hl{\dfrac{1}{a^2+b^2}e^{ax}(a\cos (bx)+b\sin (bx))+k}
$$

Este resultado se puede obtener de un modo más informal, pero a la vez muy bonito, por medio de la identidad de Euler en la exponencial compleja: 

$$e^{(a+bi)x}=e^{ax}(\cos(bx)+i\sin(bx))$$

Integrando ambas partes, 

$$\dfrac{1}{a+bi}e^{(a+bi)x}+k=\int e^{(a+bi)x}\dd x=\int e^{ax}\cos (bx)\dd x + i\int e^{ax}\sin (bx)\dd x$$

pero 

$$
\begin{array}{rcl}
\dfrac{1}{a+bi}e^{(a+bi)x} & = & \dfrac{1}{a+bi}\dfrac{a-bi}{a-bi}e^{ax}(\cos(bx)+i\sin(bx))\\[1em]
& = & \dfrac{1}{a^2+b^2}e^{ax}(a-bi)(\cos(bx)+i\sin(bx))\\[1em]
& = & \dfrac{1}{a^2+b^2}e^{ax}(a\cos(bx)+b\sin(bx)) \\[1em]
& + & i\dfrac{1}{a^2+b^2}e^{ax}(a\sin(bx)-b\cos(bx))
\end{array}
$$

y al igualar parte real y parte imaginaria nos queda

$$\int e^{ax}\cos (bx)\dd x=\dfrac{1}{a^2+b^2}e^{ax}(a\cos(bx)+b\sin(bx))+k$$
$$\int e^{ax}\sin (bx)\dd x=\dfrac{1}{a^2+b^2}e^{ax}(a\sin(bx)-b\cos(bx))+k$$

derivación verdaderamente notable

+++

---
[{c}]

$$<<< \int \cos(\ln x)\dd x$$

+++
Solución
+++

$$<<< 
\int \cos(\ln x)\dd x
\\ \qquad 
\oveq{ u=\cos(\ln x)\quad u'=-\sin(\ln x)\frac{1}{x}\\ v'=1\quad v=x }
x\cos(\ln x) - \int-\sin(\ln x)\frac{1}{x}x\dd x
\\ \qquad 
= x\cos(\ln x) + \int\sin(\ln x)\dd x
\\ \qquad 
\oveq{ u=\sin(\ln x)\quad u'=\cos(\ln x)\frac{1}{x}\\ v'=1\quad v=x }
x\cos(\ln x) + x\sin(\ln x) - \int\cos(\ln x)\frac{1}{x}x\dd x
\\ \qquad 
\Longrightarrow \int \cos(\ln x)\dd x =
\hl{\dfrac{1}{2}x\left(\cos(\ln x)+\sin(\ln x)\right) + k}
$$

Sorprendentemente, un cambio de variable $e^t=x$, $e^t\dd t=\d x$ nos llevaría a $\int e^t\cos t\dd t$, que se resuelve con la misma técnica de la doble integración por partes

+++