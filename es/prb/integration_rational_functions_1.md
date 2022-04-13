[{a}]

$$<<< \int \dfrac{5x-1}{x^2-6x+9}\dd x$$

+++
Solución
+++

$$<<< 
\int \dfrac{5x-1}{x^2-6x+9}\dd x
\\ \qquad
= \int \dfrac{5x-15+14}{(x-3)^2}\dd x
\\ \qquad
= \int \left(\dfrac{5}{x-3}+\dfrac{14}{(x-3)^2}\right)\dd x
\\ \qquad
= \hl{5\ln|x-3| -\dfrac{14}{x-3} + k}
$$

+++

---
[{b}]

$$<<< \int \dfrac{2x^2+x+1}{(x+3)(x-1)^2}\dd x$$

+++
Solución
+++

Descompongamos en fracciones simples:

$$\dfrac{2x^2+x+1}{(x+3)(x-1)^2}=\dfrac{A}{x+3}+\dfrac{B}{x-1}+\dfrac{C}{(x-1)^2}$$
$$2x^2+x+1 = A(x-1)^2+B(x+3)(x-1)+C(x+3)$$
$$x=-3\leadsto 16=2\cdot(-3)^2+(-3)+1 \\
= A(-3-1)^2+B(-3+3)(-3-1)+C(-3+3)=16A\Longrightarrow A=1$$
$$x=1\leadsto 4=2\cdot 1^2+1+1 \\
= A(1-1)^2+B(1+3)(1-1)+C(1+3)=4C\Longrightarrow C=1$$

Para hallar $B$, podemos despejarla, puesto que ya sabemos $A$ y $C$, pero va a ser más fácil derivar la expresión anterior una vez:

$$(2x^2+x+1)' = (A(x-1)^2+B(x+3)(x-1)+C(x+3))'$$
$$4x+1 = 2A(x-1)+B(x-1)+B(x+3)+C$$
$$x=1\leadsto 5=4\cdot 1+1 \\
= 2A(1-1)+B(1-1)+B(1+3)+C=4B+1\Longrightarrow B=1$$

Por tanto

$$<<< 
\int \dfrac{2x^2+x+1}{(x+3)(x-1)^2}\dd x
\\ \qquad
= \int \left(\dfrac{1}{x+3}+\dfrac{1}{x-1}+\dfrac{1}{(x-1)^2}\right)\dd x
\\ \qquad
= \hl{\ln|x+3|+\ln|x-1|-\dfrac{1}{x-1} + k}
$$

+++

---
[{c}]

$$<<< \int \dfrac{\d x}{x^3-x}$$

+++
Solución
+++

Descompongamos en fracciones simples:

$$\dfrac{1}{x^3-x}=\dfrac{A}{x}+\dfrac{B}{x-1}+\dfrac{C}{x+1}$$
$$1 = A(x-1)(x+1)+Bx(x+1)+Cx(x-1)$$
$$x=0\leadsto 1=A(0-1)(0+1)+B\cdot 0\cdot (0+1)+C\cdot 0\cdot (0-1) \\
= -A\Longrightarrow A=-1$$
$$x=1\leadsto 1=A(1-1)(1+1)+B\cdot 1\cdot (1+1)+C\cdot 1\cdot (1-1) \\
= 2B\Longrightarrow B=\dfrac{1}{2}$$
$$x=-1\leadsto 1=A(-1-1)(-1+1)+B\cdot (-1)\cdot (-1+1)+C\cdot (-1)\cdot (-1-1) \\
= 2C\Longrightarrow C=\dfrac{1}{2}$$

Por tanto

$$<<< 
\int \dfrac{\d x}{x^3-x}
\\ \qquad
= \int \left(\dfrac{-1}{x}+\dfrac{1}{2(x-1)}+\dfrac{1}{2(x+1)}\right)\dd x
\\ \qquad
= \hl{-\ln|x|+\dfrac{1}{2}\ln|x-1|+\dfrac{1}{2}\ln|x+1| + k}
$$

+++

---
[{d}]

$$<<< \int \dfrac{x}{(x+2)^4}\dd x$$

+++
Solución
+++

$$<<< 
\int \dfrac{x}{(x+2)^4}\dd x
\\ \qquad
= \int \dfrac{x+2-2}{(x+2)^4}\dd x
\\ \qquad
= \int \left(\dfrac{1}{(x+2)^3}-\dfrac{2}{(x+2)^4}\right)\dd x
\\ \qquad
= \hl{-\dfrac{1}{2(x+2)^2}+\dfrac{2}{3(x+2)^3} +k}
$$

+++

---
[{e}]

$$<<< \int \dfrac{3x^2+2}{(x+1)^3}\dd x$$

+++
Solución
+++

La descomposición en fracciones simples se va a manejar mejor con un cambio de variable $y=x+1$

$$
\dfrac{3x^2+2}{(x+1)^3}=\dfrac{3(y-1)^2+2}{y^3}=\dfrac{3y^2-6y+5}{y^3} \\
= \dfrac{3}{y}-\dfrac{6}{y^2}+\dfrac{5}{y^3}=\dfrac{3}{x+1}-\dfrac{6}{(x+1)^2}+\dfrac{5}{(x+1)^3}
$$

Por tanto

$$<<< 
\int \dfrac{3x^2+2}{(x+1)^3}\dd x
\\ \qquad
= \int \left(\dfrac{3}{x+1}-\dfrac{6}{(x+1)^2}+\dfrac{5}{(x+1)^3}\right)\dd x
\\ \qquad
= \hl{3\ln|x+1| + \dfrac{6}{x+1} - \dfrac{5}{2(x+1)^2} + k}
$$

Por supuesto un cambio de variable $t=x+1$ dentro de la integral hubiera tenido resultados análogos

+++