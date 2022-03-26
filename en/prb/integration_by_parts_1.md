[{a}]

$$<<< \int x^2 e^x\dd x$$

+++
Solution
+++

$$<<< 
\int x^2 e^x\dd x
\\ \qquad 
\oveq{ u=x^2\quad u'=2x\\ v'=e^x\quad v=e^x }
x^2 e^x-\int 2x e^x\dd x
\\ \qquad 
\oveq{ u=2x\quad u'=2\\ v'=e^x\quad v=e^x }
x^2 e^x-2xe^x+\int 2e^x\dd x
\\ \qquad 
= \hl{(x^2- 2x+2)e^x+k}
$$

+++

---
[{b}]

$$<<< \int (3x+2)\sin x\dd x$$

+++
Solution
+++

$$<<< 
\int (3x+2)\sin x\dd x
\\ \qquad 
\oveq{ u=3x+2\quad u'=3\\ v'=\sin x\quad v=-\cos x }
(3x+2)(-\cos x)-\int 3 (-\cos x)\dd x
\\ \qquad 
= \hl{-(3x+2)\cos x + 3\sin x + k}
$$

+++

---
[{c}]

$$<<< \int x^2\ln x\dd x$$

+++
Solution
+++

$$<<< 
\int x^2\ln x\dd x
\\ \qquad 
\oveq{ u=\ln x\quad u'=\frac{1}{x}\\ v'=x^2\quad v=\frac{1}{3}x^3 }
\dfrac{1}{3}x^3\ln x - \int\frac{1}{3}x^3\frac{1}{x}\dd x
\\ \qquad 
= \dfrac{1}{3}x^3\ln x -\dfrac{1}{9}x^3  + k
\\ \qquad 
= \hl{\dfrac{1}{9}x^3(3\ln x - 1) + k}
$$

+++

---
[{d}]

$$<<< \int \ln^3 x\dd x$$

+++
Solution
+++

$$<<< 
\int \ln^3 x\dd x
\\ \qquad 
\oveq{ u=\ln^3 x\quad u'=3\ln^2 x\frac{1}{x}\\ v'=1\quad v=x }
x\ln^3 x - \int 3\ln^2 x\frac{1}{x}x\dd x
\\ \qquad 
\oveq{ u=3\ln^2 x\quad u'=6\ln x\frac{1}{x}\\ v'=1\quad v=x }
x\ln^3 x - 3x\ln^2 x + \int 6\ln x\frac{1}{x}x\dd x
\\ \qquad 
\oveq{ u=6\ln x\quad u'=\frac{6}{x}\\ v'=1\quad v=x }
x\ln^3 x - 3x\ln^2 x + 6x\ln x -\int 6\frac{1}{x}x\dd x
\\ \qquad 
= \hl{x(\ln^3 x - 3\ln^2 x + 6\ln x -6) + k}
$$

+++

---
[{e}]

$$<<< \int x\cdot 3^{-x}\dd x$$

+++
Solution
+++

$$<<< 
\int x\cdot 3^{-x}\dd x
\\ \qquad 
\oveq{ u=x\quad u'=1\\ v'=3^{-x}\quad v=-\frac{1}{\ln 3}3^{-x} }
-\frac{1}{\ln 3}x\cdot 3^{-x} - \int -\frac{1}{\ln 3}3^{-x}\dd x
\\ \qquad 
= \hl{\left(-\frac{1}{\ln 3}x-\frac{1}{\ln^2 3}\right)3^{-x} + k}
$$

+++