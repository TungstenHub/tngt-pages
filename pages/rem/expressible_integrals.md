We have said that there is no set of rules that work for every function. Indeed it is much more subtle than that. There are functions whose integral _is not expressible in terms of elementary functions_:

$$\int e^{-x^2}\dd x=???$$

What does this mean? Well, there _exist_ functions (unique up to a constant) whose derivative is $e^{-x^2}$

```sage
plot([exp(-x^2), sqrt(pi)/2*erf(x)], (x,-2,2), legend_label=['$e^{-x^2}$','$F(x)$'], thickness=3)
```

but these functions may not be expressed as a combination of sums, products, quotients, powers, roots, sines or cosines, exponentials or logarithms, or anything one has used so far, no matter how we combine them. Just that. If we want, we may come up with a new name for it, much like we have named all the other functions. In fact, this function (a multiple of it) has been given a name, and it's of crucial importance in Probability, Statistics and Partial Differential Equations: it's the **Gauss Error Function**:

$$\mathrm{erf}(x)=\dfrac{2}{\sqrt{\pi}}\int_0^x e^{-t^2}\dd t$$

(you may forget about this definition for now; it's a _definite integral_). And in fact any "malicious random function" won't have in general an integral expressible in terms of elementary functions

$$\int \sin(\sin(\sin(\sin x)))\dd x=???$$

so the set of functions whose integral may be solved explicitely (that is, whose integral is expressible in terms of elementary functions) is indeed very small