Se puede entender la integración como el problema inverso de la derivación: en vez de derivar una función

$$(\sqrt{e^x+1})'=\dfrac{1}{2\sqrt{e^x+1}}e^x=\dfrac{e^x}{2\sqrt{e^x+1}}$$

buscamos _una función cuya derivada es la función que nos dan_:

$$\int\sqrt{e^x+1}\dd x=2\sqrt{e^x+1}+\ln(\sqrt{e^x+1}-1)-\ln(\sqrt{e^x+1}+1) + k$$

donde $k$ es una constante cualquiera, por ejemplo $0$, $456$, $-\dfrac{3}{7}$, lo que sea. ¡Y funciona!

$$
\begin{array}{l}
(2\sqrt{e^x+1}+\ln(\sqrt{e^x+1}-1)-\ln(\sqrt{e^x+1}+1) + k)' \\[1.5em]
\qquad = 2\dfrac{e^x}{2\sqrt{e^x+1}}+\dfrac{1}{\sqrt{e^x+1}-1}\dfrac{e^x}{2\sqrt{e^x+1}}-\dfrac{1}{\sqrt{e^x+1}+1}\dfrac{e^x}{2\sqrt{e^x+1}}\\[1.5em]
\qquad = \dfrac{e^x}{2\sqrt{e^x+1}}\left(2+\dfrac{1}{\sqrt{e^x+1}-1}-\dfrac{1}{\sqrt{e^x+1}+1}\right)\\[1.5em]
\qquad = \dfrac{e^x}{2\sqrt{e^x+1}}\left(2+\dfrac{\sqrt{e^x+1}+1}{e^x}-\dfrac{\sqrt{e^x+1}-1}{e^x}\right)\\[1.5em]
\qquad = \dfrac{e^x}{2\sqrt{e^x+1}}\left(2+\dfrac{2}{e^x}\right)\\[1.5em]
\qquad = \dfrac{e^x+1}{\sqrt{e^x+1}}\\[1.5em]
\qquad = \sqrt{e^x+1}\\
\end{array}
$$

¡Wow! Decimos que

$$2\sqrt{e^x+1}+\ln(\sqrt{e^x+1}-1)-\ln(\sqrt{e^x+1}+1) + k$$

es la **integral indefinida** de

$$\sqrt{e^x+1}$$

¿Pero cómo porras vamos a calcular esta función enormísima? Bueno, hay una diferencia crucial entre derivar e integrar: para derivar, uno tiene que seguir una serie de reglas, mientras que para integrar, _no hay un conjunto de reglas que funcionen en todos los casos_. Uno solo tiene un conjunto de trucos que a veces funcionan; los estudiaremos en este capítulo

¿Por qué la $k$? La derivada de una función siempre es única, pero no ocurre lo mismo con la integración:

$$((x+3)^2)'=2(x+3)=2x+6$$
$$(x^2+6x)'=2x+6$$
$$(x+3)^2\neq x^2+6x$$

En cambio, _es única salvo constantes_, porque si dos funciones tienen la misma derivada, su diferencia tiene que ser una constante

$$(x+3)^2-(x^2+6x)=9$$

Una vez que se encuentra un candidato a integral,

$$F'(x)=f(x)$$

añadir una constante no va a cambiar mucho

$$(F(x)+k)'=f(x)$$

por lo que siempre incluimos esta constante $k$ simbólicamente

$$\int f(x)\dd x=F(x)+k$$

y por eso la integral se llama _indefinida_. ¿Y qué es todo ese rollo de $\displaystyle\int$ y $\d x$? Ya hablaremos de ello cuando veamos integrales definidas en el siguiente capítulo.