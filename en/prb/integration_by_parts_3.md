[{a}]

$$<<< \int e^x\cos x\dd x$$

+++
Solution
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

Both times we have assigned the trigonometric part to $u$ and the exponential part to $v$. Switching roles works too:

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

_But mixing roles would not work:_

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

having the very same integral we began with

+++

---
[{b}]

$$<<< \int e^{ax}\cos (bx)\dd x$$

+++
Solution
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

This result may be obtained in a much less formal, but certainly very beautiful way, by means of Euler's identity on complex exponentiation: 

$$e^{(a+bi)x}=e^{ax}(\cos(bx)+i\sin(bx))$$

Integrating both sides, 

$$\dfrac{1}{a+bi}e^{(a+bi)x}+k=\int e^{(a+bi)x}\dd x=\int e^{ax}\cos (bx)\dd x + i\int e^{ax}\sin (bx)\dd x$$

but 

$$
\begin{array}{rcl}
\dfrac{1}{a+bi}e^{(a+bi)x} & = & \dfrac{1}{a+bi}\dfrac{a-bi}{a-bi}e^{ax}(\cos(bx)+i\sin(bx))\\[1em]
& = & \dfrac{1}{a^2+b^2}e^{ax}(a-bi)(\cos(bx)+i\sin(bx))\\[1em]
& = & \dfrac{1}{a^2+b^2}e^{ax}(a\cos(bx)+b\sin(bx)) \\[1em]
& + & i\dfrac{1}{a^2+b^2}e^{ax}(a\sin(bx)-b\cos(bx))
\end{array}
$$

and equating real and imaginary parts returns

$$\int e^{ax}\cos (bx)\dd x=\dfrac{1}{a^2+b^2}e^{ax}(a\cos(bx)+b\sin(bx))+k$$
$$\int e^{ax}\sin (bx)\dd x=\dfrac{1}{a^2+b^2}e^{ax}(a\sin(bx)-b\cos(bx))+k$$

derivation which centainly is most remarkable

+++

---
[{c}]

$$<<< \int \cos(\ln x)\dd x$$

+++
Solution
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

Surprisingly enough, a change of variable $e^t=x$, $e^t\dd t=\d x$ would lead to $\int e^t\cos t\dd t$, which is solved with the very same double integration by parts technique

+++