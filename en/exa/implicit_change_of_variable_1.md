Let's work on the integral

$$\int\sqrt{1-x^2}\dd x$$

for which an implicit change of variable will be very useful:

$$\sin t =x$$
$$\cos t \dd t = \d x$$

Since the right hand side is just $\d x$, this change may always be applied. All implicit changes of variable of the type $h(t)=x$ are directly appliable; whether these changes simplify or complicate the integrand is more subtle. In this case, the change works like a charm

$$
\int\sqrt{1-x^2}\dd x
\oveq{ \sin t =x\\ \cos t \dd t = \d x }
\int\sqrt{1-\sin^2(t)}\cos t \dd t=\int\cos^2(t) \dd t
$$

Our new integrand is indeed simpler: $\cos(2t)=\cos^2(t) – \sin^2(t) = 2\cos^2(t) – 1\Longrightarrow \cos^2(t)=\dfrac{1+\cos(2t)}{2}$, and 

$$\int\cos^2(t) \dd t=\int\dfrac{1+\cos(2t)}{2}\dd t=\dfrac{1}{2}t+\dfrac{1}{4}\sin(2t)+k$$

Now we undo our change (keep in mind that $\sin(2t)=2\sin t\cos t$)

$$
\dfrac{1}{2}t+\dfrac{1}{4}\sin(2t)+k
\oveq{ \sin t =x\\ t=\sin^{-1} x }
\dfrac{1}{2}\sin^{-1} x+\dfrac{1}{2}x\sqrt{1-x^2}+k \\
=\dfrac{1}{2}\left(x\sqrt{1-x^2}+\sin^{-1} x\right)+k
$$

Great!! Let's differentiate to check that everything is peachy

$$
\left(\dfrac{1}{2}\left(x\sqrt{1-x^2}+\sin^{-1} x\right)+k\right)'
=\dfrac{1}{2}\left(\left[\sqrt{1-x^2}+x\dfrac{-2x}{2\sqrt{1-x^2}}\right]+\dfrac{1}{\sqrt{1-x^2}}\right) \\
=\dfrac{(1-x^2)-x^2+1}{2\sqrt{1-x^2}}
=\sqrt{1-x^2}
$$