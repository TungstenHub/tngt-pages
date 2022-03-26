[{a}]

$$<<< \int \dfrac{\d x}{\sqrt{x-1}+\sqrt{x+1}}$$

+++
Solution
+++

$$<<< 
\int \dfrac{\d x}{\sqrt{x-1}+\sqrt{x+1}}
\\ \qquad
= \int \dfrac{1}{\sqrt{x-1}+\sqrt{x+1}}\dfrac{\sqrt{x+1}-\sqrt{x-1}}{\sqrt{x+1}-\sqrt{x-1}}\dd x
\\ \qquad
= \int \dfrac{\sqrt{x+1}-\sqrt{x-1}}{\left(\sqrt{x+1}\right)^2-\left(\sqrt{x-1}\right)^2}\dd x
\\ \qquad
= \dfrac{1}{2}\int(\sqrt{x+1}-\sqrt{x-1})\dd x
\\ \qquad
=\dfrac{1}{2}\dfrac{2}{3}\left((x+1)^{\frac{3}{2}}-(x-1)^{\frac{3}{2}}\right)+k
\\ \qquad
= \hl{\dfrac{1}{3}\left((x+1)^{\frac{3}{2}}-(x-1)^{\frac{3}{2}}\right)+k}
$$

+++

---
[{b}]

$$<<< \int \dfrac{2^x}{\sqrt{1-4^x}}\dd x$$

+++
Solution
+++

$$<<< 
\int \dfrac{2^x}{\sqrt{1-4^x}}\dd x
\\ \qquad
= \dfrac{1}{\ln 2}\int \dfrac{2^x\ln 2}{\sqrt{1-\left(2^x\right)^2}}\dd x
\oveq{ t=2^x\\ \d t=2^x\ln 2\dd x }
\dfrac{1}{\ln 2}\int \dfrac{1}{\sqrt{1-t^2}}\dd t
\\ \qquad
= \dfrac{1}{\ln 2}\sin^{-1}t + k
\oveq{ t=2^x }
\hl{\dfrac{1}{\ln 2}\sin^{-1}(2^x) + k}
$$

+++

---
[{c}]

$$<<< \int \dfrac{\d x}{\sqrt{2x-x^2}}$$

+++
Solution
+++

$$<<< 
\int \dfrac{\d x}{\sqrt{2x-x^2}}=
\int \dfrac{\d x}{\sqrt{1-(x-1)^2}}=
\hl{\sin^{-1}(x-1)  + k}
$$

+++

---
[{d}]

$$<<< \int \tan^3 x\dd x$$

+++
Solution
+++

Keeping in mind that $\int \tan x\dd x=-\ln|\cos x|+k$, which was [calculated in a previous problem]( prb | change_variable_2 # a ), we do a trick

$$<<< 
\int \tan^3 x\dd x
\\ \qquad 
= \int \tan x(1+ \tan^2 x)\dd x-\int \tan x\dd x
\\ \qquad 
\oveq{ t=\tan x\\ \d t=(1+ \tan^2 x)\dd x }
\int t\dd t-(-\ln|\cos x|)+k
\\ \qquad 
=\dfrac{1}{2}t^2+\ln|\cos x|+k
\oveq{ t=\tan x }
\hl{\dfrac{1}{2}(\tan x)^2+\ln|\cos x|+k}
$$

+++

---
[{e}]

$$<<< \int \dfrac{x^3+3x}{x^4+1}\dd x$$

+++
Solution
+++

$$<<< 
\int \dfrac{x^3+3x}{x^4+1}\dd x
\\ \qquad 
= \dfrac{1}{4}\int \dfrac{4x^3}{x^4+1}\dd x+\dfrac{3}{2}\int \dfrac{2x}{x^4+1}\dd x
\\ \qquad 
\oveq{ t=x^4\\ \d t=4x^3\dd x\\w=x^2\\ \d w=2x\dd x }
\dfrac{1}{4}\int \dfrac{1}{t+1}\dd t+\dfrac{3}{2}\int \dfrac{1}{1+w^2}\dd x
\\ \qquad 
= \dfrac{1}{4}\ln|t+1| + \dfrac{3}{2}\tan^{-1}w + k
\\ \qquad 
\oveq{ t=x^4\\w=x^2 }
\hl{\dfrac{1}{4}\ln|x^4+1| + \dfrac{3}{2}\tan^{-1}(x^2) + k}
$$

+++