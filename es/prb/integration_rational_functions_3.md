[{a}]

$$<<< \int \dfrac{x^3}{x^2+2x+3}\dd x$$

+++
Solution
+++

First we perform polynomial division until the degree of the numerator is less than the degree of the denominator

$$
\begin{array}{rcl}
x^3 & = & x^3+2x^2+3x-2x^2-3x\\
& = & x(x^2+2x+3)-2x^2-3x\\
& = & x(x^2+2x+3)-2x^2-4x-6+x+6\\
& = & x(x^2+2x+3)-2(x^2+2x+3)+x+6\\
& = & (x-2)(x^2+2x+3)+x+6
\end{array}$$

$$\dfrac{x^3}{x^2+2x+3}=x-2+\dfrac{x+6}{x^2+2x+3}$$

Now we focus on partial fractions decomposition. $x^2+2x+3$ has no real roots

$$x^2+2x+3=0\Longrightarrow x=\dfrac{-2\pm\sqrt{2^2-4\cdot 1\cdot 3}}{2}=\dfrac{-2\pm\sqrt{-8}}{2}$$

Indeed,

$$(x+1)^2=x^2+2x+1$$
$$x^2+2x+3=(x+1)^2+2$$
$$x+6=(x+1)+5$$
$$\dfrac{x+6}{x^2+2x+3}=\dfrac{x+1}{(x+1)^2+2}+\dfrac{5}{(x+1)^2+2}$$

Therefore

$$<<< 
\int \dfrac{4x+1}{x^2+x+3}\dd x
\\ \qquad
= \int \left(x-2+\dfrac{x+1}{(x+1)^2+2}+\dfrac{5}{(x+1)^2+2}\right)\dd x
\\ \qquad
= \dfrac{1}{2}x^2-2x+\dfrac{1}{2}\ln|(x+1)^2+2|-\dfrac{5}{\sqrt{2}}\tan^{-1}\left(\dfrac{x+1}{\sqrt{2}}\right) + k
\\ \qquad
= \hl{\dfrac{1}{2}x^2-2x+\dfrac{1}{2}\ln|x^2+2x+3|-\dfrac{5}{\sqrt{2}}\tan^{-1}\left(\dfrac{x+1}{\sqrt{2}}\right) + k}
$$

+++

---
[{b}]

$$<<< \int \dfrac{x^5}{(x+1)^3}\dd x$$

+++
Solution
+++

The partial fraction decomposition will be more easily handled with a change of variable $y=x+1$

$$\dfrac{x^5}{(x+1)^3}=\dfrac{(y-1)^5}{y^3}=\dfrac{y^5-5y^4+10y^3-10y^2+5y-1}{y^3} \\ 
= y^2-5y+10-\dfrac{10}{y}+\dfrac{5}{y^2}-\dfrac{1}{y^3} \\
= (x+1)^2-5(x+1)+10-\dfrac{10}{x+1}+\dfrac{5}{(x+1)^2}-\dfrac{1}{(x+1)^3}$$

Therefore

$$<<< 
\int \dfrac{x^5}{(x+1)^3}\dd x
\\ \qquad
= \int \left((x+1)^2-5(x+1)+10-\dfrac{10}{x+1}+\dfrac{5}{(x+1)^2}-\dfrac{1}{(x+1)^3}\right)\dd x
\\ \qquad
= \hl{\dfrac{1}{3}(x+1)^3 - \dfrac{5}{2}(x+1)^2+10x -10\ln|x+1| - \dfrac{5}{x+1} + \dfrac{1}{2(x+1)^2} + k}
$$

Of course a change of variable $t=x+1$ inside the integral would have had analogous results

+++

---
[{c}]

$$<<< \int \dfrac{\d x}{1+e^x}$$

+++
Solution
+++

$$<<< 
\int \dfrac{\d x}{1+e^x}
\\ \qquad
= \int \dfrac{e^x}{e^x(1+e^x)}\dd x
\oveq{ t=e^x\\ \d t=e^x\dd x }
\int \dfrac{1}{t(1+t)}\dd t
\\ \qquad
= \int \left(\dfrac{1}{t}-\dfrac{1}{t+1}\right)\dd t
= \ln|t|-\ln|t+1| + k 
\\ \qquad
\oveq{ t=e^x }
\hl{x - \ln(1+e^x) + k}
$$

+++

---
[{d}]

$$<<< \int \dfrac{5}{x^2-3}\dd x$$

+++
Solution
+++

Let's decompose in partial fractions:

$$x^2-3=(x-\sqrt{3})(x+\sqrt{3})$$
$$
\dfrac{1}{x-\sqrt{3}}-\dfrac{1}{x+\sqrt{3}}
= \dfrac{x+\sqrt{3}}{(x-\sqrt{3})(x+\sqrt{3})}-\dfrac{x-\sqrt{3}}{(x-\sqrt{3})(x+\sqrt{3})} \\
= \dfrac{2\sqrt{3}}{(x-\sqrt{3})(x+\sqrt{3})}
$$
$$\dfrac{5}{x^2-3}=\dfrac{5}{2\sqrt{3}}\left(\dfrac{1}{x-\sqrt{3}}-\dfrac{1}{x+\sqrt{3}}\right)$$


Therefore

$$<<< 
\int \dfrac{5}{x^2-3}\dd x
\\ \qquad
= \int \dfrac{5}{2\sqrt{3}}\left(\dfrac{1}{x-\sqrt{3}}-\dfrac{1}{x+\sqrt{3}}\right)\dd x
\\ \qquad
= \hl{\dfrac{5}{2\sqrt{3}}\left(\ln\left|x-\sqrt{3}\right|-\ln\left|x+\sqrt{3}\right|\right) + k}
$$

+++

---
[{e}]

$$<<< \int \sqrt{1+e^x}\dd x$$

+++
Solution
+++

$$<<< 
\int \sqrt{1+e^x}\dd x
= \int \dfrac{e^x\sqrt{1+e^x}}{e^x}\dd x
\oveq{ t=e^x\\ \d t=e^x\dd x }
\int \dfrac{\sqrt{t+1}}{t}\dd t
\\ \qquad
\oveq{ w=\sqrt{t+1}\\ w^2=t+1 \\ 2w\dd w=\d t }
\int \dfrac{2w^2}{w^2-1}\dd w
= \int \left(2+\dfrac{2}{w^2-1}\right)\dd w
\\ \qquad
= \int \left(2+\dfrac{1}{w-1}-\dfrac{1}{w-1}\right)\dd w
= 2w+\ln|w-1|-\ln|w+1| + k 
\\ \qquad
\oveq{ w=\sqrt{t+1} }
2\sqrt{t+1}+\ln(\sqrt{t+1}-1)-\ln(\sqrt{t+1}+1) + k 
\\ \qquad
\oveq{ t=e^x }
\hl{2\sqrt{1+e^x}+\ln(\sqrt{1+e^x}-1)-\ln(\sqrt{1+e^x}+1) + k }$$

+++