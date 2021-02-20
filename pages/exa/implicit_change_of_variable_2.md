Let's work on the integral

$$\int\dfrac{1}{1+\cos x}\dd x$$

The best way to solve this integral is to realize that $1+\cos x=2\cos^2\left(\dfrac{x}{2}\right)$, which would lead immediately to 

$$\int\dfrac{1}{1+\cos x}\dd x=\tan\left(\dfrac{x}{2}\right)+k$$

but in case one does not catch on, an implicit change of variable will be useful again. Suppose we proceed in an explicit way:

$$t =\tan\left(\dfrac{x}{2}\right)$$
$$\d t = \dfrac{1}{2}\left(1+\tan^2\left(\dfrac{x}{2}\right)\right)\dd x$$

And $\dfrac{1}{2}\left(1+\tan^2\left(\dfrac{x}{2}\right)\right)=\dfrac{1}{1+\cos x}$, so we would have indeed

$$\int\dfrac{1}{1+\cos x}\dd x=\int\d t=t+k=\tan\left(\dfrac{x}{2}\right)+k$$

which essentially is the same as above. But: would the integrand be slightly different, the change of variable could not have been applied. Instead, an implicit change of variable $h(t)=x$ is _always_ appliable - we'll stress this subtlety later. For now, we take the form

$$2\tan^{-1}t =x$$
$$\dfrac{2}{1+t^2}\dd t = \d x$$

We also need to express $\cos x$ in terms of $t$: if $\tan\left(\dfrac{x}{2}\right)=t$, then (check it!)

$$\tan x=\dfrac{2t}{1-t^2}$$
$$\sin x=\dfrac{2t}{1+t^2}$$
$$\cos x=\dfrac{1-t^2}{1+t^2}$$

and therefore

$$
\int\dfrac{1}{1+\cos x}\dd x
= \int\dfrac{1}{1+\frac{1-t^2}{1+t^2}}\dfrac{2}{1+t^2}\dd t=\int\d t \\
= t+k =\tan\left(\dfrac{x}{2}\right)+k
$$

Smart, isn't it? But it doesn't seem to outperform the explicit change of variable, so we will slightly modify our integrand

$$\int\dfrac{1}{2+\cos x}\dd x$$

Now the integral is not immediate nor the term  $\dfrac{1}{2}\left(1+\tan^2\left(\dfrac{x}{2}\right)\right)=\dfrac{1}{1+\cos x}$ appears. But the implicit change of variable is easily applied

$$
\int\dfrac{1}{2+\cos x}\dd x
= \int\dfrac{1}{2+\frac{1-t^2}{1+t^2}}\dfrac{2}{1+t^2}\dd t \\
= \int\dfrac{2}{3+t^2}\dd t=\dfrac{2}{\sqrt{3}}\tan^{-1}\left(\dfrac{t}{\sqrt{3}}\right)+k 
= \dfrac{2}{\sqrt{3}}\tan^{-1}\left(\dfrac{\tan\left(\frac{x}{2}\right)}{\sqrt{3}}\right)+k
$$

Amazing! It's your turn to differentiate and check that everything works fine