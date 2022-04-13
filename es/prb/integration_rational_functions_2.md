[{a}]

$$<<< \int \dfrac{\d x}{x^4-1}$$

+++
Solución
+++

Descompongamos en fracciones simples:

$$\dfrac{1}{x^4-1}=\dfrac{A}{x+1}+\dfrac{B}{x-1}+\dfrac{C+Dx}{x^2+1}$$
$$1 = A(x-1)(x^2+1)+B(x+1)(x^2+1)+(C+Dx)(x-1)(x+1)$$
$$x=-1\leadsto 1=A(-1-1)((-1)^2+1)+B(-1+1)((-1)^2+1)\\
+ (C+D\cdot(-1))(-1-1)(-1+1) \\
= -4A\Longrightarrow A=-\dfrac{1}{4}$$
$$x=1\leadsto 1=A(1-1)(1^2+1)+B(1+1)(1^2+1)+(C+D\cdot 1)(1-1)(1+1) \\
= 4B\Longrightarrow B=\dfrac{1}{4}$$
$$x=0\leadsto 1=A(0-1)(0^2+1)+B(0+1)(0^2+1)+(C+D\cdot 0)(0-1)(0+1) \\
= -A+B-C=\dfrac{1}{2}-C\Longrightarrow C=-\dfrac{1}{2}$$
$$x=2\leadsto 1=A(2-1)(2^2+1)+B(2+1)(2^2+1)+(C+D\cdot 2)(2-1)(2+1) \\
= 5A+15B+3C+6D=1+6D\Longrightarrow D=0$$

Sin embargo, puede ser útil tener en cuenta que

$$\dfrac{1}{a-1}-\dfrac{1}{a+1}=\dfrac{a+1}{a^2-1}-\dfrac{a-1}{a^2-1}=\dfrac{2}{a^2-1}$$
$$\dfrac{1}{a^2-1}=\dfrac{1}{2}\left(\dfrac{1}{a-1}-\dfrac{1}{a+1}\right)$$

que hubiera hecho nuestra descomposición mucho más fácil

$$\dfrac{1}{x^4-1}=\dfrac{1}{2(x^2-1)}-\dfrac{1}{2(x^2+1)}=\dfrac{1}{4(x-1)}-\dfrac{1}{4(x+1)}-\dfrac{1}{2(x^2+1)}$$

Por tanto

$$<<< 
\int \dfrac{\d x}{x^4-1}\dd x
\\ \qquad
= \int \left(\dfrac{1}{4(x-1)}-\dfrac{1}{4(x+1)}-\dfrac{1}{2(x^2+1)}\right)\dd x
\\ \qquad
= \hl{\dfrac{1}{4}\ln|x-1| - \dfrac{1}{4}\ln|x+1| -\dfrac{1}{2}\tan^{-1}(x) + k}
$$

+++

---
[{b}]

$$<<< \int \dfrac{4x+1}{x^2+x+3}\dd x$$

+++
Solución
+++

$x^2+x+3$ no tiene raíces reales

$$x^2+x+3=0\Longrightarrow x=\dfrac{-1\pm\sqrt{1^2-4\cdot 1\cdot 3}}{2}=\dfrac{-1\pm\sqrt{-11}}{2}$$

De hecho,

$$\left(x+\dfrac{1}{2}\right)^2=x^2+x+\dfrac{1}{4}$$
$$x^2+x+3=\left(x+\dfrac{1}{2}\right)^2+\dfrac{11}{4}$$
$$4x+1=4\left(x+\dfrac{1}{2}\right)-1$$
$$\dfrac{4x+1}{x^2+x+3}=\dfrac{4\left(x+\frac{1}{2}\right)}{\left(x+\frac{1}{2}\right)^2+\frac{11}{4}}-\dfrac{1}{\left(x+\frac{1}{2}\right)^2+\frac{11}{4}}$$

Por tanto

$$<<< 
\int \dfrac{4x+1}{x^2+x+3}\dd x
\\ \qquad
= \int \left(\dfrac{4\left(x+\frac{1}{2}\right)}{\left(x+\frac{1}{2}\right)^2+\frac{11}{4}}-\dfrac{1}{\left(x+\frac{1}{2}\right)^2+\frac{11}{4}}\right)\dd x
\\ \qquad
= 2\ln\left|\left(x+\dfrac{1}{2}\right)^2+\frac{11}{4}\right|-\dfrac{1}{\sqrt{\frac{11}{4}}}\tan^{-1}\left(\dfrac{x+\frac{1}{2}}{\sqrt{\frac{11}{4}}}\right) + k
\\ \qquad
= \hl{2\ln|x^2+x+3|-\dfrac{2}{\sqrt{11}}\tan^{-1}\left(\dfrac{2x+1}{\sqrt{11}}\right) + k}$$

