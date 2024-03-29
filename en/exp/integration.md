Integration may be thought as the inverse problem of differentiation: instead of differentiating a function

$$(\sqrt{e^x+1})'=\dfrac{1}{2\sqrt{e^x+1}}e^x=\dfrac{e^x}{2\sqrt{e^x+1}}$$

we're looking for _a function whose derivative is the function given_:

$$\int\sqrt{e^x+1}\dd x=2\sqrt{e^x+1}+\ln(\sqrt{e^x+1}-1)-\ln(\sqrt{e^x+1}+1) + k$$

where $k$ is some constant of choice, say $0$, $456$, $-\dfrac{3}{7}$, anything. And it works!

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

Wow! We say that 

$$2\sqrt{e^x+1}+\ln(\sqrt{e^x+1}-1)-\ln(\sqrt{e^x+1}+1) + k$$

is the **indefinite integral** of

$$\sqrt{e^x+1}$$

But how on earth could we compute this humongous function? Well, that's a crucial difference between differentiation and integration: to differentiate, one has to follow a set of rules, whereas to integrate, _there is no set of rules that work for every function_. One can only have a set of tricks that may work, and we'll study these rules through the chapter

Why the $k$? The derivative of a function is always unique, but this is not the case with integration:

$$((x+3)^2)'=2(x+3)=2x+6$$
$$(x^2+6x)'=2x+6$$
$$(x+3)^2\neq x^2+6x$$

Instead it is _unique up to a constant_, because if two functions have the same derivative, its difference has to be a constant

$$(x+3)^2-(x^2+6x)=9$$

Once a candidate for integral is found,

$$F'(x)=f(x)$$

adding a constant will preserve this quality

$$(F(x)+k)'=f(x)$$

so we always include this constant $k$ symbolically

$$\int f(x)\dd x=F(x)+k$$

and thus the integral is called _indefinite_. And why all this funny stuff of $\displaystyle\int$ and $\d x$? We'll talk about it when we study definite integrals in the next chapter.