Si $F'(x)=f(x)$, entonces $(F(g(x)))'=f(g(x))g'(x)$. De este modo, la integral de una función del tipo

$$\int f(g(x))g'(x)\dd x$$

siempre se resuelve como

$$\int f(g(x))g'(x)\dd x=F(g(x))+k$$

Es muy útil efectuar este truco como un _cambio de variable_: sea

$$t=g(x)$$

Si derivamos ambos lados de la expresión y señalamos la variable con respecto a la que estamos derivando con $\d \cdot$, tenemos

$$\d t = g'(x)\dd x$$

y la expresión de arriba se puede manejar más fácilmente

$$\int f(g(x))g'(x)\dd x\oveq{g(x)=t\\g'(x)\dd x=\dd t}\int f(t)\dd t=F(t)+k\oveq{t=g(x)}F(g(x))+k$$

Esto nos lleva a una lista de "integrales semi-inmediatas": si $t$ es alguna función de $x$,

$$
\int t^n\cdot t' \dd x=\dfrac{t^{n+1}}{n+1}+k\qquad \text{if $n\neq -1$}
$$
$$ 
\int \dfrac{t'}{t}\dd x=\ln\vert t\vert+k
$$
$$
\int e^t\cdot t' \dd x= e^t+k
$$
$$
\int a^t\cdot t' \dd x= \dfrac{a^t}{\ln a}+k
$$
$$
\int \sin t\cdot t' \dd x= -\cos t+k
$$
$$
\int \cos t\cdot t' \dd x= \sin t+k 
$$
$$
\int \dfrac{t'}{1+t^2} \dd x = \tan^{-1} t+k 
$$
$$
\int \left(1+\tan^2 t\right)\cdot t' \dd x= \int \dfrac{t'}{\cos^2 t} \dd x = \tan t+k 
$$
$$
\int \dfrac{t'}{\sqrt{1-t^2}} \dd x = \sin^{-1} t+k
$$
$$
\int \dfrac{t'}{\sqrt{1+t^2}} \dd x = \sinh^{-1} t+k
$$