+++

---
[{c}]

$$<<< \int \dfrac{2x^2+7x-1}{x^3+x^2-x-1}\dd x$$

+++
Solución
+++

Descompongamos en fracciones simples:

$$x^3+x^2-x-1=(x+1)(x^2-1)=(x+1)^2(x-1)$$
$$\dfrac{2x^2+7x-1}{x^3+x^2-x-1} \\
= \dfrac{A}{x-1}+\dfrac{B}{x+1}+\dfrac{C}{(x+1)^2}$$
$$2x^2+7x-1 = A(x+1)^2+B(x-1)(x+1)+C(x-1)$$
$$x=-1\leadsto -6=2\cdot (-1)^2+7\cdot (-1)-1 \\
= A(-1+1)^2+B(-1-1)(-1+1)+C(-1-1)=-2C\Longrightarrow C=3$$
$$x=1\leadsto 8=2\cdot 1^2+7\cdot 1-1 \\
= A(1+1)^2+B(1-1)(1+1)+C(1-1)=4A\Longrightarrow A=2$$
$$4x+7=(2x^2+7x-1)'=(A(x+1)^2+B(x-1)(x+1)+C(x-1))' \\
= 2A(x+1)+B(x+1)+B(x-1)+C$$
$$x=-1\leadsto 3=4\cdot(-1)+7=2A(-1+1)+B(-1+1)+B(-1-1)+C \\
= -2B+3\Longrightarrow B=0$$


Por tanto

$$<<< 
\int \dfrac{2x^2+7x-1}{x^3+x^2-x-1}\dd x
\\ \qquad
= \int \left(\dfrac{2}{x-1}+\dfrac{3}{(x+1)^2}\right)\dd x
\\ \qquad
= \hl{2\ln|x-1|-\dfrac{3}{x+1} + k}
$$

+++

---
[{d}]

$$<<< \int \dfrac{3x+2}{x^3+4x^2+4x}\dd x$$

+++
Solución
+++

Descompongamos en fracciones simples:

$$x^3+4x^2+4x=x(x^2+4x+4)=x(x+2)^2$$
$$\dfrac{3x+2}{x^3+4x^2+4x}=\dfrac{A}{x}+\dfrac{B}{x+2}+\dfrac{C}{(x+2)^2}$$
$$3x+2 = A(x+2)^2+Bx(x+2)+Cx$$
$$x=-2\leadsto -4=3\cdot (-2)+2 = A(-2+2)^2+B(-2)(-2+2)+C(-2) \\
= -2C\Longrightarrow C=2$$
$$x=0\leadsto 2=3\cdot 0+2=A(0+2)^2+B\cdot 0(0+2)+C\cdot 0 \\
= 4A\Longrightarrow A=\dfrac{1}{2}$$
$$3=(3x+2)'=(A(x+2)^2+Bx(x+2)+Cx)'=2A(x+2)+B(x+2)+Bx+C$$
$$x=-2\leadsto 3=2A(-2+2)+B(-2+2)+B\cdot (-2)+C \\
= -2B+2\Longrightarrow B=-\dfrac{1}{2}$$

Por tanto

$$<<< 
\int \dfrac{3x+2}{x^3+4x^2+4x}\dd x
\\ \qquad
= \int \left(\dfrac{1}{2x}-\dfrac{1}{2(x+2)}+\dfrac{2}{(x+2)^2}\right)\dd x
\\ \qquad
= \hl{\dfrac{1}{2}\ln|x|-\dfrac{1}{2}\ln|x+2|-\dfrac{2}{x+2} + k}
$$

+++

---
[{e}]

$$<<< \int \dfrac{3x+4}{x^2+4x+3}\dd x$$

+++
Solución
+++

Descompongamos en fracciones simples:

$$x^2+4x+3=(x+1)(x+3)$$
$$\dfrac{3x+4}{x^2+4x+3}=\dfrac{A}{x+1}+\dfrac{B}{x+3}$$
$$3x+4 = A(x+3)+B(x+1)$$
$$x=-3\leadsto -5=3\cdot (-3)+4 = A(-3+3)+B(-3+1)=-2B\Longrightarrow B=\dfrac{5}{2}$$
$$x=-1\leadsto 1=3\cdot (-1)+4 = A(-1+3)+B(-1+1)=2A\Longrightarrow A=\dfrac{1}{2}$$

Por tanto

$$<<< 
\int \dfrac{3x+4}{x^2+4x+3}\dd x
\\ \qquad
= \int \left(\dfrac{1}{2(x+1)}+\dfrac{5}{2(x+3)}\right)\dd x
\\ \qquad
= \hl{\dfrac{1}{2}\ln|x+1| + \dfrac{5}{2}\ln|x+3| + k}
$$

+++