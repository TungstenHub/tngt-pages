[{a}]

$$<<< \int \dfrac{e^x+e^{2x}+e^{3x}+e^{4x}}{e^{4x}}\dd x$$

+++
Solution
+++

$$<<< 
\int \dfrac{e^x+e^{2x}+e^{3x}+e^{4x}}{e^{4x}}\dd x \\
\qquad = \int \left(e^{-3x}+e^{-2x}+e^{-x}+1\right)\dd x \\
\qquad = \dfrac{e^{-3x}}{-3}+\dfrac{e^{-2x}}{-2}+\dfrac{e^{-x}}{-1}+x+k
$$

Indeed, for any integral

$$\int e^{ax}\dd x$$

we may apply a simple change of variable

$$t=ax$$
$$\dd t=a\dd x$$

so

$$\int e^{ax}\dd x=\dfrac{1}{a}\int e^{ax}a\dd x=\dfrac{1}{a}\int e^t\dd t=\dfrac{1}{a}e^t+k=\dfrac{1}{a}e^{ax}+k$$

One could also reason this way:

$$\int e^{ax}\dd x=\int \left(e^a\right)^x\dd x=\dfrac{1}{\ln\left(e^a\right)}\left(e^a\right)^x+k=\dfrac{1}{a}e^{ax}+k$$

In both ways, 

$$\int e^{ax}\dd x=\dfrac{1}{a}e^{ax}+k$$

and also

$$<<< 
\int \dfrac{e^x+e^{2x}+e^{3x}+e^{4x}}{e^{4x}}\dd x \\
\qquad = \hl{-\dfrac{e^{-3x}}{3}-\dfrac{e^{-2x}}{2}-e^{-x}+x+k}
$$

+++

---
[{b}]

$$<<< \int \dfrac{e^{2x}+e^{-2x}}{e^x}\dd x$$

+++
Solution
+++

$$<<< 
\int \dfrac{e^{2x}+e^{-2x}}{e^x}\dd x \\
\qquad = \int \left(e^x+e^{-3x}\right)\dd x \\
\qquad = \hl{e^x-\dfrac{e^{-3x}}{3}+k}
$$

+++

---
[{c}]

$$<<< \int \sin(5x+2)\dd x$$

+++
Solution
+++

$$<<< 
\int \sin(5x+2)\dd x \\
\qquad = \dfrac{1}{5}\int \sin(5x+2)5\dd x \\
\qquad \oveq{t=5x+2\\ \mathrm{d}t=5\dd x}
\dfrac{1}{5}\int \sin t\dd t=
-\dfrac{1}{5}\cos t + k \\
\qquad \oveq{t=5x+2}
\hl{-\dfrac{1}{5}\cos(5x+2) + k}
$$

+++