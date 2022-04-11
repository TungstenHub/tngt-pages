[{a}]

$$<<<  \int \tan x\dd x$$

+++
Solución
+++

$$<<<  
\int \tan x\dd x
\\ \qquad 
= \int \dfrac{\sin x}{\cos x}\dd x
\oveq{ t=\cos x\\ \d t=-\sin x\dd x }
-\int \dfrac{1}{t}\dd t
\\ \qquad 
= -\ln|t| + k
\oveq{ t=\cos x }
\hl{-\ln|\cos x| + k}
$$

+++

---
[{b}]

$$<<<  \int \dfrac{\ln(x^4)}{x}\dd x$$

+++
Solución
+++

$$<<<  
\int \dfrac{\ln(x^4)}{x}\dd x
\\ \qquad 
= 4\int \dfrac{\ln x}{x}\dd x
\oveq{ t=\ln x\\ \d t=\frac{1}{x}\dd x }
4\int t\dd t
\\ \qquad 
= 2t^2 + k
\oveq{ t=\ln x }
\hl{2(\ln x)^2 + k}
$$

+++

---
[{c}]

$$<<<  \int \dfrac{e^{\sqrt{x}}}{\sqrt{x}}\dd x$$

+++
Solución
+++

$$<<<  
\int \dfrac{e^{\sqrt{x}}}{\sqrt{x}}\dd x
\\ \qquad 
= 2\int \dfrac{e^{\sqrt{x}}}{2\sqrt{x}}\dd x
\oveq{ t=\sqrt{x}\\ \d t=\frac{1}{2\sqrt{x}}\dd x }
2\int e^t\dd t
\\ \qquad 
= 2e^t + k
\oveq{ t=\sqrt{x} }
\hl{2e^{\sqrt{x}} + k}
$$

+++

---
[{d}]

$$<<<  \int \dfrac{x}{\sqrt{1+x^2}}\dd x$$

+++
Solución
+++

$$<<<  
\int \dfrac{x}{\sqrt{1+x^2}}\dd x
\\ \qquad 
= \dfrac{1}{2}\int \dfrac{2x}{\sqrt{1+x^2}}\dd x
\oveq{ t=1+x^2\\ \d t=2x\dd x }
\dfrac{1}{2}\int \dfrac{1}{\sqrt{t}}\dd t
\\ \qquad 
= \sqrt{t} + k
\oveq{ t=1+x^2 }
\hl{\sqrt{1+x^2} + k}
$$

+++

---
[{e}]

$$<<<  \int \dfrac{3x+2}{4+x^2}\dd x$$

+++
Solución
+++

$$<<<  
\int \dfrac{3x+2}{4+x^2}\dd x
= 3\int \dfrac{x}{4+x^2}\dd x+2\int \dfrac{1}{4+x^2}\dd x
$$

Vamos con la primera parte:

$$<<<  
\int \dfrac{x}{4+x^2}\dd x
\\ \qquad 
= \dfrac{1}{2}\int \dfrac{2x}{4+x^2}\dd x
\oveq{ t=4+x^2\\ \d t=2x\dd x }
\dfrac{1}{2}\int \dfrac{1}{t}\dd t
\\ \qquad 
=\dfrac{1}{2}\ln|t| + k
\oveq{ t=4+x^2 }
\dfrac{1}{2}\ln|4+x^2| + k = \dfrac{1}{2}\ln(4+x^2) + k
$$

En cuanto a la segunda parte, sabemos de un [ejercicio previo]( prb | change_variable_1 # b ) que:

$$<<<  
\dfrac{1}{4+x^2}\dd x
= \dfrac{1}{2}\tan^{-1}\left(\dfrac{x}{2}\right) + k
$$

Así que sumando todo nos queda

$$<<<  
\int \dfrac{3x+2}{4+x^2}\dd x
= \hl{\dfrac{3}{2}\ln(4+x^2) + \tan^{-1}\left(\dfrac{x}{2}\right) + k}
$$

+++