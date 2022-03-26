[{a}]

$$<<< \int \sin x\cos(3x)\dd x$$

+++
Solution
+++

First we expand $\cos(3x)$:

$$
\cos(3x)=\cos(2x)\cos x-\sin(2x)\sin x \\
= (\cos^2(x)-\sin^2(x))\cos x-2\sin x\cos x\sin x \\
= \cos^3(x)-3\sin^2(x)\cos x=\cos^3(x)-3(1-\cos^2(x))\cos x \\
= 4\cos^3(x)-3\cos x
$$

Now we're ready to plug it in

$$<<< 
\int \sin x\cos(3x)\dd x
\\ \qquad
= \int \sin x(4\cos^3(x)-3\cos x)\dd x
\oveq{ t=\cos x\\ \d t=-\sin x\dd x }
\int (3t-4t^3)\dd t
\\ \qquad
= \dfrac{3}{2}t^2 - t^4 + k
\oveq{ t=\cos x }
\hl{\dfrac{3}{2}\cos^2(x) - \cos^4(x) +k}
$$

Alternatively,

$$\sin \alpha\cos\beta = \dfrac{1}{2}(\sin(\alpha-\beta)+\sin(\alpha+\beta))$$
$$\sin x\cos(3x) = \dfrac{1}{2}(\sin(-2x)+\sin(4x))=\dfrac{1}{2}(-\sin(2x)+\sin(4x))$$

and therefore

$$<<< 
\int \sin x\cos(3x)\dd x
\\ \qquad
= \dfrac{1}{2}\int (-\sin(2x)+\sin(4x))\dd x
\\ \qquad
= \hl{\dfrac{1}{4}\cos(2x) - \dfrac{1}{8}\cos(4x) +k}
$$

Both results are indeed the same up to a constant, because (check it!)

$$
\dfrac{1}{4}\cos(2x) - \dfrac{1}{8}\cos(4x) - \left(\dfrac{3}{2}\cos^2(x) - \cos^4(x)\right)=-\dfrac{3}{8}
$$

+++

---
[{b}]

$$<<< \int \sin^2(x)\cos^3(x)\dd x$$

+++
Solution
+++

$$<<< 
\int \sin^2(x)\cos^3(x)\dd x
\\ \qquad
= \int \sin^2(x)(1-\sin^2(x))\cos x\dd x
\oveq{ t=\sin x\\ \d t=\cos x\dd x }
\int t^2(1-t^2)\dd t
\\ \qquad
= \dfrac{1}{3}t^3 - \dfrac{1}{5}t^5 + k
\oveq{ t=\sin x }
\hl{\dfrac{1}{3}\sin^3(x) - \dfrac{1}{5}\sin^5(x) + k}
$$

+++

---
[{c}]

$$<<< \int \cos(2x)\cos(4x)\dd x$$

+++
Solution
+++

$$<<< 
\int \cos(2x)\cos(4x)\dd x
\\ \qquad
= \int \cos(2x)(\cos^2(2x)-\sin^2(2x))\dd x
\\ \qquad
=\int \cos(2x)(1-2\sin^2(2x))\dd x
\\ \qquad
\oveq{ t=\sin(2x)\\ \d t=2\cos(2x)\dd x }
\dfrac{1}{2}\int (1-2t^2)\dd t
=\dfrac{1}{2}t - \dfrac{1}{3}t^3 + k
\\ \qquad
\oveq{ t=\sin(2x) }
\hl{\dfrac{1}{2}\sin(2x) - \dfrac{1}{3}\sin^3(2x) + k}
$$

+++