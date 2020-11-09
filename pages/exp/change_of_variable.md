If $F'(x)=f(x)$, then $(F(g(x)))'=f(g(x))g'(x)$. Thus, the integral of a function of the type 

$$\int f(g(x))g'(x)\dd x$$

is always solved as 

$$\int f(g(x))g'(x)\dd x=F(g(x))+k$$

It is very useful to denote this trick with a *change of variable*: let

$$t=g(x)$$

If we differentiate both sides of the expression and keep track of variable with respect to which we are differentiating with $\d \cdot$, we get

$$\d t = g'(x)\dd x$$

and the expression above is more easily handed

$$\int f(g(x))g'(x)\dd x\oveq{g(x)=t\\g'(x)\dd x=\dd t}\int f(t)\dd t=F(t)+k\oveq{t=g(x)}F(g(x))+k$$

This also leads to a list of "semi-immediate integrals": if $t$ is some function of $x$,

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
