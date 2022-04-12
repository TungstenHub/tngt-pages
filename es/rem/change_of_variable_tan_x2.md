El cambio de variable utilizado en el ejemplo anterior

$$t=\tan\left(\dfrac{x}{2}\right)$$
$$2\tan^{-1}t =x$$
$$\dfrac{2}{1+t^2}\dd t = \d x$$

puede parecer un poco extraño, pero en realidad es muy útil. Y la razón de hacer esta elección es que todas las funciones trigonométricas se convierten en funciones racionales (cocientes de polinomios)

$$\tan x=\dfrac{2t}{1-t^2}$$
$$\sin x=\dfrac{2t}{1+t^2}$$
$$\cos x=\dfrac{1-t^2}{1+t^2}$$

y hay [reglas para integrar las funciones racionales](exp | integration_rational_functions), como veremos más tarde; de este modo, integrales que involucran funciones trigonométricas y sumas, restas, multiplicaciones y divisiones se pueden integrar _siempre_ con este cambio de variable. El cambio de variable más simple

$$t =\tan x$$
$$\tan^{-1}t =x$$
$$\dfrac{1}{1+t^2}\dd t = \d x$$

no funcionaría aquí porque en este caso $\sin x$ y $\cos x$ involucran raíces cuadradas

$$\tan x=t$$
$$\sin x=\dfrac{t}{\sqrt{1+t^2}}$$
$$\cos x=\dfrac{1}{\sqrt{1+t^2}}$$

Sin embargo, a veces otras técnicas pueden ser más cortas (especialmente para [potencias de senos y cosenos](exp | integration_powers_trig_functions)). Por ejemplo

$$
\int \sin^2 x\cos x\dd x
\oveq{ t=\tan\left(\frac{x}{2}\right)\\ 2\tan^{-1}t =x \\ \frac{2}{1+t^2}\dd t = \d x  }
\int \left(\dfrac{2t}{1+t^2}\right)^2\dfrac{1-t^2}{1+t^2}\dfrac{2}{1+t^2}\dd t \\
= 8\int \dfrac{t^2(1-t^2)}{(1+t^2)^4}\dd t
$$

lleva a una función racional tremendamente liosa, mientras que un cambio de variable más avispado

$$ 
\int \sin^2 x\cos x\dd x
\oveq{ t=\sin x\\ \d t=\cos x\dd x }
\int t^2\dd t \\
= \dfrac{1}{3}t^3 + k
\oveq{ t=\sin x }
\dfrac{1}{3}\sin^3 x + k 
$$

la resuelve inmediatamente