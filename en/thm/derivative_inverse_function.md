[{inverse}]

The derivative of the inverse function may be found with the following interesting trick: suppose that 

$$g=f^{-1}$$

and therefore

$$f(g(x))=x$$

Let's differentiate both sides of the equality and reorder everything

$$f'(g(x))g'(x)=1$$
$$g'(x)=\dfrac{1}{f'(g(x))}$$

Let's see this trick in action with some examples

---
[{logarithm}]

Suppose we know the derivative of the exponential $\exp$ but not that of the logarithm $\ln$

$$\exp(\ln(x))=x$$
$$\exp'(\ln(x))\ln'(x)=1$$
$$\ln'(x)=\dfrac{1}{\exp'(\ln(x))}=\dfrac{1}{\exp(\ln(x))}=\dfrac{1}{x}$$

---
[{arcsinus}]

Suppose we know the derivative of the sinus $\sin$ but not that of the arcsinus $\sin^{-1}$

$$\sin(\sin^{-1}(x))=x$$
$$\sin'(\sin^{-1}(x))[\sin^{-1}]'(x)=1$$
$$[\sin^{-1}]'(x)=\dfrac{1}{\sin'(\sin^{-1}(x))}=\dfrac{1}{\cos(\sin^{-1}(x))}=\dfrac{1}{\sqrt{1-\sin^2(\sin^{-1}(x))}}=\dfrac{1}{\sqrt{1-x^2}}$$

---
[{arctangent}]

Suppose we know the derivative of the tangent $\tan$ but not that of the arctangent $\tan^{-1}$

$$\tan(\tan^{-1}(x))=x$$
$$\tan'(\tan^{-1}(x))[\tan^{-1}]'(x)=1$$
$$[\tan^{-1}]'(x)=\dfrac{1}{\tan'(\tan^{-1}(x))}=\dfrac{1}{1+\tan^2(\tan^{-1}(x))}=\dfrac{1}{1+x^2}$$