Toda función racional $\dfrac{P(x)}{Q(x)}$ (cociente de polinomios con coeficientes reales) [se puede descomponer en suma de un polinomio y múltiplos de fracciones simples](thm | partial_fraction_decomposition) del tipo  

$$\dfrac{1}{(x-a)^n}$$
$$\dfrac{A+Bx}{\left((x-a)^2+b^2\right)^n}$$

Por eso la integración de funciones racionales siempre se puede resolver, siempre y cuando sepamos resolver las integrales de estas fracciones simples. Las del primer tipo son inmediatas:

$$\int \dfrac{1}{x-a}\dd x=\ln\vert x-a\vert+k$$
$$\int \dfrac{1}{(x-a)^n} \dd x=-\dfrac{1}{n-1}\dfrac{1}{(x-a)^{n-1}}+k\qquad \text{si \(n\neq 1\)}$$

Para el segundo tipo, después de cambios de variable y manipulaciones, nos quedamos con fracciones del tipo

$$\dfrac{1}{(x^2+1)^n}$$
$$\dfrac{x}{(x^2+1)^n}$$

El cambio de variable $t=x^2+1$ funciona bien para el segundo caso

$$
\int \dfrac{x}{(x^2+1)^n} \dd x
\oveq{ t=x^2+1\\ \d t=2x\dd x }
\dfrac{1}{2}\int \dfrac{1}{t^n} \dd t
$$

Para el primer caso, el cambio de variable implícito $\tan t=x$ convierte todo en [potencias de cosenos](exp | integration_powers_trig_functions)

$$
\int \dfrac{1}{(x^2+1)^n} \dd x
\oveq{ \tan t=x\\ \frac{1}{\cos^2(t)}\dd t=\d x }
\int \dfrac{1}{\left(\tan^2(t)+1\right)^n}\dfrac{1}{\cos^2(t)} \dd t \\
= \int \dfrac{1}{\left(\frac{1}{\cos^2(t)}\right)^n}\dfrac{1}{\cos^2(t)} \dd t=
\int \cos^{2n-2}(t) \dd t
$$