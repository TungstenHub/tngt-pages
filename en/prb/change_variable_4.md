[{a}]

$$<<< \int \dfrac{x^2}{8+x^6}\dd x$$

+++
Solution
+++

$$<<< 
\int \dfrac{x^2}{8+x^6}\dd x
\\ \qquad 
= \dfrac{1}{3}\int \dfrac{3x^2}{8+x^6}\dd x
\oveq{ t=x^3\\ \d t=3x^2\dd x }
\dfrac{1}{3}\int \dfrac{1}{8+t^2}\dd t
\\ \qquad 
= \dfrac{1}{3\sqrt{8}}\tan^{-1}\left(\dfrac{t}{\sqrt{8}}\right) + k
\oveq{ t=x^3 }
\hl{\dfrac{1}{3\sqrt{8}}\tan^{-1}\left(\dfrac{x^3}{\sqrt{8}}\right)  + k}
$$

+++

---
[{b}]

$$<<< \int \dfrac{e^x}{e^{2x}+2e^x+1}\dd x$$

+++
Solution
+++

$$<<< 
\int \dfrac{e^x}{e^{2x}+2e^x+1}\dd x
\\ \qquad 
= \int \dfrac{e^x}{(e^x+1)^2}\dd x
\oveq{ t=e^x+1\\ \d t=e^x\dd x }
\int \dfrac{1}{t^2}\dd t
\\ \qquad 
= -\dfrac{1}{t} + k
\oveq{ t=e^x+1 }
\hl{-\dfrac{1}{e^x+1} + k}
$$

+++

---
[{c}]

$$<<< \int \dfrac{x+4}{\sqrt{1-x^2}}\dd x$$

+++
Solution
+++

$$<<< 
\int \dfrac{x+4}{\sqrt{1-x^2}}\dd x
\\ \qquad 
= \int \dfrac{x}{\sqrt{1-x^2}}\dd x + 4\int \dfrac{1}{\sqrt{1-x^2}}\dd x
\\ \qquad 
= -\dfrac{1}{2}\int \dfrac{-2x}{\sqrt{1-x^2}}\dd x + 4\sin^{-1}x+k
\\ \qquad 
\oveq{ t=1-x^2\\ \d t=-2x\dd x }
-\dfrac{1}{2}\int \dfrac{1}{\sqrt{t}}\dd t + 4\sin^{-1}x+k
\\ \qquad 
= -\sqrt{t} + 4\sin^{-1}x + k
\oveq{ t=1-x^2 }
\hl{-\sqrt{1-x^2} + 4\sin^{-1}x  + k}
$$

+++

---
[{d}]

$$<<< \int \dfrac{1}{x\ln x}\dd x$$

+++
Solution
+++

$$<<< 
\int \dfrac{1}{x\ln x}\dd x
\oveq{ t=\ln x\\ \d t=\frac{1}{x}\dd x }
\int \dfrac{1}{t}\dd t
= \ln |t|+k
\oveq{ t=\ln x }
\hl{\ln|\ln x|+k}
$$

+++

---
[{e}]

$$<<< \int \dfrac{x}{\sqrt{1-x^4}}\dd x$$

+++
Solution
+++

$$<<< 
\int \dfrac{x}{\sqrt{1-x^4}}\dd x
\\ \qquad 
= \dfrac{1}{2}\int \dfrac{2x}{\sqrt{1-x^4}}\dd x
\oveq{ t=x^2\\ \d t=2x\dd x }
\dfrac{1}{2}\int \dfrac{1}{\sqrt{1-t^2}}\dd t
\\ \qquad 
= \dfrac{1}{2}\sin^{-1} t + k
\oveq{ t=x^2 }
\hl{\dfrac{1}{2}\sin^{-1} (x^2) + k}
$$

+++