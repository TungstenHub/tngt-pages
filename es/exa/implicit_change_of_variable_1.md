Vamos a trabajar con la integral

$$\int\sqrt{1-x^2}\dd x$$

para la que un cambio de variable implícito va a ser muy útil:

$$\sin t =x$$
$$\cos t \dd t = \d x$$

Como la parte de la derecha es simplemente $\d x$, este cambio siempre se puede aplicar. Todos los cambios de variable implícitos del tipo $h(t)=x$ se pueden aplicar directamente; que estos cambios simplifiquen o compliquen el integrando ya es otra cuestión. En este caso, el cambio funciona de maravilla

$$
\int\sqrt{1-x^2}\dd x
\oveq{ \sin t =x\\ \cos t \dd t = \d x }
\int\sqrt{1-\sin^2(t)}\cos t \dd t=\int\cos^2(t) \dd t
$$

Nuestro nuevo integrando se ha vuelto más simple: $\cos(2t)=\cos^2(t) – \sin^2(t) = 2\cos^2(t) – 1\Longrightarrow \cos^2(t)=\dfrac{1+\cos(2t)}{2}$, y 

$$\int\cos^2(t) \dd t=\int\dfrac{1+\cos(2t)}{2}\dd t=\dfrac{1}{2}t+\dfrac{1}{4}\sin(2t)+k$$

Ahora deshacemos el cambio (ten en cuenta que $\sin(2t)=2\sin t\cos t$)

$$
\dfrac{1}{2}t+\dfrac{1}{4}\sin(2t)+k
\oveq{ \sin t =x\\ t=\sin^{-1} x }
\dfrac{1}{2}\sin^{-1} x+\dfrac{1}{2}x\sqrt{1-x^2}+k \\
=\dfrac{1}{2}\left(x\sqrt{1-x^2}+\sin^{-1} x\right)+k
$$

¡Perfecto! Vamos a derivar para asegurarnos de que todo marcha bien

$$
\left(\dfrac{1}{2}\left(x\sqrt{1-x^2}+\sin^{-1} x\right)+k\right)'
=\dfrac{1}{2}\left(\left[\sqrt{1-x^2}+x\dfrac{-2x}{2\sqrt{1-x^2}}\right]+\dfrac{1}{\sqrt{1-x^2}}\right) \\
=\dfrac{(1-x^2)-x^2+1}{2\sqrt{1-x^2}}
=\sqrt{1-x^2}
$$