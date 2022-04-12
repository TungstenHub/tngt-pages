[{a}]

$$<<< \int \sin^3(3x+2)\dd x$$

+++
Solución
+++

$$<<< 
\int \sin^3(3x+2)\dd x \oveq{ t=3x+2\\ \d t=3\dd x }
\dfrac{1}{3}\int \sin^3(t)\dd t
\\ \qquad 
= \dfrac{1}{3}\int (1-\cos^2(t))\sin t\dd t
\oveq{ w=\cos t\\ \d w=-\sin t\dd t }
-\dfrac{1}{3}\int (1-w^2)\dd w
\\ \qquad 
= -\dfrac{1}{3}w+\dfrac{1}{9}w^3+k
\oveq{ w=\cos t }
-\dfrac{1}{3}\cos t+\dfrac{1}{9}\cos^3(t)+k
\\ \qquad 
\oveq{ t=3x+2 }
\hl{-\dfrac{1}{3}\cos(3x+2)+\dfrac{1}{9}\cos^3(3x+2) + k}
$$

+++

---
[{b}]

$$<<< \int \cos^4(x)\dd x$$

+++
Solución
+++

$$<<< 
\int \cos^4(x)\dd x
= \int \left(\dfrac{1+\cos(2x)}{2}\right)^2\dd x
\\ \qquad 
= \dfrac{1}{4}\int (1+2\cos(2x)+\cos^2(2x))\dd x
\\ \qquad 
= \dfrac{1}{4}\int \left(1+2\cos(2x)+\dfrac{1+\cos(4x)}{2}\right)\dd x
\\ \qquad 
= \hl{\dfrac{3}{8}x + \dfrac{1}{4}\sin(2x) + \dfrac{1}{32}\sin(4x) + k}
$$

+++

---
[{c}]

$$<<< \int \sin^2(x)\cos^4(x)\dd x$$

+++
Solución
+++

$$<<< 
\int \sin^2(x)\cos^4(x)\dd x
\\ \qquad 
= \int (1-\cos^2(x))\cos^4(x)\dd x
\\ \qquad 
= \int (\cos^4(x)-\cos^6(x))\dd x
\\ \qquad 
= \int \left(\left(\dfrac{1+\cos(2x)}{2}\right)^2-\left(\dfrac{1+\cos(2x)}{2}\right)^3\right)\dd x
\\ \qquad 
= \int \left(\dfrac{1+2\cos(2x)+\cos^2(2x)}{4}-\dfrac{1+3\cos(2x)+3\cos^2(2x)+\cos^3(2x)}{8}\right)\dd x
\\ \qquad 
= \dfrac{1}{8}\int (1+1\cos(2x)-\cos^2(2x)-\cos^3(2x))\dd x
\\ \qquad 
=\dfrac{1}{8}x+\dfrac{1}{16}\sin(2x)-\dfrac{1}{8}\int\dfrac{1+\cos(4x)}{2}\dd x - \dfrac{1}{8}\int(1-\sin^2(2x))\cos(2x)\dd x
\\ \qquad 
\oveq{ t=\sin(2x)\\ \d t=2\cos(2x)\dd x }
\dfrac{1}{8}x+\dfrac{1}{16}\sin(2x)-\dfrac{1}{16}x-\dfrac{1}{64}\sin(4x) - \dfrac{1}{16}\int(1-t^2)\dd t
\\ \qquad 
= \dfrac{1}{16}x+\dfrac{1}{16}\sin(2x)-\dfrac{1}{64}\sin(4x) -\dfrac{1}{16}t+\dfrac{1}{48}t^3
\\ \qquad 
\oveq{ t=\sin(2x) }
\dfrac{1}{16}x+\dfrac{1}{16}\sin(2x)-\dfrac{1}{64}\sin(4x) -\dfrac{1}{16}\sin(2x)+\dfrac{1}{48}t^3+k
\\ \qquad 
= \hl{\dfrac{1}{16}x -\dfrac{1}{64}\sin(4x) +\dfrac{1}{48}\sin^3(2x) + k}$$

+++