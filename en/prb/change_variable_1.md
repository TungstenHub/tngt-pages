[{a}]

$$<<< \int x^2\cos(4x^3-2)\dd x$$

+++
Solution
+++

$$<<< 
\int x^2\cos(4x^3-2)\dd x 
\\ \qquad 
= \dfrac{1}{12}\int \cos(4x^3-2)12x^2\dd x
\oveq{t=4x^3-2\\ \d t=12x^2\dd x}
\dfrac{1}{12}\int \cos t\dd t 
\\ \qquad 
= \dfrac{1}{12}\sin t + k
\oveq{t=4x^3-2}
\hl{\dfrac{1}{12}\sin(4x^3-2) + k}
$$

+++

---
[{b}]

$$<<< \int \dfrac{\d x}{a^2+x^2}$$

+++
Solution
+++

$$<<< 
\int \dfrac{\d x}{a^2+x^2}
\\ \qquad 
= \dfrac{1}{a^2}\int \dfrac{\d x}{1+\left(\frac{x}{a}\right)^2}
\oveq{t=\frac{x}{a}\\ \d t=\frac{1}{a}\dd x}
\dfrac{1}{a}\int \dfrac{\d t}{1+t^2}
\\ \qquad 
= \dfrac{1}{a}\tan^{-1} t + k
\oveq{t=\frac{x}{a}}
\hl{\dfrac{1}{a}\tan^{-1} \left(\dfrac{x}{a}\right) + k}
$$

+++

---
[{c}]

$$<<< \int x(2x^2-2)^{11}\dd x$$

+++
Solution
+++

$$<<< 
\int x(2x^2-2)^{11}\dd x
\\ \qquad 
= \dfrac{1}{4}\int (2x^2-2)^{11}4x\dd x
\oveq{t=2x^2-2\\ \d t=4x\dd x}
\dfrac{1}{4}\int t^{11}\dd t
\\ \qquad 
= \dfrac{1}{4}\dfrac{1}{12}t^{12} + k
\oveq{t=2x^2-2}
\hl{\dfrac{1}{48}(2x^2-2)^{12} + k}
$$

+++

---
[{d}]

$$<<< \int x\sqrt[3]{4+2x^2}\dd x$$

+++
Solution
+++

$$<<< 
\int x\sqrt[3]{4+2x^2}\dd x
\\ \qquad 
= \dfrac{1}{4}\int \sqrt[3]{4+2x^2}4x\dd x
\oveq{t=4+2x^2\\ \d t=4x\dd x}
\dfrac{1}{4}\int t^{\frac{1}{3}}\dd t
\\ \qquad 
= \dfrac{1}{4}\dfrac{3}{4}t^{\frac{4}{3}} + k
\oveq{t=4+2x^2}
\hl{\dfrac{3}{16}(4+2x^2)^{\frac{4}{3}} + k}
$$

+++

---
[{e}]

$$<<< \int \sin^2 x\cos x\dd x$$

+++
Solution
+++

$$<<< 
\int \sin^2 x\cos x\dd x
\\ \qquad 
\oveq{t=\sin x\\ \d t=\cos x\dd x}
\int t^2\dd t
\\ \qquad 
= \dfrac{1}{3}t^3 + k
\oveq{t=\sin x}
\hl{\dfrac{1}{3}\sin^3 x + k}$$

+++