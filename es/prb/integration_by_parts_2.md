[{a}]

$$<<< \int \tan^{-1} x\dd x$$

+++
Solución
+++

$$<<< 
\int \tan^{-1} x\dd x
\\ \qquad 
\oveq{ u=\tan^{-1} x\quad u'=\frac{1}{1+x^2}\\ v'=1\quad v=x }
x\tan^{-1} x-\int \frac{x}{1+x^2}\dd x
\\ \qquad 
= \hl{x\tan^{-1} x-\dfrac{1}{2}\ln(1+x^2)+k}
$$

+++

---
[{b}]

$$<<< \int \sin^{-1} x\dd x$$

+++
Solución
+++

$$<<< 
\int \sin^{-1} x\dd x
\\ \qquad 
\oveq{ u=\sin^{-1} x\quad u'=\frac{1}{\sqrt{1-x^2}}\\ v'=1\quad v=x }
x\sin^{-1} x-\int \frac{x}{\sqrt{1-x^2}}\dd x
\\ \qquad 
= \hl{x\sin^{-1} x+\sqrt{1-x^2}+k}
$$

+++

---
[{c}]

$$<<< \int \dfrac{\ln\left(\sqrt{x}\right)}{\sqrt{x}}\dd x$$

+++
Solución
+++

$$<<< 
\int \dfrac{\ln\left(\sqrt{x}\right)}{\sqrt{x}}\dd x
\\ \qquad 
\oveq{ u=\ln\left(\sqrt{x}\right)\quad u'=\frac{1}{\sqrt{x}}\frac{1}{2\sqrt{x}}\\ v'=\frac{1}{\sqrt{x}}\quad v=2\sqrt{x} }
2\sqrt{x}\ln\left(\sqrt{x}\right) - \int\frac{1}{2x}2\sqrt{x}\dd x
\\ \qquad 
= \hl{\sqrt{x}\ln x - 2\sqrt{x} + k}
$$

Ten en cuenta que $\ln\left(\sqrt{x}\right)=\dfrac{1}{2}\ln x$. Un cambio de variable $t=\sqrt{x}$ también habría funcionado

+++

---
[{d}]

$$<<< \int x^3 e^{x^2}\dd x$$

+++
Solución
+++

$$<<< 
\int x^3 e^{x^2}\dd x
\\ \qquad 
\oveq{ t=x^2\\ \d t=2x\dd x }
\dfrac{1}{2}\int t e^t\dd t
\\ \qquad 
\oveq{ u=t\quad u'=1\\ v'=e^t\quad v=e^t }
\dfrac{1}{2}\left(t e^t-\int e^t\dd t\right)
\\ \qquad 
= \dfrac{1}{2}(t-1)e^t + k
\oveq{ t=x^2 }
\hl{\dfrac{1}{2}(x^2-1)e^{x^2} + k}
$$

+++

---
[{e}]

$$<<< \int x\tan^{-1} x\dd x$$

+++
Solución
+++

$$<<< 
\int x\tan^{-1} x\dd x
\\ \qquad 
\oveq{ u=\tan^{-1} x\quad u'=\frac{1}{1+x^2}\\ v'=x\quad v=\frac{1}{2}x^2 }
\dfrac{1}{2}x^2\tan^{-1} x - \int \dfrac{1}{2}x^2\frac{1}{1+x^2}\dd x
\\ \qquad 
= \dfrac{1}{2}x^2\tan^{-1} x - \dfrac{1}{2}\int \left(1-\frac{1}{1+x^2}\right)\dd x
\\ \qquad 
= \dfrac{1}{2}x^2\tan^{-1} x  - \dfrac{1}{2}(x -\tan^{-1} x) + k
\\ \qquad 
= \hl{\dfrac{1}{2}\left((x^2+1)\tan^{-1} x - x\right) + k}
$$

+++