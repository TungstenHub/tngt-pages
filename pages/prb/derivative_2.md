[{a}]

$$<<< \left[\dfrac{x+\sin x}{x-\sin x}\right]' $$

+++
Solution
+++

$$<<< 
\left[\dfrac{x+\sin x}{x-\sin x}\right]'
\\ \qquad
= \dfrac{[x+\sin x]'(x-\sin x)-(x+\sin x)[x-\sin x]'}{(x-\sin x)^2}
\\ \qquad
= \dfrac{(1+\cos x)(x-\sin x)-(x+\sin x)(1-\cos x)}{(x-\sin x)^2}
\\ \qquad
= \dfrac{(x-\sin x+x\cos x-\sin x\cos x)-(x+\sin x-x\cos x-\sin x\cos x)}{(x-\sin x)^2}
\\ \qquad
= \hl{2\dfrac{x\cos x-\sin x}{(x-\sin x)^2}}
$$

+++

---
[{b}]

$$<<< \left[\dfrac{e^x+e^{-x}}{2}\right]' $$

+++
Solution
+++

$$<<< \left[\dfrac{e^x+e^{-x}}{2}\right]'= \hl{\dfrac{e^x-e^{-x}}{2}} $$

Tip: these are the hyperbolic cosine and sine

$$\sinh x=\dfrac{e^x-e^{-x}}{2}$$
$$\cosh x=\dfrac{e^x+e^{-x}}{2}$$

and satisfy

$$[\sinh x]'=\cosh x$$
$$[\cosh x]'=\sinh x$$

+++

---
[{c}]

$$<<< \left[\dfrac{e^x-e^{-x}}{e^x+e^{-x}}\right]' $$

+++
Solution
+++

$$<<< 
\left[\dfrac{e^x-e^{-x}}{e^x+e^{-x}}\right]'
\\ \qquad
= \dfrac{[e^x-e^{-x}]'(e^x+e^{-x})-(e^x-e^{-x})[e^x+e^{-x}]'}{(e^x+e^{-x})^2}
\\ \qquad
= \dfrac{(e^x+e^{-x})(e^x+e^{-x})-(e^x-e^{-x})(e^x-e^{-x})}{(e^x+e^{-x})^2}
\\ \qquad
= \dfrac{(e^{2x}+2+e^{-2x})-(e^{2x}-2+e^{-2x})}{(e^x+e^{-x})^2}
\\ \qquad
= \hl{\dfrac{4}{(e^x+e^{-x})^2}}
$$

Tip: this is the hyperbolic tangent

$$\tanh x=\dfrac{\sinh x}{\cosh x}=\dfrac{e^x-e^{-x}}{e^x+e^{-x}}$$

and its derivative is

$$[\tanh x]'=\dfrac{4}{(e^x+e^{-x})^2}=\dfrac{1}{\cosh^2(x)}$$

Quite similar to the usual trigonometric functions, aren't they?

+++

---
[{d}]

$$<<< \left[\sqrt{3x\tan(x^3)}\right]' $$

+++
Solution
+++

$$<<< 
\left[\sqrt{3x\tan(x^3)}\right]'
\\ \qquad
= \dfrac{1}{2\sqrt{3x\tan(x^3)}}[3x\tan(x^3)]'
\\ \qquad
= \dfrac{3}{2\sqrt{3x\tan(x^3)}}[x\tan(x^3)]'
\\ \qquad
= \dfrac{\sqrt{3}}{2\sqrt{x\tan(x^3)}}(\tan(x^3)+x(1+\tan^2(x^3))3x^2)
\\ \qquad
= \hl{\dfrac{\sqrt{3}(3x^3(1+\tan^2(x^3))+\tan(x^3))}{2\sqrt{x\tan(x^3)}}}
$$

+++

---
[{e}]

$$<<< \left[e^{\sin(4x)}\right]' $$

+++
Solution
+++

$$<<< 
\left[e^{\sin(4x)}\right]'
\\ \qquad
= e^{\sin(4x)}[\sin(4x)]'
\\ \qquad
= \hl{4e^{\sin(4x)}\cos(4x)}
$$

+++