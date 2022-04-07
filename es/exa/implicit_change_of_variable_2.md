Vamos ahora con la integral

$$\int\dfrac{1}{1+\cos x}\dd x$$

La mejor manera de resolver esta integral es darse cuenta de que $1+\cos x=2\cos^2\left(\dfrac{x}{2}\right)$, que conduciría inmediatamente a

$$\int\dfrac{1}{1+\cos x}\dd x=\tan\left(\dfrac{x}{2}\right)+k$$

pero en el caso en que uno no se dé cuenta, un cambio de variable implícito volverá a ser de utilidad. Supongamos que procedemos de un modo explícito:

$$t =\tan\left(\dfrac{x}{2}\right)$$
$$\d t = \dfrac{1}{2}\left(1+\tan^2\left(\dfrac{x}{2}\right)\right)\dd x$$

Y $\dfrac{1}{2}\left(1+\tan^2\left(\dfrac{x}{2}\right)\right)=\dfrac{1}{1+\cos x}$, así que tendríamos de hecho

$$\int\dfrac{1}{1+\cos x}\dd x=\int\d t=t+k=\tan\left(\dfrac{x}{2}\right)+k$$

que es esencialmente lo mismo que antes. Sin embargo: si el integrando fuese ligeramente distinto, el cambio de variable no se podría haber aplicado. En contraposición a esto, un cambio de variable implícito $h(t)=x$ _siempre_ es aplicable - más tarde pondremos énfasis en este punto. Por ahora tomamos el cambio

$$2\tan^{-1}t =x$$
$$\dfrac{2}{1+t^2}\dd t = \d x$$

También necesitamos expresar $\cos x$ en términos de $t$: si $\tan\left(\dfrac{x}{2}\right)=t$, entonces (¡compruébalo!)

$$\tan x=\dfrac{2t}{1-t^2}$$
$$\sin x=\dfrac{2t}{1+t^2}$$
$$\cos x=\dfrac{1-t^2}{1+t^2}$$

y por tanto

$$
\int\dfrac{1}{1+\cos x}\dd x
= \int\dfrac{1}{1+\frac{1-t^2}{1+t^2}}\dfrac{2}{1+t^2}\dd t=\int\d t \\
= t+k =\tan\left(\dfrac{x}{2}\right)+k
$$

Ingenioso, ¿verdad? Como no parece superar al cambio de variable explícito, vamos a modificar ligeramente nuestro integrando

$$\int\dfrac{1}{2+\cos x}\dd x$$

Ahora la integral ni es inmediata ni aparece el término $\dfrac{1}{2}\left(1+\tan^2\left(\dfrac{x}{2}\right)\right)=\dfrac{1}{1+\cos x}$. Pero el cambio de variable implícito se aplica fácilmente

$$
\int\dfrac{1}{2+\cos x}\dd x
= \int\dfrac{1}{2+\frac{1-t^2}{1+t^2}}\dfrac{2}{1+t^2}\dd t \\
= \int\dfrac{2}{3+t^2}\dd t=\dfrac{2}{\sqrt{3}}\tan^{-1}\left(\dfrac{t}{\sqrt{3}}\right)+k 
= \dfrac{2}{\sqrt{3}}\tan^{-1}\left(\dfrac{\tan\left(\frac{x}{2}\right)}{\sqrt{3}}\right)+k
$$

¡Increíble! Es tu turno de derivar y comprobar que todo va bien