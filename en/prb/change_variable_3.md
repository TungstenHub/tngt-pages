[{a}]

$$<<< \int \dfrac{x+2}{x^2+4x-13}\dd x$$

+++
Solution
+++

$$<<< 
\int \dfrac{x+2}{x^2+4x-13}\dd x
\\ \qquad 
= \dfrac{1}{2}\int \dfrac{2x+4}{x^2+4x-13}\dd x
\oveq{ t=x^2+4x-13\\ \d t=(2x+4)\dd x }
\dfrac{1}{2}\int \dfrac{1}{t}\dd t
\\ \qquad 
= \dfrac{1}{2}\ln|t| + k
\oveq{ t=x^2+4x-13 }
\hl{\dfrac{1}{2}\ln|x^2+4x-13| + k}
$$

+++

---
[{b}]

$$<<< \int e^x\sin(e^x)\dd x$$

+++
Solution
+++

$$<<< 
\int e^x\sin(e^x)\dd x
\\ \qquad 
\oveq{ t=e^x\\ \d t=e^x\dd x }
\int \sin t\dd t
\\ \qquad 
= -\cos t + k
\oveq{ t=e^x }
\hl{-\cos(e^x) + k}
$$

+++

---
[{c}]

$$<<< \int \dfrac{\ln(\sqrt{x})}{x}\dd x$$

+++
Solution
+++

$$<<< 
\int \dfrac{\ln(\sqrt{x})}{x}\dd x
\\ \qquad 
= \dfrac{1}{2}\int \dfrac{\ln x}{x}\dd x
\oveq{ t=\ln x\\ \d t=\frac{1}{x}\dd x }
\dfrac{1}{2}\int t\dd t
\\ \qquad 
= \dfrac{1}{4}t^2 + k
\oveq{ t=\ln x }
\hl{\dfrac{1}{4}(\ln x)^2 + k}
$$

+++

---
[{d}]

$$<<< \int \ln(\cos x)\tan x\dd x$$

+++
Solution
+++

$$<<< 
\int \ln(\cos x)\tan x\dd x
\\ \qquad 
= \int \ln(\cos x)\dfrac{\sin x}{\cos x}\dd x
\oveq{ t=\cos x\\ \d t=-\sin x\dd x }
-\int \dfrac{\ln t}{t}\dd t
\\ \qquad 
\oveq{ w=\ln t\\ \d w=\frac{1}{t}\dd t }
-\int w\dd w
= -\dfrac{1}{2}w^2+k
\\ \qquad 
\oveq{ w=\ln t }
-\dfrac{1}{2}(\ln t)^2+k
\oveq{ t=\cos x }
\hl{-\dfrac{1}{2}(\ln(\cos x))^2+k}
$$

+++

---
[{e}]

$$<<< \int x\sqrt{1-3x^2}\dd x$$

+++
Solution
+++

$$<<< 
\int x\sqrt{1-3x^2}\dd x
\\ \qquad 
= -\dfrac{1}{6}\int \sqrt{1-3x^2}(-6x)\dd x
\oveq{ t=1-3x^2\\ \d t=-6x\dd x }
-\dfrac{1}{6}\int t^{\frac{1}{2}}\dd t
\\ \qquad 
= -\dfrac{1}{6}\dfrac{2}{3}t^{\frac{3}{2}} + k
\oveq{ t=1-3x^2 }
\hl{-\dfrac{1}{9}(1-3x^2)^{\frac{3}{2}} + k}
$$

+++