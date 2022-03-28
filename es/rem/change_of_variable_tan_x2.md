The change of variable used in the previous example

$$t=\tan\left(\dfrac{x}{2}\right)$$
$$2\tan^{-1}t =x$$
$$\dfrac{2}{1+t^2}\dd t = \d x$$

may seem rather strange, but is indeed very useful. The ultimate reason for this choice is that all trigonometric functions are transformed into rational functions (polynomial quotients)

$$\tan x=\dfrac{2t}{1-t^2}$$
$$\sin x=\dfrac{2t}{1+t^2}$$
$$\cos x=\dfrac{1-t^2}{1+t^2}$$

and there are [rules to integrate all rational functions](exp | integration_rational_functions), as we will see later; therefore integrals involving trigonometric functions and additions, substractions, products and quotients may_always_ be integrated with this change of variable. The simpler change of variable

$$t =\tan x$$
$$\tan^{-1}t =x$$
$$\dfrac{1}{1+t^2}\dd t = \d x$$

would not work here, since in this case $\sin x$ and $\cos x$ involve square roots

$$\tan x=t$$
$$\sin x=\dfrac{t}{\sqrt{1+t^2}}$$
$$\cos x=\dfrac{1}{\sqrt{1+t^2}}$$

However, sometimes other techniques may be shorter (especially for [powers of sines and cosines](exp | integration_powers_trig_functions)). For instance

$$
\int \sin^2 x\cos x\dd x
\oveq{ t=\tan\left(\frac{x}{2}\right)\\ 2\tan^{-1}t =x \\ \frac{2}{1+t^2}\dd t = \d x  }
\int \left(\dfrac{2t}{1+t^2}\right)^2\dfrac{1-t^2}{1+t^2}\dfrac{2}{1+t^2}\dd t \\
= 8\int \dfrac{t^2(1-t^2)}{(1+t^2)^4}\dd t
$$

leads to a tedious rational function, whereas a wiser change of variable

$$ 
\int \sin^2 x\cos x\dd x
\oveq{ t=\sin x\\ \d t=\cos x\dd x }
\int t^2\dd t \\
= \dfrac{1}{3}t^3 + k
\oveq{ t=\sin x }
\dfrac{1}{3}\sin^3 x + k 
$$

solves it immediately